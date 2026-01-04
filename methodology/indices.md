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

## Vegetation Condition Index (VCI)

VCI is calculated as:

VCI = (NDVIᵢ − NDVIₘᵢₙ) / (NDVIₘₐₓ − NDVIₘᵢₙ) × 100


## Temperature Condition Index (TCI)

TCI is calculated as:

TCI = (LSTₘᵢₙ − LSTᵢ) / (LSTₘₐₓ − LSTₘᵢₙ) × 100


## Vegetation Health Index (VHI)

VHI is calculated as the weighted average of VCI and TCI:

VHI = 0.5 × VCI + 0.5 × TCI


### Where:
- NDVIᵢ : NDVI value for pixel/location *i*
- NDVIₘᵢₙ , NDVIₘₐₓ : minimum and maximum NDVI values over the reference period
- LSTᵢ : land surface temperature value for pixel/location *i*
- LSTₘᵢₙ , LSTₘₐₓ : minimum and maximum LST values over the reference period
  

### Normalisation and Composite Indices

Indicator values were normalised using a min–max scaling approach, applying
different formulations depending on whether the relationship with drought
conditions was positive or negative (Ortega-Gaucin et al., 2021).

Positive relationship:
zᵢ = (xᵢ − xₘᵢₙ) / (xₘₐₓ − xₘᵢₙ)

Negative relationship:
zᵢ = (xₘᵢₙ − xᵢ) / (xₘₐₓ − xₘᵢₙ)

The normalised indicators were subsequently aggregated to derive composite
indices, including the Drought Hazard Index (DHI), Drought Exposure Index (DEI),
and Drought Vulnerability Index (DVI), calculated as the mean of the normalised
variables.

## Composite Drought Risk Index
A composite drought risk index was generated using an equal-weighted overlay
approach, where all indicators contributed equally to the final index:

DRI = Σ (wᵢ × Iᵢ)

where:
• Iᵢ represents the standardised drought indicators  
• wᵢ denotes the indicator weights, with equal weights assigned to all indicators
  (wᵢ = 1/n)
