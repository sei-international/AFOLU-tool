---
title: Adding National Data
permalink: /setup/agriculture/adding-national-data/
layout: default
---

[Previous]({{ '/setup/installation/' | relative_url }})
## Agriculture
### Adding National Data

#### Livestock
In *Current Accounts*, under the *KEY/Agriculture/Livestock/[ANIMAL SPECIES]* branch, update:
-	**N of Livestock:** Add all years for which data is available. Suggested Source: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Stocks, Items: Live Animals).
  -	In the Baseline scenario, develop appropriate projections. In the default-model these follow 10-year historical trends (2011-2020). 
-	**Liveweights:** Adjust liveweights for each animal type based on National Data under *KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE]*-branch. If national data is not available use default IPCC data _(Table 10.A2, Chapter 10, Vol 4, IPCC19R_)
-	**Animal waste management system:** Update fraction of manure managed in each animal waste management system (Lagoon or Liquid Slurry, Solid storage, Drylot, Pasture, Range or Paddock, Daily spread, Digester, Pit <1 month, Pit >1 month, Burned for fuel, Other) for each animal type under *KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE]*-branch. If national data is not available use default IPCC data for your region _(Table 10A.6, Chapter 10, Vol 4, IPCC 19R)_ Check CHECKSUM_AWMS variable for each animal type to make sure all manure is managed.
_Note:_ The variable  _Fraction Burned for Fuel_ under *KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE]*-branch (This will also update fraction fuel used to calculate fraction available for soil application)
  -	If part of manure is used for feed or construction update variables _Fraction Feed_ and _Fraction Construction_ under  *KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE]*-branch
- **Nitrogen and Volatile Solid excretion:** Update _Daily VS Excretion Rate_ and _Daily N Excrecion Rate_- variables to match your regional and climate context with default data provided in _Tables10.13a and  10.19, Vol 4,IPCC 19R_

#### Fertilizer
In *Current Accounts*,  under *KEY/Agriculture/Fertilizer/[FERTILIZER TYPE]*. update the amount of fertilizer applied.
-	**Approach 1**: Enter fertilizers by type from National Statistics or FAO Stat (under Land, Inputs and Sustainability>Inputs>Fertilizer by Product choose Countries: Country in question, Elements: Agricultural Use, Items:  Ammonium nitrate (AN), Ammonium sulphate, Urea and Other where applicable (N content of Other category is assumed at 0.2, update if necessary)).
-	**Approach 2:** Alternatively you can specify, total mineral fertilizer (in amounts of N) and specify amount of urea applied. 
Depending on which approach you use the _Key assumption_-variable of all other fertilizer types should be set to zero (except Urea). Amounts of urea applied always need to be specified, as this variable is used to estimate CO2 emissions from urea. 
-	In the Baseline scenario, develop appropriate projections. In the default-model these follow 10-year historical trends (2011-2020). 

#### Rice cultivation
In *Current Accounts*, under the *KEY/Non-energy/Agriculture/Area rice cultivation*-branch update the area under rice cultivation (_Key assumption_-variable). Add all years for which data is available. 
Suggested Source: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Area Harvested, Items: Crops primary>Rice).
-	In the Baseline scenario, develop appropriate projections. In the default-model these stay constant.
-	Update scaling factors for organic amendment, irrigation scheme during cultivation, and pre cultivation in accordance with national circumstances under *Key\Non Energy\IPCC Emission Factors\EF_rice_cultivation_5_4_19R*-branch *(Tables 5.11 and 5.11A in Chapter 5, Volume 4, IPCC Methods 19R)* 

#### Crops
Under *Current Accounts*, under the *KEY/Non-energy/Agriculture/Crops/[CROP TYPE]*-branch), update
-	**Amount harvested:**  Amount harvested for each crop type under the _Key Assumptions_-variable. Add all years for which data is available.
-	**Area harvested:** Area harvested or under cultivation under the _Area harvested_-variable. Add all years for which data is available.
Suggested Sources: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Area Harvested and Yield, Items: Crops primary>Select all). You can use the variable Dry weight under branch KEY/Non-energy/Agriculture/Crops/Total_Yield dry weight to check whether total yield aligns with national statistics.
*Note: You might need to map crop types reported to the IPCC categories, depending on the disaggregation in country reporting. Make sure all crops in the national statistics are included, and set crop categories not produced in the national context to zero.
-	In the *Baseline* scenario, develop appropriate projections. In the default-model these follow historical trends.
-	If part of crop residue is removed, or slash and burn practices are used, update variables *Slashed and Burnt* and *Fraction removed* under *KEY/Non-energy/Agriculture/Crops/[CROP TYPE]*-branch

#### Other climate and geography dependent variables

Key climate dependent variables that also need to be updated:

**Emission Factors** for
- **Enteric fermentation** under *KEY/Non-energy/IPCC Emission Factors/Chapter10_Vol4_Enteric Fermentation/[ANIMAL SPECIES]* _(Tables 10.10 and 10.11, Chapter 10, Vol 4, IPCC 19R)_
- **Manure management** for specific by manure management system for local climateunder *KEY/Non-energy/IPCC Emission Factors/Chapter10_Vol4_Manure Management/EF_CH4/:[AWMS]* to correspond to local climate _(Table 10.14, Chapter 10, Vol 4, IPCC 19R)_
- **Emission factors for direct N2O emissions from managed soils** under *KEY/Non-energy/IPCC Emission Factors/Chapter11_Vol4_Agricultural Soils*-branch:
  - Emission factor for N additions from synthetic fertilisers, organic amendments and crop residues, and N mineralised from mineral soil as a result of loss of soil carbon _EF1_ for local climate under the _EF1_11_4_19R:Key Assumptions_-variable _(Table 11.1, Chapter 11, Vol 4, IPCC 19R)_
  - Emission factor for flooded rice fields _EF1RF_ for local climate under the _EF1FR_11_4_19R:Key Assumptions_-variable _(Table 11.1, Chapter 11, Vol 4, IPCC 19R)_
  - Emission factor for manure deposited on pastures, and during grazing _EF3PRP_ for cattle (dairy, non-dairy and buffalo), poultry and pigs for local climate under the _EF3PRP_11_4_19R/Cattle poultry and pigs:Key Assumptions_-variable _(Table 11.1, Chapter 11, Vol 4, IPCC 19R)_
- **Emission factors for indirect N2O emissions from managed soils**
  - Emission factor for N volatilisation and re-deposition _EF4_ for climate _(Table 11.3, Chapter 11, Vol 4, IPCC 19R)_


[Next]({{ '/setup/agriculture/calibrating-to-nghgi/' | relative_url }})
