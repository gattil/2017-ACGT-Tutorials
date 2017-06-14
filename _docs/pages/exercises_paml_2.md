---
title: Exercise 3 - Site models
permalink: /docs/exercises_paml_2/
redirect_from: /index.html

---
<p>We will use codeml program from PAML by Ziheng Yang. Use the command line mode for the tasks below. First, you need to understand which control file options to use. Next, try to reproduce the same analyses with <code>codeml</code>.</p>
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

<p><strong>Site-models</strong>.</p>


1. Choose a dataset from publication 1 and fit the following site models to your data:

2. M1, M2, M3, M7, M8a, and M8 (always estimate branch lengths by ML).
Note 1:Model M0 was already fitted in exercise 1 (make sure you have the output file).  
Note 2: M8a is model M8 with ω for the discrete category fixed to 1.
Which models are nested?

3. Perform likelihood ratio tests (LRTs) of nested hypotheses.
How many degrees of freedom do you use each time to test for significance of the LRT statistic?
Do your tests suggest positive selection?

4. Interpret the ML estimates relevant to selective pressure.

5. If LRTs suggest positive selection, which sites are inferred by the Bayesian approach to be under positive selection (models M2 and M8)?

6. Do NEB and BEB agree on the sites inferred?

7. Compare results from the LRT comparing M7 vs M8 and the LRT comparing M8a vs M8. Are they both significant (or both non-significant)? If they are both significant, does the Bayesian approach predict the same sites?

---

Please refer to <code>PaML/codeml</code> documentation available [here](http://abacus.gene.ucl.ac.uk/software/pamlDOC.pdf)
