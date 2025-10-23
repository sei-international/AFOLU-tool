---
title: Model Description
permalink: /model-description/
layout: default
---

[Previous]({{ '/index/' | relative_url }}

## Model Description

The AFOLU tool adopts a bottom-up, sector-specific approach to estimate baseline greenhouse gas emissions  agriculture, forestry, and other land use (AFOLU) sectors. The model structure and emission calculations are aligned with the 2019 Refinement to the 2006 IPCC Guidelines for National Greenhouse Gas Inventories, applying a combination of Tier 1 and Tier 2 methodologies.

The following **AFOLU sectors** are included:

- Methane emissions from enteric fermentation *(Tier 1)*
- Methane and nitrous oxide emissions from manure management *(Tier 1)*
- Nitrous oxide emissions from agricultural soil management *(Tier 1)*
- Methane emission from rice cultivation
- Carbon dioxide emissions from urea application *(Tier 1)*
- Carbon dioxide emissions from Land Use, Land-Use Change, and Forestry (LULUCF):  
  The *Gain–Loss* method is applied to enable tracking emissions and sequestration from changes in land use and management practices. For forested lands, Tier 2 methods are applied, which is essential to account for biomass accumulation as well the impacts of overexploitation on total carbon storage in natural and plantation forests. For all other land use categories, Tier 1 methods are used. 
- Methane emissions from wetlands *(Tier 1)*

  
To facilitate updating context dependent parameters, the model is set up such that all national data, and parameters are stored under key assumptions.

Final emission calculations for each relevant subcategory takes place under the non-energy branch, and can be displayed in LEAP's Results-View.


[Next]({{ '/setup/setup/' | relative_url }}
