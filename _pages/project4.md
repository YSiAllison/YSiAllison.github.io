
---
layout: archive
title: "Projects"
permalink: /projects/project4
author_profile: true
---

## Project 4: Genome Assembly from PacBio Sequencing Reads 

**Background**  Constructing genome assemblies is the first step to characterize pathogens on the molecular level and provide a foundation for developing targeted diagnostic and treatment plans related diseases. Although, there are genome assemblies available for the two pathogens of interest, they are from illumina short reads. A higher-quality genome assembly from long-read sequencing technology (for example PacBio) is in need for downstream research. One challenge is that the pathogens only grow on leaves in the lab due to their obligate nature. The samples for PacBio sequencing are naturally contaminated with leaves, bacteria, and fungi. The aim of this project is to pick out the pathogen reads from the PacBio sequencing results and generate a more accurate assembly with less contamination.
  



**Methods**  
Step 1: We extracted target sequences from the PacBio raw data based on reference genomes. 1) Apply DIAMOND to the PacBio raw reads to map the reference genome at the significant threshold for blastx at E-values $< 10^{-10}$. Extract Sequence reads matched to the reference genomes. 2) Apply kraken2 to the PacBio raw reads with default settings to map to the reference genome. Extract sequence reads classified as target pathogens according to the reference genome. 

Step 2: Apply Hifiasm genome assembly to the extracted sequence to generate a genome assembly for each isolation. Hifiasm constructs one of the best de novo genome assembly from PacBio Hifi sequencing reads. 

Step 3: Assess quality of genome assembly with Quality Assessment Tool for Genome Assemblies (QUAST) and Benchmarking Universal Single-Copy Orthologs (BUSCO) to check the genome assembly quality returned from different methods. QUAST takes assembled genomes in the form of contig or scaffold sequences as input and output the key statistics such as the total number of constructed contigs, N50 of contigs, and genome assembly size in base pairs. BUSCO constructs single-copy orthologs that are compared to all species within a particular taxonomic group. The output are about the completeness and redundancy of the gene in the genome assembly measured by the proportion of the orthologs that are complete, fragmented, or missing.  


**Results and Conclusion** Genome assembly constructed with sequence reads extracted from the Kranken2 methods with P.sojae asthe reference genome outperforms those extracted from Blast methods. The Hifiasm genome assembly tool constructed a reasonable genome assembly size of 90-130 MB out of sequence reads extracted from the Kranken2 data cleaning procedure. The genome assembly size is compatible to other published downy mildew genome assemblies from short reads. In addition, the higher gene completeness with lower duplication rate demonstrate that Kranken2 has better performance.


<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/Fig1.ga_gmiu.png" alt="projects" width="1000"/>









