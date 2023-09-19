---
layout: default
title: Home
nav_order: 1
description: "Spatial Statistics with R."
---

# (Geo)spatial Statistics with R (Meuse)
{: .fs-9 }

In this exercise, we will explore the concepts and applications of Deterministic and Stochastic Interpolation Methods. 

<figure><center>
  <img src="{{site.baseurl | prepend: site.url}}/img/preds.png" style="width: 800px; height: 300px; border: 0px">
  <figcaption>Fig.1 - Inverse Distance Weighting, 2nd-order Ordinary Least Squares and Ordinary Kriging interpolation </figcaption>
</center></figure> 

<!-- <iframe src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 300px; border: 0px"></iframe> -->
We traverse such technics as:

&nbsp;&nbsp;&nbsp;**1) Deterministic methods**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. Thiessen polygons  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b. Linear Regression  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c. Inverse Distance Weighting  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;d. Ordinary Least Squares  
&nbsp;&nbsp;&nbsp;**2) Stochastic methods**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. Variograms and Kriging  
&nbsp;&nbsp;&nbsp;**3)** we also briefly highlight ways we can **interrogate the quality** of an interpolation with;  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. _N_-fold cross validation; and  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b. Residual Mean Squared Error (rmse).

<!--<figure><center>
  <img src="{{site.baseurl | prepend: site.url}}/img/5-fold.png" style="width: 800px; height: 300px; border: 0px">
  <figcaption>Fig.2 - Inverse Distance Weighting, 2nd-order Ordinary Least Squares and Ordinary Kriging interpolation </figcaption>
</center></figure>-->
_____
For this assignment we use a dataset that is well-suited to illustrate these concepts. The [meuse](https://search.r-project.org/CRAN/refmans/sp/html/meuse.html) dataset which comes with the `gstat` package. 
**meuse**: gives locations (on a regular grid) and topsoil heavy metal concentrations, along with a number of soil and landscape variables at the observation locations, collected in a flood plain of the river Meuse, near the village of Stein (NL). Heavy metal concentrations are from composite samples of an area of approximately 15 m x 15 m.
