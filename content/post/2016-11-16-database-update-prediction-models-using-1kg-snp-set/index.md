---
title: 'Database update: prediction models using 1KG SNP set'
author: PredictDB Team
date: '2016-11-16'
slug: database-update-prediction-models-using-1kg-snp-set
categories:
  - News
tags: []
---
Today we are updating the tissue-wide prediction models trained from GTEx data which use 1000 Genomes SNPs. There are two main differences:

1. The snp covariance files we had provided previously were built using a reference dataset with 1000 genomes data. Now the covariance data is based off of the GTEx training data. This should resolve many issues with MetaXcan not being able to utilize all snps in models.

2. In the previous release of our GTEx 1000 Genomes models, we had mistakenly excluded some well-performing protein-coding gene models before filtering for statistical significance at the level of FDR < .05. We have now included these models in the databases. After including these genes though, some gene-tissue models that had previously just reached the threshold of statistical significance now no longer meet the necessary criteria. These models have been dropped appropriately. As these models were not predicted to have great performance anyway, we hope that few people, if any, will miss these models.

If you are using the GTEx 1000 Genomes models in your research, we ask you to rerun your analyses using these updated models.

