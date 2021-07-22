---
title: 'Why are there fewer available genes/introns in the prediction models than
  in the GTEx dataset?'
author: PredictDB Team
date: '2021-07-21'
slug: why-are-there-fewer-available-genes-introns-in-the-prediction-models-than-in-the-gtex-dataset
categories:
  - FAQ
tags: []
---
The prediction model databases only contain models that pass a stringent criteria (each family of models has its own criteria, e.g. MASHR models require at least one snp with high posterior probability of being an eQTL). Our model training algorithms are complex and conservative. Sometimes, a good enough signal can't be captured from a gene's expression profile, even if it has an eQTL. Conversely, sometimes the algorithms converge for genes with complex profiles where no eQTL could be found. On other occasions, the algorithm doesn't converge.
