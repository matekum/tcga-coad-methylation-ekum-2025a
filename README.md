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
