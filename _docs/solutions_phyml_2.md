---
title: Solution 3 - Model comparison
permalink: /docs/solutions_phyml_2/
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

---

<h5 id="execution-2">Execution</h5>

<table>
<thead>
<tr>
  <th>Model</th>
  <th>Log-likelihood</th>
  <th>Parameters</th>
  <th>AIC</th>
</tr>
</thead>
<tbody><tr>
  <td>JC</td>
  <td>-6379.66383</td>
  <td>38</td>
  <td>12835.32766</td>
</tr>
<tr>
  <td>JC_I</td>
  <td>-6311.41650</td>
  <td>39</td>
  <td>12700.833</td>
</tr>
<tr>
  <td>JC_G</td>
  <td>-6304.38084</td>
  <td>39</td>
  <td>12686.76168</td>
</tr>
<tr>
  <td>JC_G_I</td>
  <td>-6304.35263</td>
  <td>40</td>
  <td>12688.70526</td>
</tr>
<tr>
  <td>HKY</td>
  <td>-6251.43051</td>
  <td>42</td>
  <td>12586.86102</td>
</tr>
<tr>
  <td>HKY_I</td>
  <td>-6180.09689</td>
  <td>43</td>
  <td>12446.19378</td>
</tr>
<tr>
  <td>HKY_G</td>
  <td>-6172.58045</td>
  <td>43</td>
  <td>12431.1609</td>
</tr>
<tr>
  <td>HKY_G_I</td>
  <td>-6172.52896</td>
  <td>44</td>
  <td>12433.05792</td>
</tr>
<tr>
  <td>GTR</td>
  <td>-6241.48788</td>
  <td>46</td>
  <td>12574.97576</td>
</tr>
<tr>
  <td>GTR_I</td>
  <td>-6171.17472</td>
  <td>47</td>
  <td>12436.34944</td>
</tr>
<tr>
  <td>GTR_G</td>
  <td>-6163.87291</td>
  <td>47</td>
  <td>12421.74582</td>
</tr>
<tr>
  <td>GTR_G_I</td>
  <td>-6172.52896</td>
  <td>48</td>
  <td>12441.05792</td>
</tr>
</tbody></table>


<p>The number of parameters are computed in the following way for a rooted <br>
tree:</p>

<blockquote>
  <p><script type="math/tex" id="MathJax-Element-11">k = (2 \ast \text{no. taxa} - 2) + \text{no. parameters in substitution model} + \text{extra parameters}</script></p>

  <p>substitution models: JC = 0 parameters | HKY = 4 parameters | GTR = 8 <br>
  parameters <br>
  invariant sites = +1 parameter <br>
  gamma rates = +1 parameter</p>
</blockquote>

<p>We compute the AIC value as follows:</p>

<blockquote>
  <p><script type="math/tex" id="MathJax-Element-12">AIC = 2(k) - \log(L)</script></p>
</blockquote>


---

<h5 id="questions-2">Questions</h5>

<p><strong>1. Which model is the best (including HKY+Gamma), based on the AIC criterion?</strong></p>

<p>We select the model with the lowest AIC value. In this case, <strong>GTR + Gamma</strong></p>

<hr>

<p>This exercise can also be solved using <a href="https://github.com/ddarriba/jmodeltest2">jmodeltest</a> which performs automatically phylogenetic tree reconstructions with every model and extra parameters (i.e. invariant sites, gamma).</p>


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
