---
title: AttributeError 'NoneType' object has no attribute 'groups'
author: Festus
date: '2021-07-21'
slug: error-nonetype-object-has-no-attribute-groups
categories:
  - FAQ
tags:
  - MultiXcan
---

## Possible explanation
This error happens when using the Multixcan tool, it usually happens when the tool cant find files in the Metaxcan folder you provided. Thus halting the process of meta analyzing the results. The most probable cause of this error are;
  1. Providing a wrong path in the **--metaxcan_folder**
  2. Providing a wrong pattern in **--models_name_pattern** which results into zero files being captured
  3. Providing a wrong pattern in **--metaxcan_file_name_parse_pattern** which results into zero files being matched hence no file to analyze
  4. Not providing your pattern in quotes or placing the wild cards in wrong positions

## Possible solution
- Ensure your **--metaxcan_folder** path is correct
- Ensure you provide yor patterns correctly i.e in the example below the first filter selects all the files that start with **_PGZ-SCZ_Brain__** and the second filter extracts the trait from the name.
    >--metaxcan_filter "PGZ-SCZ_Brain_(.*).csv" \
     --metaxcan_file_name_parse_pattern "(.*)_Brain_(.*).csv"