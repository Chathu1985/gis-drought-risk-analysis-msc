*© Chathurika Thilakarathna, 2026.  
This repository documents original MSc research work. Shared for academic
and professional reference.*

# GIS-Based Drought Risk Analysis 
*MSc Dissertation: Cloud-based open-source approach for drought risk assessment: Case Study Southeast Asia*


## Study Context
This research was conducted as part of an MSc in Geospatial Science at RMIT University
and focuses on GIS-based drought risk assessment using spatial analysis and remote
sensing techniques.

## My Role & Approach
I designed and implemented a GIS-based drought risk assessment framework by integrating cloud-based remote sensing analysis using Google Earth Engine with desktop GIS and spatial multi-criteria methods. The work involved deriving drought indices, constructing hazard, exposure, and vulnerability components, and generating composite drought risk maps to support regional drought assessment and decision-making.


## Methodological Framework
• Remote sensing and climatic datasets were acquired and preprocessed using
  Google Earth Engine to support large-scale spatiotemporal analysis.

• Key drought-related indicators were derived from environmental and climate variables.

• All indicators were integrated and analysed within desktop GIS environments,
  including ArcGIS Pro and QGIS.

• Indicators were standardised and weighted according to their relative contribution
  to drought risk.

• A GIS-based weighted overlay approach was applied to generate a composite drought
  risk index.

• The resulting index was spatially classified and mapped to identify drought risk
  patterns and vulnerable regions.
  
 
  ## Data Sources
The drought risk assessment utilised multiple publicly available remote sensing and
climate datasets, including precipitation (CHIRPS), drought indices (TerraClimate),
soil moisture (SMAP), vegetation condition (MODIS NDVI), land surface temperature
(MODIS LST), land use/land cover (Copernicus), elevation (SRTM), and population
distribution (WorldPop). Data processing and extraction were primarily conducted
using Google Earth Engine.

 ## Drought indices
  • Drought indices were computed using established formulations (e.g. SPI, SMI),
  with a composite drought risk index derived through weighted integration of
  standardised indicators.
  
[View drought indices and formulations →](methodology/indices.md)


## Key Outputs
• A GIS-based drought risk index integrating multiple climatic and environmental
  indicators.

• Spatial drought risk maps illustrating the distribution of low, moderate, and high
  drought risk across the study area.

• Classification of drought-prone regions to identify spatial patterns of vulnerability.

• Thematic maps designed to support environmental assessment, planning, and resource
  management.



## Selected Spatial Results

### Drought Risk Index Maps

#### Drought Risk Index 2015
![Drought Risk Index Map 2015](figures/Drought_Risk_South_East_Asia_2015.PNG)

#### Drought Risk Index 2020
![Drought Risk Index Map 2020](figures/Drought_Risk_South_East_Asia_2020.PNG)

### Population Density South East Asia
![South East Asia Population Density Map](figures/South_East_Asia_Population_Density_2020.PNG)



## Statistical Analysis

### Distribution of Drought Indicators by Region 2015
![Violin Plot of Drought Indicators](plots/Drought_hazard_density_and_spatial_distribution_across_countries_2015.png)

### Distribution of Drought Indicators by Region 2020
![Violin Plot of Drought Indicators](plots/Drought_hazard_density_and_spatial_distribution_across_countries_2020.png)




