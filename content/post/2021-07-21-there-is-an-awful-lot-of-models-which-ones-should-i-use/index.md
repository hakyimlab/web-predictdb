---
title: There is an awful lot of models! Which ones should I use?
author: PredictDB Team
date: '2021-07-21'
slug: there-is-an-awful-lot-of-models-which-ones-should-i-use
categories:
  - FAQ
tags: []
---
A1: GTEx v8 MASHR-based models are parsimonious and have been shown to yield more reliable set of putative causal variants. These are the best option. However, they require GWAS preprocessing on older GWAS as detailed [here](https://github.com/hakyimlab/MetaXcan/wiki/Best-practices-for-integrating-GWAS-and-GTEX-v8-transcriptome-prediction-models).

A2: GTEx v8 UTMOST models are a robust but with lower performance. These are based on HapMap snps and as such have a good overlap with most GWAS' snp sets.

A3: If your GWAS population is non-European, you might be interested in population-specific models.