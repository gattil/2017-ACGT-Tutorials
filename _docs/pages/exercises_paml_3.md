---
title: Exercise 7
permalink: /docs/exercises_paml_3/
redirect_from: /index.html

---
<p>We will use codeml program from PAML by Ziheng Yang. Use the command line mode for the tasks below. First, you need to understand which control file options to use. Next, try to reproduce the same analyses with codeml</code>.</p>

<p>You will need a dataset of homologous protein-coding DNA sequences (starting with the 1<sup>st</sup> codon position and ending with the 3<sup>rd</sup>). We will use data from published articles and will regenerate published results: </p>

<ul>
<li><p>Branch models: Yang, Z. 1998. Likelihood ratio tests for detecting positive selection and application to primate lysozyme evolution. Mol. Biol. Evol. 15:568-573.  <br>
Data 1: <a href="../../tutorial_data/tutorial02_paml/lysozymeSmall.nuc">lysozymeSmall.nuc</a>Tree 1: <a href="../../tutorial_data/tutorial02_paml/lysozymeSmall.trees">lysozymeSmall.trees</a> </p></li>
</ul>


---

**Branch-site models**.

Use the small lysozyme example to to fit branch-site models:
1. For each branch of the tree (one at a time) perform the LRT comparing model MA (ω is estimated) with model MA (fixed ω = 1).
2. How many LRTs are significant?
3. How many LRTs remain significant after the Bonferroni correction for multiple testing?
4. What can you tell about the evolution of your gene from the ML estimates obtained after the multiple LRT procedure?

> To get the Bonferroni corrected/adjusted p value, divide the original α-value by the number of analyses on the dependent variable. The researcher assigns a new alpha for the set of dependent variables (or analyses) that does not exceed some critical value: αcritical= 1 - (1 – αaltered)k, where k = the number of comparisons on the same dependent variable
