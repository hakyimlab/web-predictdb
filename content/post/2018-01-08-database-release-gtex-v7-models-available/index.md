---
title: 'Database release: GTEx V7 Models available'
author: PredictDB Team
date: '2018-01-08'
slug: database-release-gtex-v7-models-available
categories:
  - News
tags: []
---
We are releasing prediction models trained on GTEx Version 7 data. Download from[here](http://predictdb.org/). We have updated our processing pipeline, and restricted to individuals of European ancestry to obtain more reliable LD data. This reduces false positive associations in the Summary Version of PrediXcan. Because of this choice, the gain in sample size relative to V6p is modest (ranging from -18 to 89), with whole blood, LCLs and fibroblasts experiencing reduced sample size. We developed a new criteria to assess model performance. We have also decided to include prediction models for both pseudogenes and lincRNAs. For your convenience, we also include a SNP annotation file with information on the SNPs used to train the models.

While preparing GTEx V7 prediction models, we identified a few issues in the way prediction performance was estimated in the previous release (2016-09-08 release). In aggregate, these caused the prediction model performance to be overestimated. Reassuringly, predicted expression levels and the downstream associations with phenotypes remain mostly unchanged, even though prediction weights vary slightly. However, some gene/tissue pairs are no longer considered reliable.

Detailed description of the pipeline update and the effect in prediction models performance and downstream S-PrediXcan association can be found[here](http://hakyimlab.org/post/2017/v7-v6p-analysis/).

We would appreciate comments to our mailing list predixcanmetaxcan@googlegroups.com