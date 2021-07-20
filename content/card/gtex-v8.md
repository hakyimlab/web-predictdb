# GTEx v8 models on eQTL and sQTL

We have produced different families of prediction models for sQTL and eQTL, using several prediction strategies, on GTEx v8 release data.

We recommend MASHR-based models below. Elastic Net-based are a safe, robust alternative with decreased power.
MASHR-based models

Expression and splicing prediction models with LD reference data are available in this Zenodo repository.

Files:

    mashr_eqtl.tar: PrediXcan's and S-PrediXcan's support on expression
    mashr_sqtl.tar: PrediXcan's and S-PrediXcan's support on splicing
    gtex_v8_expression_mashr_snp_smultixcan_covariance.txt.gz: S-MultiXcan expression's LD reference
    gtex_v8_splicing_mashr_snp_smultixcan_covariance.txt.gz: S-MultiXcan splicing's LD reference


Warning: these models are based on fine-mapped variants that may occasionally be absent in a tipical GWAS, and frequently absent in older GWAS. We have tools to address this, presented here. A tutorial is available here.

Acknowledging these models: If you use these models in your research, please cite:

    "Widespread dose-dependent effects of RNA expression and splicing on complex diseases and traits", Barbeira et al, 2019, preprint
    "A gene-based association method for mapping traits using reference transcriptome data", Gamazon et al, 2015, Nature Genetics
    "Exploring the phenotypic consequences of tissue specific gene expression variation inferred from GWAS summary statistics", Barbeira et al, 2018, Nature Communications

If you use S-MultiXcan, we ask you to cite:

    "Integrating predicted transcriptome from multiple tissues improves association detection", Barbeira et al, 2019, PLOS Genetics

