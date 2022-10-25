El Niño–La Niña cycle and recent trends in continental evaporation

Nazanin Tavakoli

CLIM 680 - Fall 2022

Introduction

The hydrological cycle is expected to intensify in response to global warming with acceleration on a global scale. This holds in particular for terrestrial evaporation, the crucial return flow of water from land to the atmosphere. A better understanding of the interactions between soil moisture, vegetation activity, and evaporation, and how these variables are affected by climatic factors, is critical for informing debate on current and future changes in a warming world.
As a result, in this project, I will show the atmospheric moisture content and evapotranspiration associated with La Niña (El Niño) events using the southern Oscillation Index (SOI). This topic has already been explored by other researchers  (Diego G. Miralles1 et al.).

Data

ESA Climate Change Initiative (CCI) SM v06.1
This product provides global merged surface soil moisture datasets with NetCDF format at daily temporal resolution from 1978 to 2020 and spatial resolution of 0.25°; however, I will narrow my analysis only from 2011-2020 in the global domain due to the size of this dataset.
 
References:
W. Dorigo et al., “ESA CCI Soil Moisture for improved Earth system understanding: State-of-the art and future directions,” Remote Sens. Environ., vol. 203, pp. 185–215, 2017, doi: https://doi.org/10.1016/j.rse.2017.07.001.

A. Gruber, T. Scanlon, R. van der Schalie, W. Wagner, and W. Dorigo, “Evolution of the ESA CCI Soil Moisture climate data records and their underlying merging methodology,” Earth Syst. Sci. Data, vol. 11, no. 2, pp. 717–739, 2019, doi: https://doi.org/10.5194/essd-11-717-2019.

A. Gruber, W. A. Dorigo, W. Crow, W. Wagner, “Triple Collocation-Based Merging of Satellite Soil Moisture Retrievals”, IEEE Transactions on Geoscience and Remote Sensing. PP. 1-13, (2017), https://doi.org/10.1109/TGRS.2017.2734070

For more information, visit this website:

https://esa-soilmoisture-cci.org/

TerraClimate

Actual Evapotranspiration

TerraClimate is a dataset of monthly climate and climatic water balance for global terrestrial surfaces from 1958-2019. These data provide monthly climate and climatic water balance for global terrestrial surfaces with NetCDF format from 1958-2021 with a spatial resolution of ~4-km (1/24th degree).

References:

J. T. Abatzoglou, S. Z. Dobrowski, S. A. Parks, and K. C. Hegewisch, “TerraClimate, a high-resolution global dataset of monthly climate and climatic water balance from 1958-2015,” Sci. Data, vol. 5, pp. 1–12, 2018, doi: 10.1038/sdata.2017.191.

For more information, visit this website:

https://www.climatologylab.org/terraclimate.html

Moderate Resolution Imaging Spectroradiometer (MODIS)

Normalized Difference Vegetation Index (NDVI)

The MOD13A3 Version 6 data are provided monthly NDVI index with HDF format at 1 kilometer (km) spatial resolution from 2000 to the present. In this project, we are using this data from 2011 to 2020.

References:

Didan, K.. MOD13A3 MODIS/Terra vegetation Indices Monthly L3 Global 1km SIN Grid V006. 2015, distributed by NASA EOSDIS Land Processes DAAC, https://doi.org/10.5067/MODIS/MOD13A3.006. Accessed 2022-10-24.

For more information, visit this website:

https://lpdaac.usgs.gov/products/mod13a3v006/

Southern Oscillation Index (SOI) 

SOI Index is the monthly index provided by NOAA (National Oceanic and Atmospheric Administration) from 1951 to the present.

For more information, visit this website:

https://www.ncei.noaa.gov/access/monitoring/enso/soi

Proposed Analysis

I will use the following analysis in this project:

Interpolating or extrapolating data

Use the groupby function to calculate climatologies by month or year

Calculate the Time series of global annual anomalies of ET

Calculate the Spatial distribution of the linear trends in ET

Calculate the correlation coefficient between monthly anomalies of ET and the SOI, the SOI and soil moisture, and the SOI and NDVI

Calculate monthly mean anomalies of ET, soil moisture, and NDVI during El Niño and La Niña

Calculate the regression of SOI with ET and Soil moisture

Functions

I will create a set of functions for doing this project, such as calculating anomalies or labeling plots. More ideas for creating functions may come to my mind while I am working on this project.

Conda Environment

All environments used in this project have been provided in the environment.yml file.
