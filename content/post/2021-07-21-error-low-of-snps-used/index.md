---
title: Error low % of SNPs used
author: Festus
date: '2021-07-21'
slug: error-low-of-snps-used
categories:
  - FAQ
tags:
  - PrediXcan
  - SPrediXcan
---

## Possible explanation
There are different reasons where you could get a low % of SNPs in the model used with your individual level data or summary stats file. Some of the issues include;
  1. Little overlap between  the model SNPs and genotype/summary stats SNPs
  
  2. Incomplete/malformed models .db file especially when downloading
  
  3. Using only a few chromosomes to run prediXcan

## Possible solution
- Perform a "manual" inspection of the data. It is recommended you use an interactive environment like R or ipython - then load the model data and GWAS data and check the intersection of variants in model and GWAS.
- When using variant ids check if the model variant ids and the genotype/summary stats variant ids are in the same genome build. If they are not use the liftover option to generate a variant id that matches the models variant id.
    > The argument for the lift over is: \
    **_--liftover path/to/hg19ToHg38.over.chain.gz \
      --on_the_fly_mapping METADATA "chr{}_{}_{}_{}_b38"**
      
  On the fly mapping informs the tool how to recreate the variant name from the co ordinates to match the variant id format in the model.