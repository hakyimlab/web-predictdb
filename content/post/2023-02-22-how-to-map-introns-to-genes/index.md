---
title: How to map introns to genes
author: Haky Im
date: '2023-02-22'
slug: how-to-map-introns-to-genes
categories:
  - FAQ
tags: []
---

- Q: We've successfully run the S-PrediXcan and S-MultiXcan methods on our GWAS data using the MASHR sQTL models and have the outputs. My question is, how do I interpret and/or follow up on the results? I see a handful of intron IDs that look significant and I find the relevant single tissue results for those intron IDs. 


Find the mapping from intron ids to gene ids in this link
https://uchicago.box.com/s/xy71r0su6refrfggivrwc7kpvsxysmmn


- Q: How should I interpret the z-score? Does a negative z-score for an intron imply that a decrease in the excision of that intron leads to an increase in the GWAS trait? Yes


- Q: How can I recover the SNPs that are predicted to lead to a decrease in the excision of that intron?

Use this post to query the database file where the prediction weights are included https://predictdb.org/post/2021/07/21/how-do-i-query-the-prediction-model-db/
