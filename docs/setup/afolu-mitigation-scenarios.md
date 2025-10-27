---
title: AFOLU mitigation scenarios
permalink: /setup/afolu-mitigation-scenarios/
layout: default
---

## Developping AFOLU mitigation scenarios

Adding mitigation scenarios makes use of the powerful scenario building capacity in LEAP. LEAP allows to simply add new scenarios, only requires users to update expressions that change in the mitigation scenario, and can the visualize effects of multiple in the _Results_-View. 

To create a new mitigation scenario, simply:
1. Add a new scenario in the _Scenarios_-pane
2. Switch to the new scenario in the _Scenario_drop down menu
3. Edit the expression that describes the change
4. Click on _Results_ to run the model with the new scenario, and visualize results

### Examples of AFOLU mitigation scenarios

**1. Reforestation**  
To increase reforestation, you can simply change the _KEY/LULUCF/Forest Land/Natural Forest Land/Other Land converted to Natural Forest : Key Assumption_ variable with the number of ha you intend to reforest in a given year. Make sure the parameters delta_CG,
_Dead wood stock_new_, and _Litter stock_new_ match your forest type. You can also modify the land use type on which you are planting the new forest (adjust variables _Biomass_old_, _Dead wood stock_new_, and _Litter stock_new_, F_LU_Old_, F_MG_Old and F_I_Old). It is recommended to copy and rename the branch accordingly, before adjusting parameters.

**2. Sustainable agricultural management practice - expanding organic agriculture**  
To expand organic agriculture, you can simply change the _KEY/LULUCF/Cropland/Cropland Organic agriculture/Conventionally Cultivated Land converted to organic agriculture:Key Assumption_ with the number of ha targeted for conversion to organic agriculture. This will increase the amount of carbon stored in the soil (reference variables _F_MG_Old_ and _F_MG_New_ which change from 1.0 to 1.04). A similar approach can be used to model carbon sequestration from expanding no till agriculture or agroforestry. Tables 5.5 (Cropland), Vol 4, IPCC 19R provide default data for different agricultural management practies.

_Note: Users are responsible that the land use changes are internally consistent and do not exceed the area of land actually available for improved land use practices. Users should also make sure that their assumptions are consistent with the total natioanl territory_
