---
title: 'Unexpected error: No objects to concatenate'
author: Festus
date: '2021-07-21'
slug: unexpected-error-no-objects-to-concatenate
categories:
  - FAQ
tags:
  - MultiXcan
---

## Possible explanation
This error raise when the multixcan tool does get gwas files which should be concatenated. The error is common when you are provoding multiple gwas files in a directory. The common mistake that brings the issue rises from;
  1. Providing wring path to the gwas_folder argument or a folder which does not contain gwas files
  2. A mismatch in the gwas file pattern provided in the command line argument
  3. Lack of quotes around the pattern provided

## Possible solution
- Ensure the correct path is provided to **--gwas_folder**
- Ensure the pattern you provide to **--gwas_file_pattern** is correct and in quotes, e.g
    > --gwas_file_pattern "(.*).txt" #selects all gwas files \
    --gwas_file_pattern "Brain_(.*).gz" #selects only gwas files with Brain prefix