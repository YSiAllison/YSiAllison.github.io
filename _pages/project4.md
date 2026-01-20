---
layout: archive
title: "Projects"
permalink: /projects/project4
author_profile: true
---

## Project 4: Genome Assembly from PacBio Sequencing Reads 

**Background**  Constructing genome assemblies is the first step to characterize pathogens on the molecular level and provide a foundation for developing targeted diagnostic and treatment plans related diseases. Long-read sequencing technology (for example PacBio) may generate a higher-quality genome assembly for downstream research. One challenge is that the pathogens of interest only grow on leaves in the lab due to their obligate nature. The samples for PacBio sequencing are naturally contaminated with leaves, bacteria, and fungi. The aim of this project is to pick out the pathogen reads from the PacBio sequencing results and generate a more accurate assembly with less contamination.
  



**Methods**  
Step 1: Extracted target sequences from the PacBio raw data based on reference genomes. Apply DIAMOND blastx (at E-values < 10^{-10}) and kraken2 to the PacBio raw reads with default settings to map to the reference genome. 

Step 2: Apply Hifiasm genome assembly to the extracted sequence to generate a genome assembly 

Step 3: Assess quality of genome assembly with Quality Assessment Tool for Genome Assemblies (QUAST, evaluates total number of constructed contigs, N50 of contigs, and genome assembly size) and Benchmarking Universal Single-Copy Orthologs (BUSCO, evaluates the completeness and redundancy of the gene) to check the genome assembly quality returned from different methods.   


**Results and Conclusion** Genome assembly constructed with sequence reads extracted from the Kranken2 methods with P.s as the reference genome outperforms those extracted from Blast methods. The Hifiasm genome assembly tool constructed a reasonable genome assembly size of 90-130 MB out of sequence reads extracted from the Kranken2 data cleaning procedure. The genome assembly size is compatible to other published downy mildew genome assemblies from short reads. In addition, the higher gene completeness with lower duplication rate demonstrate that Kranken2 has better performance.


<img src="/files/DMGenomeAssembly.png" alt="projects" width="1000"/>









