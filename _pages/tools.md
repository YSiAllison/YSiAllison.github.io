---
layout: archive
title: "Tools"
permalink: /tools/
author_profile: true
redirect_from:
  - /resume
---

### CNVreg R package ([CRAN](https://cran.r-project.org/web/packages/CNVreg/index.html); [Github](https://github.com/Oceanyq/CNVreg))

CNVreg: CNV-Profile Regression for Copy Number Variants Association Analysis with Penalized Regression


Performs copy number variants association analysis with Lasso and Weighted Fusion penalized regression. Creates a "CNV profile curve" to represent an individual’s CNV events across a genomic region so to capture variations in CNV length and dosage. When evaluating association, the CNV profile curve is directly used as a predictor in the regression model, avoiding the need to predefine CNV loci. 

CNV profile regression estimates CNV effects at each genome position, making the results comparable across different studies. The penalization encourages sparsity in variable selection with a Lasso penalty and encourages effect smoothness between consecutive CNV events with a weighted fusion penalty, where the weight controls the level of smoothing between adjacent CNVs. 

For more details, see [Si (2024)](https://www.biorxiv.org/content/10.1101/2024.11.23.624994v1).
