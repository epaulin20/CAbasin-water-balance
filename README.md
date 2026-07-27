# huc8basin-water-balance

The goal of this repository is to automate ET evaluation using a basin water balance-based ET (WBET) at the Hydrologic Unit Code 8 spatial scale. 

WBET = P - Q - dS/dt

Where P is precipitation, Q is discharge, and dS/dt is change in storage. This analysis uses multi-water-year average P and Q and assumes dS/dt to be 0. 

The HUC8 basins were identified by matching USGS-gauges to basin outflow points. A classification was applied to rate the match of stream gauge to HUC8 water basins.

### Data description

* Discharge data are sourced from the USGS.
	* get_q.ipynb: is a script to download USGS discharge data
* ET, precipitation are sourced from Google Earth Engine (GEE). 
	* get_et.ipynb is a script to download OpenET data from GEE.

* **Q data** are downloaded and converted from cubic feet per second to basin average depth (mm) to compare with Precipitation.



* **ET models** include:

	|Model | Citation | GEE Image Collection Path|
	|DisALEXI | Citation | GEE Image Collection Path|
	|eeMETRIC | Citation | GEE Image Collection Path|
	|geeSEBAL | Citation | GEE Image Collection Path|
	|PT-JPL | Citation | GEE Image Collection Path|
	|SSEBop | Citation | GEE Image Collection Path|
	|OpenET ensemble | Citation | GEE Image Collection Path|

* The **precpitation data** products include

|Product | Citation | GEE Image Collection Path|


### Analysis
