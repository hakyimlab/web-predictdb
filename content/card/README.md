---
title: README
style: 'background: #f7f9fb;'
weight: 3
---

# README

## Prediction weights and covariance files
The prediction weigths are saved in SQLite format, `*.db`, which can be easily queried using sqlit, R, python, etc. [See example in R here](https://lab-notes.hakyimlab.org/post/2021/04/27/querying-predictdb-sqlite-databases/). The summary statistics based methods need covariances (LD reference) between predictor SNPs and are saved in gzipped text files `*.txt.gz`. S-PrediXcan is meant to use the single-tissue LD reference files ("covariances") appropriate to each model. S-MultiXcan uses single-tissue prediction models and a cross-tissue LD reference.

## Search
The **Search** option in the menu may be the fastest way to find the right models or answers to your questions. If you still have more questions, join our mailing list and post your questions there. You can also navigate through the menu options.

## Mailing List

Please join our [Google Group](https://groups.google.com/forum/#!forum/predixcanmetaxcan) for general discussion, notification of future changes to our tools, feature requests, etc.

## Disclaimer

The models are provided "as is", with the hope that they may be of use, without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. in no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the models or the use or other dealings in the models.

## References
1. **PrediXcan**: Gamazon ER†, Wheeler HE†, Shah KP†, Mozaffari SV, Aquino-Michaels K, Carroll RJ, Eyler AE, Denny JC, Nicolae DL, Cox NJ, Im HK. (2015) A gene-based association method for mapping traits using reference transcriptome data. Nat Genet. doi:10.1038/ng.3367 [url](http://www.nature.com/ng/journal/v47/n9/full/ng.3367.html)
2. **S-PrediXcan**: Barbeira, Alvaro N., Scott P. Dickinson, Rodrigo Bonazzola, Jiamao Zheng, Heather E. Wheeler, Jason M. Torres, Eric S. Torstenson, Kaanan P. Shah, Tzintzuni Garcia, Todd L. Edwards, Eli A. Stahl, Laura M. Huckins, Dan L. Nicolae, Nancy J. Cox, and Hae Kyung Im. 2018. “Exploring the Phenotypic Consequences of Tissue Specific Gene Expression Variation Inferred from GWAS Summary Statistics.” Nature Communications 9 (1). Nature Publishing Group: 1–20.
3. **Genetic Architecture of Expression traits**: Heather E Wheeler, Kaanan P Shah, Jonathon Brenner, Tzintzuni Garcia, Keston Aquino-Michaels, GTEx Consortium, Nancy J Cox, Dan L Nicolae, Hae Kyung Im. (2016) Survey of the Heritability and Sparsity of Gene Expression Traits Across Human Tissues. [url](http://biorxiv.org/content/early/2016/03/15/043653.1)
4. **MultiXcan**: Barbeira, Alvaro N., Milton Pividori, Jiamao Zheng, Heather E. Wheeler, Dan L. Nicolae, and Hae Kyung Im. 2019. “Integrating Predicted Transcriptome from Multiple Tissues Improves Association Detection.” PLoS Genetics 15 (1). Public Library of Science: e1007889–20.
5. **GTEx V8 models**: Barbeira, Alvaro N., Rodrigo Bonazzola, Eric R. Gamazon, Yanyu Liang, Yoson Park, ..., and Hae Kyung Im. 2021. “Exploiting the GTEx Resources to Decipher the Mechanisms at GWAS Loci.” Genome Biology 22 (1): 49.
6. **GTEx Consortium Main Paper**: 2020. “The GTEx Consortium Atlas of Genetic Regulatory Effects across Human Tissues.” Science 369 (6509): 1318–30.
7. **Fine-mapping-based prediction more reliable**: Barbeira, Alvaro N., Owen J. Melia, Yanyu Liang, Rodrigo Bonazzola, Gao Wang, Heather E. Wheeler, François Aguet, Kristin G. Ardlie, Xiaoquan Wen, and Hae K. Im. 2020. “Fine-Mapping and QTL Tissue-Sharing Information Improves the Reliability of Causal Gene Identification.” Genetic Epidemiology n/a (n/a). John Wiley & Sons, Ltd. doi:10.1002/gepi.22346.

## License

This work is licensed under [the Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0).
