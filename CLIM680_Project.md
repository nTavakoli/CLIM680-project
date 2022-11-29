# El Niño–La Niña cycle and recent trends in regional evapotranspiration and soil moisture

## Nazanin Tavakoli

## CLIM 680 - Fall 2022

### Introduction

The hydrological cycle is expected to intensify in response to global warming with acceleration on a global scale. This holds in particular for terrestrial evaporation, the crucial return flow of water from land to the atmosphere. A better understanding of the interactions between soil moisture, vegetation activity, and evaporation, and how these variables are affected by climatic factors, is critical for informing debate on current and future changes in a warming world. 
     
 The Southern Oscillation (ENSO), the cycling of El Niño and La Niña, has strong impacts on weather around the world by influencing high and low pressure systems, winds, and precipitation. Also, as the warmer ocean waters release excess energy (heat) into the atmosphere, global temperatures rise. The Southern Oscillation Index (SOI), a standardized index based on the observed sea level pressure (SLP) differences between Tahiti and Darwin, Australia, is one measure of the large-scale fluctuations in air pressure occurring between the western and eastern tropical Pacific during the Southern Oscillation states. In general, smoothed time series of the SOI correspond very well with changes in ocean temperatures across the eastern tropical Pacific. The negative phase of the SOI represents below-normal air pressure at Tahiti and above-normal air pressure at Darwin. Prolonged periods of negative (positive) SOI values coincide with abnormally warm (cold) ocean waters across the eastern tropical Pacific typical of El Niño (La Niña) episodes.
   
 In this project, I will show the atmospheric moisture content and evapotranspiration associated with La Niña (El Niño) events using the southern Oscillation Index (SOI). To be more specific, in this project, the monthly averaged variables of soil moisture (SM) and actual evapotranspiration (AET), the quantity of water that is removed from a surface due to the processes of evaporation and transpiration and is measured in millimeters (mm), will be analyzed over the domain of Australia to tackle how these variables have changed in the La Niña (El Niño) events. The analysis will include climatology calculations, correlations, linear regressions, and composites. Previous work has shown that during El Niño, limitations in terrestrial moisture supply result in vegetation water stress and reduced evaporation in eastern and central Australia. The opposite situation occurs during La Niña (Diego G. Miralles1 et al.).With this motivation, the impacts of SOI on soil moisture and evapotranspiration over Australia will be analyzed.


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

Link: https://github.com/nTavakoli/CLIM680_Project/tree/main/Figures

### Climatology and Anomalies

Time series of monthly anomalies of AET and SM have been plotted in response to the SOI index from 2011 to 2020 due to investigate the oscillation of AET and SM with the alternation of El Niño and La Niña events. The following plot reveals that years in which AET is high, coincide with La Niño conditions. On the other hand, years of low AET mostly correspond to El Niña years. 

![Time series of AET   SOI monthly anomalies](https://user-images.githubusercontent.com/114028224/204381182-a3e869c5-b26f-4589-96a9-368235bdb514.png)

A panel plot of monthly anomalies of SM and SOI index shows that the largest amount of SM happened during La Nino. However, negative monthly anomalies of SM can be found during strong El Nino. As we know, El Niño events are associated with warmer temperatures and a reduction in rainfall which cause soil moisture to decrease.

![Time series of SM   SOI monthly anomalies](https://user-images.githubusercontent.com/114028224/204381271-dab83d27-80b0-48e4-af7d-a59b07342add.png)



Link: https://github.com/nTavakoli/CLIM680_Project/blob/main/Codes/Monthly%20anomalies%20of%20SOI%20%26%20AET%20and%20SM.ipynb

### Composite AET and SM Anomalies during ENSO

The composite analysis was performed on actual evapotranspiration anomalies and soil moisture over Australia with the SOI index. These Composites were then plotted during El Niño, La Niña, and neutral events, mentioned in the following. The composite of actual evapotranspiration anomalies indicates that most of Australia have a negative composite with SOI during El Niño, especially in the east, north, and north-western of this continent; however, a weak positive composite can be observed in the north-eastern. Also, the weak negative composite of soil moisture with SOI is observed in the northern and central of Australia during El Niño.

During La Niña, positive composite with SOI dominates over most of Australia, and the strongest ones are in central and western. This pattern seems to be found in the plot of soil moisture composite with SOI with less strength compared to actual evapotranspiration composite during La Niña condition.



![Composite Actual Evapotranspiration Anomalies during ENSO](https://user-images.githubusercontent.com/114028224/204168393-1c3a4d05-50a4-45b3-a2c7-74225f76bf4a.png)


![Composite Soil Moisture Anomalies during ENSO](https://user-images.githubusercontent.com/114028224/204169649-21654981-1dc6-4f27-a5b7-f806184d8f86.png)

Link: https://github.com/nTavakoli/CLIM680-project/blob/main/Codes/Composite_AET_SOI.ipynb

Link: https://github.com/nTavakoli/CLIM680-project/blob/main/Codes/Composite_SM_SOI.ipynb

### Regression Analysis 

For linear regression analysis, anomalies were once again calculated for each of the two variables, including soil moisture and actual evapotranspiration.

First, the regression was applied between the SOI and actual evapotranspiration anomaly time series, see the following. The regression coefficient is positive in most of Australia, except in the northeast and some part of central, however, a strong positive slope between the SOI and actual evapotranspiration can be observed in the western part of Australia, with statistically significant regression coefficients at the 95% confidence level indicated by the hatchings.

![Regression between SOI and AET Anomalies](https://user-images.githubusercontent.com/114028224/204174092-89af5a0b-ca69-4f5c-a5cf-4260105b8ea1.png)

Second, a panel plot map of the linear regression between SOI and soil moisture is then shown, and dotting represents statistically significant (p<0.05) regression. Based on this map, areas of the strongest positive slope between soil moisture anomalies and the SOI Index are found in the northeast and northwest of Australia. Most regions have a positive slope, however, the values of the regression coefficient between soil moisture anomalies and the SOI are small. This can be because of noise in the precipitation datasets. As we know, soil moisture is responding to precipitation, and precipitation is a noisy field. 

It should be noted that the strongest positive slope between soil moisture and SOI index and between actual evapotranspiration and SOI is observed in the same region, northwest of Australia.

![Regression between SOI and Soil Moisture Anomalies](https://user-images.githubusercontent.com/114028224/204174136-16c7be60-a8af-4f7f-8b7c-1ab7c9c9533f.png)



Link: https://github.com/nTavakoli/CLIM680_Project/blob/main/Codes/Linear%20Regression%26Correlation%20Coefficient.ipynb

### Correlation Analysis

For correlation analysis, the correlation of each of the two variables (soil moisture and actual evapotranspiration) with the SOI index was investigated, and plots are shown in the following. Dotting represents statistically significant (p<0.05) correlations.

Firstly, the monthly mean anomalies of AET show significant positive correlations with the Southern Oscillation Index (SOI) in the northwest of Australia as well as in a small region in the southeast (0.30<R<0.45). Also, a strong statistically significant positive correlation between soil moisture and SOI index is found in these regions (0.30<R<0.60). My results indicate that there is a weak statistically significant correlation between AET and SOI index and between soil moisture and SOI index in other parts of Australia.

During El Niño, there is typically a decrease in the amount of rain falling over Australia and more heatwaves and droughts occur in these parts, especially in the northwestern due to the weak trade winds leading to the warm weather shifting to the eastern part of equatorial Pacific ocean. This reduced moisture supply is potentially related to changes in atmospheric circulation and decreases in evaporation in these regions. The significant correlation between AET and SOI as well as between soil moisture and SOI index confirms that during El Niño episodes an overall reduction in land precipitation limits terrestrial water storage, resulting in less continental evaporation, which can cause a reduction in soil moisture and intensify droughts in the northwest part of Australia.


![Correlation Coefficient between SOI and AET Anomalies](https://user-images.githubusercontent.com/114028224/204306992-ecefbc72-8676-4b36-b0f0-b0351874b1ce.png)


![Correlation Coefficient between SOI and Soil Moisture Anomalies](https://user-images.githubusercontent.com/114028224/204307078-6c9a9ecc-7f4d-4682-8fbd-81b73cc66d32.png)

Link: https://github.com/nTavakoli/CLIM680_Project/blob/main/Codes/Linear%20Regression%26Correlation%20Coefficient.ipynb

### Summary

Our results suggest that El Niño conditions are typically associated with negative anomalies of actual evapotranspiration and soil moisture in Australia. Both transpiration and soil evaporation are abnormally low in these regions. On the other hand, positive anomalies in those same regions are characteristic of La Niña conditions. Areas where monthly anomalies of soil moisture are positively correlated to the SOI coincide with regions where AET is typically limited by the supply of water. This explains why we also find positive correlations between AET and SOI in those same regions. These results can also be found in previous studies (Diego G. Miralles et al.)

To sum up, ENSO regulates the total volume of water vapor moving from continental land surfaces into the atmosphere. Terrestrial water shortages, as a consequence of low moisture supplies during El Niño, are the cause of vegetation stress and prolonged declines in AET. However, in the possible El Niño conditions will be intensified in the future, the total flux of water vapor from land to the atmosphere may in fact be progressively reduced. A recent study predicts the highest sensitivity of evapotranspiration to El Niño conditions. Consequences may be in the form of regional reductions in net primary production, water resources, or ecosystem services, and the intensification of feedback from soil moisture on precipitation and temperature.

Investigating the response of ENSO to changes in global radiative forcing, precipitation patterns, and temperature extremes can be done in the future.

### References
W. Dorigo et al., “ESA CCI Soil Moisture for improved Earth system understanding: State-of-the art and future directions,” Remote Sens. Environ., vol. 203, pp. 185–215, 2017, doi: https://doi.org/10.1016/j.rse.2017.07.001.

A. Gruber, T. Scanlon, R. van der Schalie, W. Wagner, and W. Dorigo, “Evolution of the ESA CCI Soil Moisture climate data records and their underlying merging methodology,” Earth Syst. Sci. Data, vol. 11, no. 2, pp. 717–739, 2019, doi: https://doi.org/10.5194/essd-11-717-2019.

A. Gruber, W. A. Dorigo, W. Crow, W. Wagner, “Triple Collocation-Based Merging of Satellite Soil Moisture Retrievals”, IEEE Transactions on Geoscience and Remote Sensing. PP. 1-13, (2017), https://doi.org/10.1109/TGRS.2017.2734070

J. T. Abatzoglou, S. Z. Dobrowski, S. A. Parks, and K. C. Hegewisch, “TerraClimate, a high-resolution global dataset of monthly climate and climatic water balance from 1958-2015,” Sci. Data, vol. 5, pp. 1–12, 2018, doi: 10.1038/sdata.2017.191.


### Acknowledgments
I would like to thank both the CLIM680 instructors Prof. Paul Dirmeyer and Prof. Luis Ortiz Uriarte for coding assistance and answering questions.
