---
title: Solution 1 - Parameter estimation
permalink: /docs/solutions_phyml_0/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
###### **Observing the effect of parameter estimation from data on the inferred tree topology.**

<br>

#### Goals

In this exercise you are asked to run PhyML twice in order to compare the effect of estimating nucleotide frequencies from the used dataset vs. optimising them with a maximum likelihood (ML) approach.

---


<div class="panel panel-primary">
    <div class="panel-heading">Datasets</div>
    <div class="panel-body">
        Dataset file: <div class="btn-group">
          <a href="#" class="btn btn-default">primates-nt.phy</a>
          <a href="#" class="btn btn-default dropdown-toggle" data-toggle="dropdown"><span class="caret"></span></a>
          <ul class="dropdown-menu">
            <li><a href="#">View</a></li>
            <li><a href="#">Download</a></li>
          </ul>
        </div>
    </div>
</div>

---

##### First Run

<ul>
<li>Nucleotide substitution model = <em>HKY85 + Gamma</em></li>
<li>Estimating <em>transition/transversion</em> ratio ( <script type="math/tex" id="MathJax-Element-1">\kappa</script> parameter of HKY85 model)</li>
<li>Estimating <em>alpha</em> parameter (remember <script type="math/tex" id="MathJax-Element-2">\alpha = \beta</script>  for gamma distributions used in phylogenetics)</li>
<li>Estimating <em>nucleotide frequencies</em> <strong>with ML</strong></li>
</ul>

<p>Here is the list of the parameters to change:</p>

<p>From 2<sup>nd</sup> menu</p>

<pre><code>[M] ................. Model of nucleotide substitution  HKY85
[F] ................. Optimise equilibrium frequencies  yes
[T] .................... Ts/tv ratio (fixed/estimated)  estimated
[C] ........... Number of substitution rate categories  4
[G] ............. Gamma distributed rates across sites  yes
[A] ... Gamma distribution parameter (fixed/estimated)  estimated
</code></pre>

---

##### Second Run

<ul>
<li>Nucleotide substitution model = <em>HKY85 + Gamma</em></li>
<li>Estimating <em>transition/transversion</em> ratio ( <script type="math/tex" id="MathJax-Element-3">\kappa</script> parameter of HKY85 model)</li>
<li>Estimating <em>alpha</em> parameter (remember <script type="math/tex" id="MathJax-Element-4">\alpha = \beta</script> for gamma distributions used in phylogenetics)</li>
<li>Estimating <em>nucleotide frequencies</em> <strong>empirically</strong> from the data</li>
</ul>

<p>Here is the list of the parameters to change:</p>

<p>From 2<sup>nd</sup> menu</p>

<pre><code>[M] ................. Model of nucleotide substitution  HKY85
[F] ................. Optimise equilibrium frequencies  no
[T] .................... Ts/tv ratio (fixed/estimated)  estimated
[C] ........... Number of substitution rate categories  4
[G] ............. Gamma distributed rates across sites  yes
[A] ... Gamma distribution parameter (fixed/estimated)  estimated
</code></pre>

---

<h5 id="questions">Questions</h5>

<p><strong>1. Do you see much difference in the tree?</strong></p>

<p>The topology does not change, however we can observe a change in the computed branch lengths.</p>

<table>
<thead>
<tr>
  <th>Nt-frequencies optimised</th>
  <th>Nt-frequencies estimated</th>
</tr>
</thead>
<tbody><tr>
  <td><img src="../../img/ex1_tree1.png" alt="" title=""></td>
  <td><img src="../../img/ex1_tree2.png" alt="" title=""></td>
</tr>
</tbody></table>


<p><strong>2. In the likelihood value (stat file)?</strong></p>

<p>The likelihood value of the tree inferred using the nucleotide frequencies estimated empirically from the dataset is lower than the likelihood value of the tree inferred using the nucleotide frequencies estimated via ML. This is due to dataset dimensions (the number of the sequences used).</p>

<pre><code>    run 1: -6172.58045
    run 2: -6173.49655
</code></pre>

<p><strong>3. Which option is best and why do you think so?</strong></p>

<p>The best option in this case is to use the ML approach since the ML optimisation technique provides better estimates for the nucleotide frequencies, which, in turn, affect the likelihood of the inferred tree. This is due to the nucleotide frequencies which are used in the calculation of the likelihood of each site of the alignment (<script type="math/tex" id="MathJax-Element-5">\pi Q = 0</script>, where <script type="math/tex" id="MathJax-Element-6">\pi</script> is the vector of the nucleotide frequencies and <script type="math/tex" id="MathJax-Element-7">Q</script> the rate matrix).</p>


---

<p>
<span class="label label-default">phylogenies</span>
<span class="label label-default">tree-estimation</span>
<span class="label label-default">maximum-likelihood</span>
<span class="label label-default">parameter-estimation</span>
</p>
