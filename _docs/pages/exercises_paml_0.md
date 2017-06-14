---
title: Exercise 1 - Simple codon model
permalink: /docs/exercises_paml_0/
redirect_from: /index.html

---
<p>We will use codeml program from PAML by Ziheng Yang. Use the command line mode for the tasks below. First, you need to understand which control file options to use. Next, try to reproduce the same analyses with codeml</code>.</p>

<p>You will need a dataset of homologous protein-coding DNA sequences (starting with the 1<sup>st</sup> codon position and ending with the 3<sup>rd</sup>). We will use data from published articles and will regenerate published results: </p>

<ul>
<li><p>Site-models: Yang, Z., R. Nielsen, N. Goldman, A.-M. K. Pedersen. 2000. Codon-substitution models for heterogeneous selection pressure at amino acid sites. Genetics 155: 431-449. <br>

Data 1: <a href="../../tutorial_data/tutorial02_paml/bglobin.nuc">bglobin.nuc</a> Tree 1:
<a href="../../tutorial_data/tutorial02_paml/bglobin.trees">bglobin.tree</a> <br>

Data 2: <a href="../../tutorial_data/tutorial02_paml/HIVenvSweden.nuc">HIVenvSweden.nuc</a>
Tree 2: <a href="../../tutorial_data/tutorial02_paml/HIVenvSweden.trees">HIVenvSweden.trees</a><br>

Data 3: <a href="../../tutorial_data/tutorial02_paml/adh.nuc">adh.nuc</a>
 Tree 3: <a href="../../tutorial_data/tutorial02_paml/adh.trees">adh.trees</a></p></li>
</ul>


---

<p><strong>The simple codon model with constant ω</strong>.</p>

1. Choose a dataset from the publication above and fit model **M0** - the most simple codon model with constant ω over time and sites. Run model M0 twice: first with branch lengths fixed to those in the tree file, and once with branch lengths estimated by ML.

2. Compare the optimised log-likelihoods for the two runs? In which case is it higher? Why?

3. Next, study the output file for the run with estimated branch lengths: Do you observe the codon frequency bias?

4. Study the statistics of nucleotide usage for different codon positions. Which position displays the most bias? Why?
What is the ML estimate of the transition-transversion ratio κ? What is the ML estimate of the ω-ratio? How do you interpret these ML estimates?

---

Please refer to PaML/codeml documentation available [here](http://abacus.gene.ucl.ac.uk/software/pamlDOC.pdf)
