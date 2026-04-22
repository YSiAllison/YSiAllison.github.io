---
layout: archive
title: "Projects"
permalink: /projects/project4
author_profile: true
---

## Project 4: Causal DAG learning framework ([Presentation](https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DAG_VAE.pptx); [Video](https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DAG_VAE.mp4)

**Summary** Causality is an important concept for health sciences. Causality is particularly vital for finding adverse drug events, risk factors, or important biomarkers for disease using high-dimension health data. However, under a general causal graph, the exposure may not only have a direct effect on the outcome, but also an indirect effect regulated by a set of mediators. Thus, to estimate this complicate causal network, structure learning algorithms of the directed acyclic graph (DAG) are widely used. Many popular DAG learning algorithms therefore have been applied to better solve this problem both computationally and mathematically. Specifically, for this project, we would like to try a new method--- Analysis of Causal Effects (ANOCE), under the linear structure equation model (LSEM), which is an extension of classical variational auto-encoder (VAE) framework, but with a novel identification constraint that specifies the topological order of the exposure and the outcome in the DAG. 


<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DAG.png" alt="projects" width="1000"/>
