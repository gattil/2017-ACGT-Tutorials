---
title: Introduction to PaML Exercises
permalink: /docs/exercises_paml_intro/
redirect_from: /index.html

---
<h2 id="tutorial-2-evaluating-selection-pressure-with-codon-models"><strong>Tutorial 2</strong>: Evaluating selection pressure with codon models</h2>

<p>We will use codeml program from PAML by Ziheng Yang. Use the command line mode for the tasks below. First, you need to understand which control file options to use. Next, try to reproduce the same analyses with codeml or PAML-X (the GUI for PAML).  <br>
You will need a dataset of homologous protein-coding DNA sequences (starting with the 1<sup>st</sup> codon position and ending with the 3<sup>rd</sup>). We will use data from published articles and will regenerate published results: </p>

<ol>
<li><p>Site-models: Yang, Z., R. Nielsen, N. Goldman, A.-M. K. Pedersen. 2000. Codon-substitution models for heterogeneous selection pressure at amino acid sites. Genetics 155: 431-449. <br>
Data 1: <code>bglobin.nuc</code> Tree 2: <code>bglobin.tree</code> <br>
Data 2: <code>HIVenvSweden.nuc</code> Tree 3: <code>HIVenvSweden.tree</code> <br>
Data 3: <code>adh.nuc</code> Tree 1: <code>adh.tree</code></p></li>

<li><p>Branch models: Yang, Z. 1998. Likelihood ratio tests for detecting positive selection and application to primate lysozyme evolution. Mol. Biol. Evol. 15:568-573.  <br>
Data 1: <code>lysozymeSmall.nuc</code> Tree 1: <code>lysozymeSmall.trees</code></p></li>

<li><p>Branch-site models: Zhang, J., R. Nielsen, and Z. Yang. 2005. Evaluation of an improved branch-site likelihood method for detecting positive selection at the molecular level. Molecular Biology and Evolution 22:2472-2479. <br>
We will use the same data as in 2 (also analysed in the paper).</p></li>
</ol>
