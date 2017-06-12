---
title: Exercise 4 - Branch support
permalink: /docs/exercises_phyml_3/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
In this tutorial you will be guided in using PhyML and its extension, CodonPhyML, to solve common phylogenetic problems. For some of the following exercises there might be more than one single solution.

---

##### **Goal: Computing the branch support on the inferred phylogenetic tree.**

In this exercise we are going to compute the branch support using 2 different approaches: non-parametric ML bootstrap and SH-aLRT (note: the running time is much shorter for SH-aLRT).

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

Run PhyML with the using the branch support method: **Bootstrap**

##### Second Run

Run PhyML with the using the branch support method: **SH-aLRT**


---


<div class="panel panel-default">
    <div class="panel-heading">Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Compare supports inferred by non-parametric ML bootstrap to those obtained using SH-aLRT method</li>
      <li>Are the results compatible?</li>
    </ol>
    </div>
</div>

---

This exercise was prepared by *Maria Anisimova*
