---
title: Exercise 2 - Branch models
permalink: /docs/exercises_paml_1/
redirect_from: /index.html

---

<p>We will use codeml program from PAML by Ziheng Yang. Use the command line mode for the tasks below. First, you need to understand which control file options to use. Next, try to reproduce the same analyses with <code>codeml</code>.</p>
<p>You will need a dataset of homologous protein-coding DNA sequences (starting with the 1<sup>st</sup> codon position and ending with the 3<sup>rd</sup>). We will use data from published articles and will regenerate published results: </p>

<ul>
<li><p>Branch models: Yang, Z. 1998. Likelihood ratio tests for detecting positive selection and application to primate lysozyme evolution. Mol. Biol. Evol. 15:568-573.  <br>
Data 1: <a href="../../tutorial_data/tutorial02_paml/lysozymeSmall.nuc">lysozymeSmall.nuc</a>Tree 1: <a href="../../tutorial_data/tutorial02_paml/lysozymeSmall.trees">lysozymeSmall.trees</a> </p></li>
</ul>



---

<p><strong>Branch models</strong>.</p>

1. Use the small lysozyme example to fit **free-ratio model** for branches.
Are results consistent with those presented in the publication above?

2. Label the branch leading to colobine clade and fit the **2-ratio branch model** to your data.

3. In addition, **label the branch** leading to hominoids clade (use different label) and fit the **3-ratio branch model** to your data.

4. Based on LRTs, what model fits your data the best (among 2-ratio, 3-ratio and free-ratio models)?
What are the degrees of freedoms for each comparison?

5. What can you tell about the evolution of your gene from the ML estimates under this best model?</p></li>

---

Please refer to <code>PaML/codeml</code> documentation available [here](http://abacus.gene.ucl.ac.uk/software/pamlDOC.pdf)
