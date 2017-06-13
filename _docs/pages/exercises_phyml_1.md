---
title: Exercise 2 - Tree topologies
permalink: /docs/exercises_phyml_1/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
In this tutorial you will be guided in using PhyML and its extension, CodonPhyML, to solve common phylogenetic problems. For some of the following exercises there might be more than one single solution.

---

##### **Goal: Observing the effect of tree search routines on the initial inferred tree topology.**

In this exercise you are asked to optimise the tree topology on the substitution parameters obtained using ML performing a tree search (i.e. NNI, SPR, TBR) on the initial tree topology.

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

---

By default PhyML builds a BioNJ tree and uses this tree as a starting tree. Run PhyML without the tree-search, so that all model parameters are optimized on the BioNJ tree.

---

<div class="panel panel-default">
    <div class="panel-heading">Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Compare the ML and the BioNJ trees and the model estimates (HKY+Gamma) obtained for the two trees.</li>
      <li>Compare the likelihood of the ML and BioNJ trees.</li>
      <li>What do you observe and why?</li>
      
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
