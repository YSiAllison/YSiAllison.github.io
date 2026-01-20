---
layout: archive
title: "Projects"
permalink: /projects/project5
author_profile: true
---

## Project 1: Terrain Identification from wearable device signals using Neural Networks [Report]()

**Background**   Copy number variants (CNVs) are DNA gains or losses involving $>50$ base-pairs. While whole-genome sequencing (WGS) enables comprehensive CNV detection, CNV association analysis of WGS data faces key challenges: Because CNVs rarely align to common breakpoints, different locus definitions can yield substantially different CNV loci. Such inconsistencies hinder result interpretability and cross-study comparison. Moreover, most existing association methods adapted from SNP analysis focus on CNV dosage and ignore length, despite evidence that CNV length contributes to disease risk.


**Methods** In the prediction for terrains, we composed four different
neural network architectures to select the best model based on
accuracy and averaged F1-score in the validation set. The mod-
els we used were: a Fully-connected Neural Network(FNN),
a Convolutional Neural Network (CNN), a Long Short-Term
Memory (LSTM) Neural Network, and a Transformer Neural
Network(TransNN), to predict a categorical distribution over
the target classes.

**Results and Conclusion** Simulations show that CNVreg more effectively identifies causal CNVs and yields more precise effect size estimates. Using CNVreg for WGS data analyses from the Alzheimer’s Disease Sequencing Project identifies additional disease-relevant CNVs associated with Alzheimer's Disease. An R package [CNVreg](https://cran.r-project.org/web/packages/CNVreg/index.html) is available on CRAN. 


<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/Fig1.ga_gmiu.png" alt="projects" width="1000"/>









