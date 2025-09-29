[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1722394.svg)](https://doi.org/10.5281/zenodo.1722394)

# TCGA–COAD methylation pipeline (Ekum 2025)

Reproducible TCGA–COAD Illumina 450K DNA-methylation analysis:
Exploratory data analysis → per-CpG limma eBayes testing →
surrogate-variable adjustment (SVA) → region-level DMR detection with
`bumphunter` → GAM visualisation → machine-learning benchmark
(logistic regression, Random Forest, XGBoost and neural networks).

## How to run

1. Install R (≥4.3) and required packages:
   `TCGAbiolinks, limma, bumphunter, mgcv, ggplot2, ranger, xgboost, nnet, pROC`.
2. From an R session:
   ```r
   source("scripts/tcga_coad_pipeline.R")

## Citation
If you use this pipeline, please cite:

Matthew Iwada Ekum (2025). *TCGA-COAD methylation pipeline.*  
Zenodo. [https://doi.org/10.5281/zenodo.1722394](https://doi.org/10.5281/zenodo.1722394)
