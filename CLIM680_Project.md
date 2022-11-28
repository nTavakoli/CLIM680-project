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

In this project, El Niño months are defined as those with values of SOI less than the 15th percentile of the SOI distribution; the value of the 15th percentile of SOI is -0.73. Moreover, La Niña months are considered as those with values of SOI more than the 85th percentile of the SOI distribution; the value of the 85th percentile of SOI is 1. Neutral condition is also defined as those with values of SOI between -0.73 and 1.

![Southern Oscillation Index for 2011-2020](https://user-images.githubusercontent.com/114028224/204163634-65e776a5-d8ac-486a-a5d6-685b1861e2ff.png)

![Southern Oscillation Index for 2011-2020_1](https://user-images.githubusercontent.com/114028224/204168168-bc13fec1-1c1d-4729-bb44-64a2a38fb2c7.png)

![Southern Oscillation Index for 2011-2020_2](https://user-images.githubusercontent.com/114028224/204168199-257597af-b4eb-4325-9bf9-8c8436098245.png)


Link to dataset description: https://www.ncei.noaa.gov/access/monitoring/enso/soi

### Results and Analysis
Project Notebook via GitHub located within my "CLIM680_project" repository includes a series of jupyter notebooks containing all the labeled and commented code used in my analysis. Each topic will be discussed separately, along with a link to each relevant notebook.

Link: https://github.com/nTavakoli/CLIM680-project

### Functions

Two sets of functions were created to calculate climatologies and anomalies and or labeling plots.

Link to xyticks function: https://github.com/nTavakoli/CLIM680-project/blob/main/Functions/Defining_xricks_yticks_function.ipynb

Link to climo,anoms function: https://github.com/nTavakoli/CLIM680-project/blob/main/Functions/climo_anoms_function.ipynb

### Conda Environment

All environments used in this project have been provided in the environment.yml file.

### Figures
The figures from my project notebook are saved in a seperate 'figures' subdirectory, as well as shown in the project notebook.

Link: 

### Climatology and Anomalies

Link: 

### Composite AET Anomalies during ENSO

Link:

### Regression Analysis 

Link:

### Correlation Analysis

Link:

### Summary





### References
W. Dorigo et al., “ESA CCI Soil Moisture for improved Earth system understanding: State-of-the art and future directions,” Remote Sens. Environ., vol. 203, pp. 185–215, 2017, doi: https://doi.org/10.1016/j.rse.2017.07.001.

A. Gruber, T. Scanlon, R. van der Schalie, W. Wagner, and W. Dorigo, “Evolution of the ESA CCI Soil Moisture climate data records and their underlying merging methodology,” Earth Syst. Sci. Data, vol. 11, no. 2, pp. 717–739, 2019, doi: https://doi.org/10.5194/essd-11-717-2019.

A. Gruber, W. A. Dorigo, W. Crow, W. Wagner, “Triple Collocation-Based Merging of Satellite Soil Moisture Retrievals”, IEEE Transactions on Geoscience and Remote Sensing. PP. 1-13, (2017), https://doi.org/10.1109/TGRS.2017.2734070

J. T. Abatzoglou, S. Z. Dobrowski, S. A. Parks, and K. C. Hegewisch, “TerraClimate, a high-resolution global dataset of monthly climate and climatic water balance from 1958-2015,” Sci. Data, vol. 5, pp. 1–12, 2018, doi: 10.1038/sdata.2017.191.


### Acknowledgments
I would like to thank both the CLIM680 instructors Prof. Paul Dirmeyer and Prof. Luis Ortiz Uriarte for coding assistance and answering questions.
