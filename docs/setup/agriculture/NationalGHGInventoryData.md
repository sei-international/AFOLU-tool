---
title: Adding National Data
permalink: /setup/agriculture/calibrating-to-nghgi/
layout: default
---
## Agriculture
# Calibrating to National GHG Inventory data

In order to make projections consistent with national inventories that have been developed outside of LEAP, the AFOLU tool allows adding the inventory directly to the AFOLU tool and overwriting bottom-up calculations. 

This is done in the *Current Accounts*-scenario under the *Non Energy*-branch. To add your data:
- Select *Current Accounts* from the *Scenarios*-drop down menu
- Add historical GHG inventory data under each relevant category:
  - Enteric Fermentation (CH4 emissions)
  - Rice Cultivation (CH4 emissions)
  - Manure Management (CH4 and N2O emissions)
  - Managed Soils (N2O emissions)
  - Urea Application (CO2 emissions)



If you do not add National GHG Inventory data, the tool will default to bottom-up calculations of GHG emissions based on activity data. Bottom-up calculation will begin in the earliest year for which activity data is available and no inventory data is available. 

#Important# Data can be added using the Interp() or the Data() function. If using the interp()-function make sure to specify the first year after the last inventory year as 0 , e.g. : Interp(2019, 200, 2020, 210, 2021, 0)
