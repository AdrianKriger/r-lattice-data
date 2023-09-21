---
layout: default
title: The Dataset
nav_order: 2
---

# The Dataset

In this practical we will be working with South African Police Service (SAPS), Statistics South Africa (STATSSA) and the City of Cape Town (CoCT)  open data. The data set contains information on crime (combined residential burglaries and residential thefts) and property valuation as well as other variables specific to Cape Town, South Africa in 2015.  
<br>
**In the spirit of Open Science and Open Data the creation of this dataset is available as a seperate document: [latticeSpatial](https://github.com/AdrianKriger/r-lattice-data/blob/main/latticeSpatial.ipynb)**. It is open for inquiry, exploration and welcomes contribution, criticism and review.
<br>
Unit of analysis: 777 suburbs in Cape Town, South Africa

The variables contained in the dataset are:  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`OBJECTID`   : polygon ID  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`OFC_SBRB_N` : official suburb name  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`SHAPE_Leng` : suburb perimeter  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`SHAPE_Area` : suburb area   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`OFFICIAL_SUBURB` : suburb name carried over from property valuation dataset  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`NUM_RES_PROP` : number residential properties sold.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`MED_LAND_EXTENT.m2` : median extent land (m^2)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`MED_TOT_BLD_AREA.m2` : median building area (m^2)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`GV2015VAL` : 2015 general property valuation  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`X` : x coordinate of suburb centroid  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`Y` : y coordinate of suburb centroid   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`AVESTADist` : average distance to the local police station  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`AVAPREArea` : average precinct area  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`AvePrecinctsLen` : average precinct perimeter  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`ROBRes` : residential robbery  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`BUGRes` : residential burglary  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`CRIME` : total theft  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`AVMEDINC` : average median household income  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`BACH` : number bachelors degrees  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`AVBACH` : average number bachelors degrees  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`STA` : police station  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`STAD` : distances to the local police station  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`PREA` : precinct area  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`PREL` : precinct perimeter  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`WARD` : official ward / track number  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; •	`geom` : suburb geometry
<br>
The dataset comes in the form of a `shapefile` within a `.geopackage` along with ALL the source material. Analysis will focus on `SHAPE_Area`, `GV2015_VAL`, `AVESTADist' 'AVAPREArea`, `CRIME`, `INCOME`, `AVBAC`.
