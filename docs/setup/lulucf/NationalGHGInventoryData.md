---
title: Adding National Data
permalink: /setup/lulucf/calibrating-to-nghgi/
layout: default
---
## LULUCF
# Calibrating to national GHG inventories
In order to make projections consistent with national inventories that have been developed outside of LEAP, the AFOLU tool allows adding the inventory directly to the AFOLU tool and overwriting bottom-up calculations. 

This is done in the *Current Accounts*-scenario under the *Non Energy*-branch. To add your data:
- Select *Current Accounts* from the *Scenarios*-drop down menu
- Add Historical GHG inventory data to the **Historical Inventory** variable under each land use category:
  - Forested Lands
  - Croplands
  - Grasslands
  - Wetlands
  - Settlements
  - Other Lands


If you do not add National GHG Inventory data, the tool will default to bottom-up calculations of GHG emissions based on activity data. Bottom-up calculation will begin in the earliest year for which activity data is available and no inventory data is available. 

**Important** 
1) Data can be added using the Interp() or the Data() function. If using the interp()-function make sure to specify the first year after the last inventory year as 0 , e.g. : 'Interp(2019, 200, 2020, 210, 2021, 0)'
2) If the national GHG inventory was developed using the Stockchange method which only considers net changes in land use area, carbon fluxes from individual land use categories in the AFOLU's tool bottom up modeling will not align with the land uses reported in the national inventories (see section on LULUCF methods and land use conversion matrix). Bottom up results should then be compared to total emissions across the LULUCF sectors.

