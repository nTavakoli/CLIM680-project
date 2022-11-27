# El Niño–La Niña cycle and recent trends in continental evaporation

## Nazanin Tavakoli

## CLIM 680 - Fall 2022

### Introduction

The hydrological cycle is expected to intensify in response to global warming with acceleration on a global scale. This holds in particular for terrestrial evaporation, the crucial return flow of water from land to the atmosphere. A better understanding of the interactions between soil moisture, vegetation activity, and evaporation, and how these variables are affected by climatic factors, is critical for informing debate on current and future changes in a warming world. 
     
 The Southern Oscillation (ENSO), the cycling of El Niño and La Niña, has strong impacts on weather around the world by influencing high and low pressure systems, winds, and precipitation. Also, as the warmer ocean waters release excess energy (heat) into the atmosphere, global temperatures rise. The Southern Oscillation Index (SOI), a standardized index based on the observed sea level pressure (SLP) differences between Tahiti and Darwin, Australia, is one measure of the large-scale fluctuations in air pressure occurring between the western and eastern tropical Pacific during the Southern Oscillation states. In general, smoothed time series of the SOI correspond very well with changes in ocean temperatures across the eastern tropical Pacific. The negative phase of the SOI represents below-normal air pressure at Tahiti and above-normal air pressure at Darwin. Prolonged periods of negative (positive) SOI values coincide with abnormally warm (cold) ocean waters across the eastern tropical Pacific typical of El Niño (La Niña) episodes.
   
 In this project, I will show the atmospheric moisture content and evapotranspiration associated with La Niña (El Niño) events using the southern Oscillation Index (SOI). To be more specific, in this project, the monthly averaged variables of soil moisture and actual evapotranspiration will be analyzed over the domain of Australia to tackle how these variables have changed in the La Niña (El Niño) events. The analysis will include climatology calculations, correlations, linear regressions, and composites. Previous work has shown that during El Niño, limitations in terrestrial moisture supply result in vegetation water stress and reduced evaporation in eastern and central Australia. The opposite situation occurs during La Niña (Diego G. Miralles1 et al.).With this motivation, the impacts of SOI on soil moisture and evapotranspiration over Australia will be analyzed.


### Data
The datasets used in my project are:

#### ESA Climate Change Initiative (CCI) SM v06.1
##### Soil Moisture
This product provides global merged surface soil moisture datasets with NetCDF format at daily temporal resolution from 1978 to 2020 and spatial resolution of 0.25°; however, I will narrow my analysis only from 2011-2020 in the global domain due to the size of this dataset.

Link to dataset description: https://esa-soilmoisture-cci.org/

#### TerraClimate

##### Actual Evapotranspiration

TerraClimate is a dataset of monthly climate and climatic water balance for global terrestrial surfaces from 1958-2019. These data provide monthly climate and climatic water balance for global terrestrial surfaces with NetCDF format from 1958-2021 with a spatial resolution of ~4 km (1/24th degree).

TerraClimate uses climatically aided interpolation, combining high-spatial resolution climatological normals from the WorldClim dataset, with coarser spatial resolution, but time-varying data from CRU Ts4.0 and the Japanese 55-year Reanalysis (JRA55). Conceptually, the procedure applies interpolated time-varying anomalies from CRU Ts4.0/JRA55 to the high-spatial-resolution climatology of WorldClim to create a high-spatial-resolution dataset that covers a broader temporal record.

Link to dataset description: https://www.climatologylab.org/terraclimate.html

#### Southern Oscillation Index (SOI) 

SOI Index is the monthly index provided by NOAA (National Oceanic and Atmospheric Administration) from 1951 to the present.

Link to dataset description: https://www.ncei.noaa.gov/access/monitoring/enso/soi

### Results and Analysis
Project Notebook via GitHub located within my "CLIM680_project" repository includes a series of jupyter notebooks containing all the labeled and commented code used in my analysis. Each topic will be discussed separately, along with a link to each relevant notebook.

Link: 



### Functions

I will create a set of functions for doing this project, such as calculating anomalies or labeling plots. More ideas for creating functions may come to my mind while I am working on this project.

### Conda Environment

All environments used in this project have been provided in the environment.yml file.
