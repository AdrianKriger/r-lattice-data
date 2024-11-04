---
layout: default
title: Home
nav_order: 1
description: "Lattice Data with R."
---

# Lattice Data with R (Cape Town)
{: .fs-9 }

In this exercise, we explore the concepts and applications of spatial autocorrelation _(Is their a relationship between attributes and their location? Do similar attributes cluster? Is their an underlying (spatial) pattern in the data?)_.

<figure><center>
  <!--<img src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 300px; border: 0px">-->
  <iframe src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 400px; border: 0px"></iframe>
  <figcaption>Fig.1 - Residential crime (theft and burglary) per suburb (Cape Town, South Africa) </figcaption>
</center></figure> 

<!-- <iframe src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 300px; border: 0px"></iframe> -->

The aim is to equip a user with the skills to understand and test the connections and relationship between lattice data with such methods as Global and Local Morans as-well-as extending ordinary least squares regression to accommodate location; namely geographically weighted regression. 

We traverse such technics as:

&nbsp;&nbsp;&nbsp;**1) Spatial Autocorrelation**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. Neighbors and Weight Matrices  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b. Moran’s I, along with its Monte-Carlo derivative, test for spatial autocorrelation  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c. Moran’s scatter plot and correlogram  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;d. Local Indicators of Spatial Autocorrelation (LISA)  
&nbsp;&nbsp;&nbsp;**3) Ordinary Least Squares (OLS) Regression** and **Geographically Weighted Regresssion (GWR)**  
&nbsp;&nbsp;&nbsp;**4)** we also briefly highlight ways we can **interrogate the quality** of a GWR with;  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. three `spgwr` significance tests

<!--<figure><center>
  <img src="{{site.baseurl | prepend: site.url}}/img/5-fold.png" style="width: 800px; height: 300px; border: 0px">
  <figcaption>Fig.2 - Inverse Distance Weighting, 2nd-order Ordinary Least Squares and Ordinary Kriging interpolation </figcaption>
</center></figure>-->

For this assignment we use a dataset that is well-suited to illustrate these concepts. A lattice dataset containing such variables such as: residential theft and burglaries (SAPS SA), median property valuation (City of Cape Town Open Data), median income and number Bachelor degrees (STATSSA), among other variables, of suburbs within the City of Cape Town; South Africa. The dataset is discussed in [The Dataset](https://adriankriger.github.io/r-lattice-data/docs/data/).

<!--The [meuse](https://search.r-project.org/CRAN/refmans/sp/html/meuse.html) dataset which comes with the `gstat` package. 
**meuse**: gives locations (on a regular grid) and topsoil heavy metal concentrations, along with a number of soil and landscape variables at the observation locations, collected in a flood plain of the river Meuse, near the village of Stein (NL). Heavy metal concentrations are from composite samples of an area of approximately 15 m x 15 m.-->
