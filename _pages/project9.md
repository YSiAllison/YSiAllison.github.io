---
layout: archive
title: "Projects"
permalink: /projects/project6
author_profile: true
---

## Project 4: Naturally-inspired algorithm for multiple sequence alignment ([Report](https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DCantdocs.pdf); [Presentation](https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DCAntcolony.pdf))


We have implemented the algorithm described in “An efficient algorithm for multiple sequence
alignment based on ant colony optimization and divide-and-conquer method” by Wei Liu, Ling Chen, and
Juan Chen (2007). This algorithm consists of three parts: Divide and Conquer, Ant Colony Optimization,
and Assembly.
In the Divide and Conquer stage, a genetic algorithm is used to find the best way to divide the
DNA sequences into more manageable chunks. The overall complexity of Divide and Conquer is 𝑂(𝑁2 ∗ 𝐿𝑒𝑛 ∗ 𝑇 ∗ 𝐶 ∗ 𝑙𝑜𝑔⁡(𝑙𝑒𝑛)), in
which N is the number of sequences, T is the number of mutation and crossover operations, C is the
number of new generations of the population, Len is the length of the longest sequence, 𝑙𝑜𝑔⁡(𝑙𝑒𝑛) is the
approximate number of subsets.
The next stage then aligns each of these subsequences using an Ant Colony Optimization heuristic.
In this step, we loop through every nucleotide from every sequence, with an “ant” forming a path from
each of these nucleotides to its best match in every other sequence. As each path is formed, the ant
“pheromone” is updated, eventually leading more ants to choose the more popular (and hopefully best)
paths. After every nucleotide in a sequence has a path, an alignment of all the sequences is formed from
the paths, and its sum of pairs score is calculated. This is repeated for every sequence, keeping track of
the best alignment. The computation complexity of the Ant Colony
Optimization is 𝑂(𝑁2 ∗ 𝐿𝑒𝑛 ∗ 𝐶𝑦𝑐𝑙𝑒⁡ ∗ ⁡𝑙𝑜𝑔(𝐿𝑒𝑛)), in which N is the number of sequences, Cycle is the
number of iterations “ants” travel, and Len is the length of the longest sequence.
Finally, after each set of subsequences is aligned, they are reassembled to form one overall
alignment. This is done by simply concatenating the aligned subsequences together. The time complexity
is 𝑂(𝑁 ∗ 𝑙𝑜𝑔(𝑙𝑒𝑛)), where again N is the number of sequences and len is the length of the longest
sequence.
Both the runtime and memory usage increases quadratically as the
number of DNA sequences increased and both appeares to have an nlogn relationshipas the length of the DNA sequences increases. The accuracy of the Ant Colony and Divide and Conquer algorithm is compatible with Rose for short sequences and for a small number of sequences. However,
when the length of sequence is large or the number of sequences increases, the accuracy decreases. 
<img src="https://github.com/YSiAllison/YSiAllison.github.io/blob/master/files/DCant.png" alt="projects" width="1000"/>










