---
title: 'Unexpected error: nothing to repeat at position 0"'
author: Festus
date: '2021-07-21'
slug: info-unexpected-error-nothing-to-repeat-at-position-0
categories:
  - FAQ
tags:
  - MultiXcan
---

## Possible explanation
This error happens when the data bases cannot be loaded into the tool and the main cause might be;
  1. Not providing the correct path to the models folder 
  2. providing the wrong pattern to match the models in the directory

## Possible solution
- Ensure you provide the correct path to **--models_folder** argument
- Ensure the patterns are provided correctly. In the example below only models which start with **_en\_Brain\__** will be selected. 
    > --models_name_pattern "en_(.*).db" \
    --models_name_filter "en_Brain_(.*).db"
    
