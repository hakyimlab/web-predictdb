---
title: GTEx v8 models on eQTL and sQTL
author: PredictDB Team
date: '2021-07-21'
slug: gtex-v8-models-on-eqtl-and-sqtl
categories:
  - Downloads
  - Models
tags: []
---
We have produced different families of prediction models for sQTL and eQTL, using several prediction strategies, on GTEx v8 release data.

We recommend MASHR-based models below. Elastic Net-based are a safe, robust alternative with decreased power.

## MASHR-based models

Expression and splicing prediction models with LD reference data are available in this Zenodo repository.

Files:

- [mashr_eqtl.tar](https://zenodo.org/record/3518299/files/mashr_eqtl.tar?download=1): PrediXcan's and S-PrediXcan's support on expression
- [mashr_sqtl.tar](https://zenodo.org/record/3518299/files/mashr_sqtl.tar?download=1): PrediXcan's and S-PrediXcan's support on splicing
- [gtex_v8_expression_mashr_snp_smultixcan_covariance.txt.gz](https://zenodo.org/record/3518299/files/gtex_v8_expression_mashr_snp_smultixcan_covariance.txt.gz?download=1): S-MultiXcan expression's LD reference
- [gtex_v8_splicing_mashr_snp_smultixcan_covariance.txt.gz](https://zenodo.org/record/3518299/files/gtex_v8_splicing_mashr_snp_smultixcan_covariance.txt.gz?download=1): S-MultiXcan splicing's LD reference

> Note: if the download links don't work, use this [link to zenodo](https://zenodo.org/record/3518299/) and fine the files listed above and download them directly from the webpage

**Warning:** these models are based on fine-mapped variants that may occasionally be absent in a tipical GWAS, and frequently absent in older GWAS. We have tools to address this, presented [here](https://github.com/hakyimlab/MetaXcan/wiki/Best-practices-for-integrating-GWAS-and-GTEX-v8-transcriptome-prediction-models). A tutorial is available [here](https://github.com/hakyimlab/MetaXcan/wiki/Tutorial:-GTEx-v8-MASH-models-integration-with-a-Coronary-Artery-Disease-GWAS).

Acknowledging these models: If you use these models in your research, please cite:

    "Exploiting the GTEx resources to decipher the mechanisms at GWAS loci", Barbeira, Bonazzola, Gamazon, Liang, Park, et al. Genome Biol 22, 49 (2021)
    "A gene-based association method for mapping traits using reference transcriptome data", Gamazon et al, 2015, Nature Genetics
    "Exploring the phenotypic consequences of tissue specific gene expression variation inferred from GWAS summary statistics", Barbeira et al, 2018, Nature Communications

If you use S-MultiXcan, we ask you to cite:

    "Integrating predicted transcriptome from multiple tissues improves association detection", Barbeira et al, 2019, PLOS Genetics

## Elastic Net

Expression and splicing prediction models with LD references data are available in this Zenodo repository.

Files:

- [elastic_net_eqtl.tar](https://zenodo.org/record/3519321/files/elastic_net_eqtl.tar?download=1): PrediXcan's and S-PrediXcan's support on expression
- [elastic_net_sqtl.tar](https://zenodo.org/record/3519321/files/elastic_net_sqtl.tar?download=1): PrediXcan's and S-PrediXcan's on splicing
- [gtex_v8_expression_elastic_net_snp_smultixcan_covariance.txt.gz](https://zenodo.org/record/3519321/files/gtex_v8_expression_elastic_net_snp_smultixcan_covariance.txt.gz?download=1): S-MultiXcan expression's LD reference
- [gtex_v8_splicing_elastic_net_snp_smultixcan_covariance.txt.gz](https://zenodo.org/record/3519321/files/gtex_v8_splicing_elastic_net_snp_smultixcan_covariance.txt.gz?download=1): S-MultiXcan splicing's LD reference


Acknowledging these models : If you use these models in your research, we ask you to cite:

    "Exploiting the GTEx resources to decipher the mechanisms at GWAS loci", Barbeira, Bonazzola, Gamazon, Liang, Park, et al. Genome Biol 22, 49 (2021)
    "A gene-based association method for mapping traits using reference transcriptome data", Gamazon et al, 2015, Nature Genetics
    "Exploring the phenotypic consequences of tissue specific gene expression variation inferred from GWAS summary statistics", Barbeira et al, 2018, Nature Communications

If you use S-MultiXcan, we ask you to cite:

    "Integrating predicted transcriptome from multiple tissues improves association detection", Barbeira et al, 2019, PLOS Genetics

