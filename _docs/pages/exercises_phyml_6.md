---
title: Exercise 7 - Inferring ML phylogenies using real datasets
permalink: /docs/exercises_phyml_6/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
In this tutorial you will be guided in using PhyML and its extension, CodonPhyML, to solve common phylogenetic problems. For some of the following exercises there might be more than one single solution.

---

##### **Goal: Analysing real datasets**

Analyze a real dataset - the primate AA dataset - and test for substitution models with and without frequencies estimation.

---


<div class="panel panel-primary">
    <div class="panel-heading">Datasets</div>
    <div class="panel-body">
        Dataset file: <div class="btn-group">
          <a href="#" class="btn btn-default">primates-aa.phy</a>
          <a href="#" class="btn btn-default dropdown-toggle" data-toggle="dropdown"><span class="caret"></span></a>
          <ul class="dropdown-menu">
            <li><a href="#">View</a></li>
            <li><a href="../../tutorial_data/tutorial01_phyml/primates-aa.phy">Download</a></li>
          </ul>
        </div>
    </div>
</div>

---

### Fist Step

Set the model to <em>LG+Gamma</em>, and try both <em>+F</em> and <em>–F</em> options.

### Second Step

Search for the best model using ProtTest: http://darwin.uvigo.es/software/prottest2_server.html

---


<div class="panel panel-default">
    <div class="panel-heading">Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Compare the trees and the likelihood values. Which model is best, based on AIC criterion.
      What about using invariant sites?</li>
      <li>After executing the second step, compare the trees, likelihood and AIC values to those of <em>LG+Gamma</em>.  
</li>
    </ol>
    </div>
</div>

---

This exercise was prepared by *Maria Anisimova*
