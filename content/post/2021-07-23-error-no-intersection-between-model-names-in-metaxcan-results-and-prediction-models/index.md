---
title: Error No intersection between model names in MetaXcan Results and Prediction
  Models
author: Festus
date: '2021-07-23'
slug: error-no-intersection-between-model-names-in-metaxcan-results-and-prediction-models
categories:
  - FAQ
tags:
  - MultiXcan
---

## Possibe explanation
This error happen when the strings captured from the metaxcan results and models don't coincide

A good example is when the metaxcan results' captured names looked like `Aorta` while the models' captured names looked like `Artery_Aorta`, this will result into this error


## Possible solutions
- To make sure that this error doesn't occur when SMulTiXcan is checking the model names for the MetaXcan Results, make sure you save the results from running MetaXcan as the tissue name only-exactly the way it's used in .db files. 
- The strings captured from metaxcan results and models must coincide
- The commands to check out for;
  > **--models_name_filter**: allows to select only some of the models in a folder (i.e. only adipose from all GTEx tissues). If you  have only those two models in the models folder, you don't need this argument \
**--models_name_pattern**: allows to extract a name to be matched to metaxcan results \
**--metaxcan_filter**: select specific metaxcan results from a folder \
**--metaxcan_file_name_parser_pattern**: extract tissue names from file names