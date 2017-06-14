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


<blockquote>
<a href="http://www.biostathandbook.com/multiplecomparisons.html">About Bonferroni Correction</a>
<li>Any time you reject a null hypothesis because a P value is less than your critical value, it's possible that you're wrong; the null hypothesis might really be true, and your significant result might be due to chance.</li>
<li>Instead of setting the critical P level for significance, or alpha, to a certain value (i.e 0.05), you use a lower critical value. If the null hypothesis is true for all of the tests, the probability of getting one result that is significant at this new, lower critical value is 0.05.</li>
<li>The most common way to correct for multiple testing is with the Bonferroni correction. You find the critical value (alpha) for an individual test by dividing the P-value (i.e. 0.05) by the number of tests. Thus if you are doing 100 statistical tests, the critical value for an individual test would be 0.05/100=0.0005, and you would only consider individual tests with P<0.0005 to be significant.</li>
</blockquote>
