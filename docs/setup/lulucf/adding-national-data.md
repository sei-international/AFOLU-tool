---
title: Adding National Data
permalink: /setup/lulucf/adding-national-data/
layout: default
---
[Previous]({{ '/setup/lulucf/fictional-example/' | relative_url }})

## LULUCF
### Adding National Data 


### Land use conversion 
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

Estimated areas subject to land use change can be directly added to the _Key Assumption_-variable under the particular branch (e.g. _KEY/LULUCF/Forested Land/Natural Forest Lands/Other Land converted to Natural Forest: Key Assumption_)

**Projections**  
The land use conversion matrix should not only include historical data, but users should also develop projections based on likely land use change trends. These might be due to human pressures or climate driven pressures, for example historical deforestation and urbanisation trends might be expected to continue at historical rates, and climate driven cropland degradation might be expected to accelerate. When developing mitigation scenarios, actions that will contribute to sequestration, such as reforestation or changes in agricultural croplands that increase both climate resilience and carbon sequestrations, might be excluded from the _Baseline_ scenario so they can be counted towards mitigation potential.
Per default the model is set up such that no land use changes will take place after the first Scenario year unless otherwise specified by the user. This also means that land use changes post 2024 entered into _Current Accounts_ will be ignored unless the user updates the _Baseline_-expressions.

### Data for applying Tier 2 _Gain-Loss_-method for forested lands:
- Natural forests remaining natural forests
- Plantation forests remaining plantation forests
- Wood extractions
  - Fuel wood extractions
    - Coniferous : _KEY/LULUCF/Forested Land/Fuel Wood Extraction coniferous incl bark: Key Assumption_
    - Non-coniferous: _KEY/LULUCF/Forested Land/Fuel Wood Extraction non coniferous incl bark: Key Assumption_
  - Industrial wood extractions
    - Coniferous: _KEY/LULUCF/Forested Land/Industrial Wood Extraction coniferous incl bark: Key Assumption_
    - Non-coniferous: _KEY/LULUCF/Forested Land/Industrial Wood Extraction coniferous incl bark: Key Assumption_
- Fraction wood extraction Natural forest: the remainder will be extracted from Plantation forests
- Area burnt in forest fires: _Forest Land Burnt: Key Assumption_
- Add 20-year lagged values from land converted to forest land to _Natural forests remaining natural forests_ and _Plantation forests remaining plantation forests_ (after 20 years reforested areas are considered forest lands remaining forests). An example can be found under the branch _KEY/Forested Land/Natural Forest/Natural forests remaining natural forests:Key Assumption_ : `ScenarioValue(Current Accounts) + LaggedValue(Other Land converted to Natural Forest, 19)`
 
If national statistics on these data are not available, they can be retrieved from [FAOStat](https://www.fao.org/faostat/en/#data).

### Climate and geography dependent variables 
Key climate dependent variables that need to be updated:  
- KEY\Forested Land\Natural Forest\Natural Forest remaining Natural Forest and KEY\Forested Land\Plantation Forest\Plantation Forest remaining Plantation Forest:
  - Annual biomass growth rates _delta_CG_ (Table 4.9, Chapter 4, Vol 4, IPCC 19R)
  - Root to shoot ratio _Root_shoot Ratio_ (Table 4.4, Chapter 4, Vol 4, IPCC 19R)

- KEY\[LAND USE CATEGORY B]\[Natural or Plantation forest converted to LAND USE B]:
  - Old biomass stock _Biomass_old_ (Table 4.7, Chapter 4, Vol 4, IPCC 19R)
  - Dead wood carbon stocks _Dead wood stock_ (Table 2.2, Chapter 4, Vol 4, IPCC 19R)
  - Litter carbon stocks _Litter stock_old_ (Table 2.2, Chapter 4, Vol 4, IPCC 19R)

- KEY\Cropland\[LAND USE A converted to Cropland]:
  - Adjustment factor for new land use: _LU_new_
  - Adjustment factor for new management practice: _LMG_new_
  - Adjustment factor for new inputs (fertilization practice): _LI_new_
 
- KEY\[LAND USE CATEGORY]\[LAND USE A converted to LAND USE B]:
  - Annual biomass growth rates _delta_CG_ (Tables 5.9 and 6.4, Vol 4, IPCC 19R; Tables 5.1,5.2 IPCC 19R)
  - Reference soil organic carbon stock _SOC_ref_ (Table 2.3, Chapter 4, Vol 4, IPCC 19R, can be specific to land use type)


[Next]({{ '/setup/lulucf/calibrating-to-nghgi/' | relative_url }})
