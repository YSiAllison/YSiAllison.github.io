---
layout: archive
title: "Projects"
permalink: /projects/project1
author_profile: true
---

## Project 1: Phylogeny-guided Microbiome OTU-specific Association Test ([Paper](https://microbiomejournal.biomedcentral.com/articles/10.1186/s40168-022-01266-3); [Poster](http://hczdavid.github.io/files/JSM_post.pdf))

**Background**   Copy number variants (CNVs) are DNA gains or losses involving $>50$ base-pairs. While whole-genome sequencing (WGS) enables comprehensive CNV detection, CNV association analysis of WGS data faces key challenges: Because CNVs rarely align to common breakpoints, different locus definitions can yield substantially different CNV loci. Such inconsistencies hinder result interpretability and cross-study comparison. Moreover, most existing association methods adapted from SNP analysis focus on CNV dosage and ignore length, despite evidence that CNV length contributes to disease risk.
**Methods** We propose CNV profile regression (CNVreg), which represents individuals’ CNV data using CNV profile curves and evaluates association by regressing traits directly on these curves. This approach naturally incorporates dosage and length effects, and produces effect estimates interpretable and comparable across studies. CNVreg uses Lasso penalty to select trait-associated CNVs and weighted fusion penalty to encourage similar effects of adjacent CNVs. 
**Results and Conclusion** Simulations show that CNVreg more effectively identifies causal CNVs and yields more precise effect size estimates. Using CNVreg for WGS data analyses from the Alzheimer’s Disease Sequencing Project identifies additional disease-relevant CNVs associated with Alzheimer's Disease. An R package \href{https://cran.r-project.org/web/packages/CNVreg/index.html}{``CNVreg''} is available on CRAN. 


<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/Fig1.ga_gmiu.png" alt="projects" width="1000"/>









