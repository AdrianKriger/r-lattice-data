---
layout: default
title: Home
nav_order: 1
description: "Lattice Data with R."
---

# Lattice Data with R (Cape Town)
{: .fs-9 }

In this exercise, we will explore the concepts and applications of spatial autocorrelation _(Is their a relationship between attributes and their location? Do similar attributes cluster? Is their an underlying (spatial) pattern in the data?)_ and extend Ordinary Least Squares regression with location; namely Geographically Weighted Regression.

<figure><center>
  <!--<img src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 300px; border: 0px">-->
  <iframe src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 400px; border: 0px"></iframe>
  <figcaption>Fig.1 - Residential crime (theft and burglary) per suburb (Cape Town, South Africa) </figcaption>
</center></figure> 

<!-- <iframe src="{{site.baseurl | prepend: site.url}}/img/plotly.html" style="width: 800px; height: 300px; border: 0px"></iframe> -->
We traverse such technics as:

&nbsp;&nbsp;&nbsp;**1. Exploratory Data Analysis**  
&nbsp;&nbsp;&nbsp;**2. Defining Neighbors and Constructing a Weight Matrix**  
&nbsp;&nbsp;&nbsp;**3. Moran's I test for Spatial Autocorrelation**  
&nbsp;&nbsp;&nbsp;**4. Moran's I significance test through simulation**  
&nbsp;&nbsp;&nbsp;**5. Moran's scatter plot**   
&nbsp;&nbsp;&nbsp;**6. Correlogram**  
&nbsp;&nbsp;&nbsp;**7. Local Indicators of Spatial Autocorrelation (LISA)**  
&nbsp;&nbsp;&nbsp;**8. Ordinary Least Squares (OLS) Regression**  
&nbsp;&nbsp;&nbsp;**9. Geographically Weighted Regresssion (GWR)**  and  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a. check the quality of a GWR with three 'spgwr` significance tests

<!--<figure><center>
  <img src="{{site.baseurl | prepend: site.url}}/img/5-fold.png" style="width: 800px; height: 300px; border: 0px">
  <figcaption>Fig.2 - Inverse Distance Weighting, 2nd-order Ordinary Least Squares and Ordinary Kriging interpolation </figcaption>
</center></figure>-->
_____
For this assignment we use a dataset that is well-suited to illustrate these concepts. A lattice dataset containing such variables such as: residential theft and burgalaries (SAPS SA), median property valuation (City of Cape Town Open Data), median income and number Bachelor degrees (STATSSA), among other variables, of suburbs within the City of Cape Town; South Africa.

<!--The [meuse](https://search.r-project.org/CRAN/refmans/sp/html/meuse.html) dataset which comes with the `gstat` package. 
**meuse**: gives locations (on a regular grid) and topsoil heavy metal concentrations, along with a number of soil and landscape variables at the observation locations, collected in a flood plain of the river Meuse, near the village of Stein (NL). Heavy metal concentrations are from composite samples of an area of approximately 15 m x 15 m.-->
