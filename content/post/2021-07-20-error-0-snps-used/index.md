---
title: Error 0% SNPs used
author: Festus Nyasimi
date: '2021-07-20'
slug: error-0-snps-used
categories: [FAQ]
tags: [PrediXcan,SPrediXcan]
---

## Possible explanation
This error usually occurs when there is a mismatch between the SNP ids used in the model and those used in the genotype file or the summary stats file.
A few examples to mention;

    1. Using rsids in the models against variant ids (chr_pos_ref_alt_build) in the genotype and summary stats file and vice versa
    
    2. Using variant ids with different builds i.e the model has the ids in build hg37 while the genotype/summary stats file has the ids in build38 and vice versa. This could be any other build and not restricted to hg38 or hg37.
    
    3. Using totally different ids in your genotype/summary stats file which are not in the models (The elastic net models contain both rsids and variant ids while the mashr models contain only variant ids)


## Possible solutions
- When having different genome builds use chr{}*{}*{}_{}_b38" for the --on_the_fly_mapping argument. This parameter specifies a format string to be used when building a variant id from its (liftover coordinates) and alleles (genotype). Then these ids will be matched to the ids in the mashr/elastic net model, which are all hg38-based.
- When you have totally different ids that dont follow the rsid/variant id format you need to use a text variant mapping instead of on_the_fly_mapping. The textfile contains a map of the model ids in one column and the ids in the genotype in another column to provide information on how to map the id from the model to the genotype, you can use the file as below

    > The argument you would need to use is: \
    _**--variant_mapping /path/to/tab-separated-file.txt KEYNAME VALUENAME**_ \
    where: \
     a) path refers to a simple tabular file \
     b) **KEYNAME** is the name of the column with your input variants \
     c) **VALUENAME** is the name of the column with the mapped variant as existing in a model (NA would cause the model to be ignored)

- When you are using mashr models they don't use RSIDs so you need to let S-PrediXcan
 knows this is the case with the additional command line arguments:

    >--keep_non_rsid \
    --additional_output \
    --model_db_snp_key varID