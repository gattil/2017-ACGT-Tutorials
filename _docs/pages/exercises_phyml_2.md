---
title: Exercise 3 - Model comparison
permalink: /docs/exercises_phyml_2/
redirect_from: /index.html
---

##### Inferring phylogenies using maximum likelihood
###### **Observing the effect of substitution models the final inferred tree topology.**

<br>

#### Goals

In this exercise you are asked to compare different substitution models (and their variations) on the same dataset.


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


##### First Run

Run PhyML with the substitution model set to **GTR**, estimating the nucleotide frequencies empirically from the dataset, and executing the tree search optimisation routines.

In addition, set the following options:

<div class="row">
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">1. GTR</div>
            <div class="panel-body">
            No extra option
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">2. GTR+Gamma</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">3. GTR+I</div>
            <div class="panel-body">
            <ul>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">4. GTR+Gamma+I</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
</div>


##### Second Run

Run PhyML with the substitution model set to **HKY**, estimating the transition/transversion ratio, estimating the nucleotide frequencies empirically from the dataset, and executing the tree search optimisation routines.

In addition, set the following options:

<div class="row">
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">1. HKY</div>
            <div class="panel-body">
            No extra option
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">2. HKY+Gamma</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">3. HKY+I</div>
            <div class="panel-body">
            <ul>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">4. HKY+Gamma+I</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
</div>



##### Third Run

Run PhyML with the substitution model set to **JC**, nucleotide frequencies are estimated empirically from the dataset, and executing the tree search routines.

In addition, set the following options:

<div class="row">
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">1. JC</div>
            <div class="panel-body">
            No extra option
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">2. JC+Gamma</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">3. JC+I</div>
            <div class="panel-body">
            <ul>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
    <div class="col-xl-3 col-lg-6">
        <div class="panel panel-default">
            <div class="panel-heading">4. JC+Gamma+I</div>
            <div class="panel-body">
            <ul>
            <li>Gamma distribution with 4 classes</li>
            <li>Estimating Gamma shape parameter</li>
            <li>Adding Invariable sites option</li>
            </ul>
            </div>
        </div>
    </div>
</div>





<div class="panel panel-info">
    <div class="panel-heading">Informations</div>
    <div class="panel-body">
        You will run PhyML at maximum 12 times (remember that some combinations have been run previously in exercise 1 and 2)
    </div>
</div>

---


<div class="panel panel-default">
    <div class="panel-heading">Tasks</div>
    <div class="panel-body">
    <ol>
      <li>Which model is the best (including HKY+Gamma), based on the AIC criterion?</li>
      <li>What about adding invariant sites (+I)?</li>
    </ol>
    </div>
</div>
