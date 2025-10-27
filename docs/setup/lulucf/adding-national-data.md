---
title: Adding National Data
permalink: /setup/lulucf/adding-national-data/
layout: default
---
[Previous]({{ '/setup/lulucf/fictional-example/' | relative_url }})

## LULUCF
### Adding National Data 

* under construction*

## Land use conversion 
Once the land use conversion matrix described in the previous section has been developed by the national experts, the data can be directly added to the model. The structure, and calculations for the majority of typical land use conversions such as re- and deforestation, urbanisation, expansion of pastures, and severe degradation of pastures are already established in the sample 
model and only require filling land areas undergoing land use chage (_Key Assumption_ variable) as well as updating certain parameters that are specific to the national context and the local climate.

Major land use conversions already in the model include:

Natural forests:  
- _Other Land_ converted to _Natural Forest_  

Cropland:  
- _Grassland_ converted to _Cropland_  
- _Other Land_ converted to _Cropland_  

Grassland:
- _Other Land_ converted to _Grassland_  

Settlements:  
- _Cropland_ converted to _Settlements_  
- _Grassland_ converted to _Settlements_  
- _Other Land_ converted to _Settlements_  

Other lands:  
- _Plantation Forest_ converted to _Other Land_  
- _Cropland_ converted to _Other Land_  
- _Wetland_ converted to _Other Land_  
- _Grassland_ converted to _Other Land_  
- _Cropland_ converted to _Other Land_

Estimated areas subject to land use change can be directly added to the _Key Assumption_-variable under the particular branch (e.g. _AFOLU tool/KEY/LULUCF/Natural forest/Other Land converted to Natural Forest: Key Assumption_)

**Projections**  
The land use conversion matrix should not only include historical data, but users should also develop projections based on likely land use change trends. These might be due to human pressures or climate driven pressures, for example historical deforestation and urbanisation trends might be expected to continue at historical rates, and climate driven cropland degradation might be expected to accelerate. When developing mitigation scenarios, actions that will contribute to sequestration, such as reforestation or changes in agricultural croplands that increase both climate resilience and carbon sequestrations, might be excluded from the _Baseline_ scenario so they can be counted towards mitigation potential.
Users need to make sure that land use changes specified in _Baseline_-scenario are set to zero if no future trend is expected, otherwise the model will default to the last value in _Current Accounts_.

## Data for applying Tier 2 _Gain-Loss_-method for forested lands:
- Natural forests remaining natural forests
- Plantation forests remaining plantation forests
- Fuel wood extractions
  - Coniferous
  - Non-confierous
- Industrial wood extractions
  - Coniferous
  - Non-confierous
 
If national statistics on these data are not available, they can be retrieved from [FAOStat](https://www.fao.org/faostat/en/#data).

## Climate dependent variables 


[Next]({{ '/setup/lulucf/calibrating-to-nghgi/' | relative_url }})
