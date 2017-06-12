---
title: Exercise 6 - Inferring ML phylogenies with codon models
permalink: /docs/exercises_phyml_5/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
In this tutorial you will be guided in using PhyML and its extension, CodonPhyML, to solve common phylogenetic problems. For some of the following exercises there might be more than one single solution.

---

##### **Goal: Inferring ML phylogenies with codon models using CodonPhyML**

For this task, use CodonPhyML (the menu mode) to analyse your dataset (data should be protein-coding DNA). The menu interface is very similar to PhyML except CodonPhyML includes codon models and some additional amino acid models (eg, PCA models by Zoller and Schneider; antibody model AB by Mirsky et al 2015; models for ordered/disordered proteins by Szalkowski and Anisimova 2011).

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

### Fist Step

Choose to work with a protein-coding DNA dataset (codon sequences, eg, one of datasets).

The dataset should not include any stop codon, therefore we must modify the dataset deleting the last 3 columns (the last codon) from the MSA. In order to do so, you can open primates-nt.phy with AliView and after selecting the last 3 columns press delete on the keyboard. Save the new file as Phylip with the following name primates-nt-nostop.phy.

### Second Step
Analyze the data using codon models M0, M0+Gamma and M5; amino acid models LG, WAG, LG+Gamma and WAG+Gamma; and GTR+Gamma.
The Log-likelihods for codon models and amino acid models are comparable. For GTR+Gamma model, the converted log-likelihood score is also available so the comparison across DNA, AA and codon models can be made.

<div class="panel panel-info">
    <div class="panel-heading">Informations</div>
    <div class="panel-body">
        You will run CodonPhyML at maximum 8 times
    </div>
</div>
---


<div class="panel panel-default">
    <div class="panel-heading">Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Based on AIC, which model fits your dataset best?</li>
      <li>Are the trees inferred using the best AA and best codon model different?</li>
      <li>Are they different to the tree inferred using the DNA model?</li>
    </ol>
    </div>
</div>

---

This exercise was prepared by *Maria Anisimova*
