---
title: Exercise 1 - Parameter estimation
permalink: /docs/exercises_phyml_0/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
In this tutorial you will be guided in using PhyML and its extension, CodonPhyML, to solve common phylogenetic problems. For some of the following exercises there might be more than one single solution.

---

##### **Goal: Observing the effect of parameter estimation from data on the inferred tree topology.**

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
            <li><a href="../../tutorial_data/tutorial01_phyml/primates-nt.phy">Download</a></li>
          </ul>
        </div>
    </div>
</div>



##### First Run


Set the model to HKY+Gamma, estimating the transition/transversion ratio and the alpha parameter of the Gamma distribution by maximum likelihood (ML), nucleotide frequencies are estimated by ML.


#####  Second Run

Set the model to HKY+Gamma, estimating the transition/transversion ratio and the alpha parameter of the Gamma distribution by maximum likelihood (ML), nucleotide frequencies are estimated empirically from the data



---

<div class="panel panel-default">
    <div class="panel-heading">Questions/Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Do you see much difference in the tree?</li>
      <li>In the likelihood value (stat file)?</li>
      <li>Which option is best and why do you think so?</li>
    </ol>
    </div>
</div>

---

<p>
<span class="label label-default">phylogenies</span>
<span class="label label-default">tree-estimation</span>
<span class="label label-default">maximum-likelihood</span>
<span class="label label-default">parameter-estimation</span>
</p>

---

This exercise was prepared by *Maria Anisimova*
