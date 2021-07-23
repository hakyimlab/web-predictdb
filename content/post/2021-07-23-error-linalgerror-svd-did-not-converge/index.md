---
title: Error for region (...) LinAlgError('SVD did not converge')
author: PredictDB Team
date: '2021-07-23'
slug: error-linalgerror-svd-did-not-converge
categories:
  - FAQ
tags:
  - MetaXcan
---

## Possible explanation
- This can happen when there are inf or nan values in the data
- This might also happen due to resources issues - a thread corruption or memory corruption 
- A comprehensive explanation;
  >One step of the summary imputation, the computation of snp covariance matrix inverse, is performed via singular value decomposition (SVD).
Numerical solutions to the SVD algorithm are not guaranteed to converge, and fail on some regions.
When this happens, unmeasured zscores will not be present in the imputation output, thus they are not the ones with zscore=NA.
This is undesirable but expected, given the nature of the data.\
Now, the case with zscore=NA is trickier. It corresponds to regions where the SVD algorithm did converge, but the covariance inverse is filled with NaN (not-a-number) values.
The warnings are emitted when pvalues are computed from an array of zscores that contain NaN values; again, this is undesirable but expected.
I found this a bit dependent on the underlying numerical libraries sitting beneath python's numpy (BLAS and LAPACK). \
There are some improvements to be done, as sometimes only a portion of the matrix is NaN and working on the well-defined subset of variants should be viable (alas, we didn't have time to implement this). \
The post-process script is a mere tidy-up step, gathering entries from the original, unimputed snps from the GWAS and imputed snps. \
The summary is that the behavior you observe is  normal; our implementation will try to compute as many results as possible, but some regions have complicated snp covariance (LD) and the algorithm doesn't behave. ~ Alvaro

## Possible solution
- Remove nan or inf values from your dataset
- Running in an HPC with twice the memory of the original job