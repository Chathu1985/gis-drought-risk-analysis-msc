# Drought Indices and Formulations

## Standardised Precipitation Index (SPI)
The SPI was calculated to quantify precipitation anomalies over a specified
time scale, using the following formulation:

SPI = (X − μ) / σ

where:
• X is the observed precipitation
• μ is the long-term mean precipitation
• σ is the standard deviation

## Soil Moisture Index (SMI)
The SMI was derived to represent relative soil moisture conditions and is
defined as:

SMI = (SM − SM_min) / (SM_max − SM_min)

where:
• SM is the observed soil moisture
• SM_min and SM_max represent minimum and maximum soil moisture values

## Vegetation Health Index (VHI)

The Vegetation Health Index (VHI) was computed as the average of the Vegetation
Condition Index (VCI) and the Temperature Condition Index (TCI). VCI is derived
from NDVI, while TCI is derived from LST (Ekundayo et al., 2020; Zuhro, Tambunan &
Marko, 2020).

### Vegetation Condition Index (VCI)
\[
VCI = \frac{NDVI_i - NDVI_{min}}{NDVI_{max} - NDVI_{min}} \times 100
\]

### Temperature Condition Index (TCI)
\[
TCI = \frac{LST_{min} - LST_i}{LST_{max} - LST_{min}} \times 100
\]

### Vegetation Health Index (VHI)
\[
VHI = 0.5 \times VCI + 0.5 \times TCI
\]

**Where:**
- \(NDVI_i\): NDVI value for pixel/location \(i\)  
- \(NDVI_{min}, NDVI_{max}\): minimum and maximum NDVI values over the reference period  
- \(LST_i\): LST value for pixel/location \(i\)  
- \(LST_{min}, LST_{max}\): minimum and maximum LST values over the reference period  


## Composite Drought Risk Index
A composite drought risk index was generated using a weighted overlay
approach:

DRI = Σ (wᵢ × Iᵢ)

where:
• Iᵢ represents the standardised drought indicators
• wᵢ denotes the relative weights assigned to each indicator
