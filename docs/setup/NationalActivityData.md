[Previous](Installation.md)
## Update National Activity Data

### Agriculture

Livestock
-	Under Current Accounts, update the number of animals under KEY/Agriculture/Livestock/[ANIMAL SPECIES]. Add all years for which data is available. Suggested Source: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Stocks, Items: Live Animals). 
-	In the Baseline scenario, develop appropriate projections. In the default-model these follow 10-year historical trends (2011-2020). 
-	If part of manure is used for feed, construction or fuel update variables Fraction Feed, Construction under KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE] branch
-	If part of manure is burned for fuel, update variable Fraction Burned for Fuel under KEY/Non-energy/Agriculture/Livestock/[ANIMAL TYPE] branch (This will also update fraction fuel used to calculate fraction available for soil application)

Fertilizer
-	Under Current Accounts, update the amount of fertilizer applied under KEY/Agriculture/Fertilizer/[FERTILIZER TYPE]. Suggested Source: National Statistics or FAO Stat (under Land, Inputs and Sustainability>Inputs>Fertilizer by Product choose Countries: Country in question, Elements: Agricultural Use, Items:  Ammonium nitrate (AN), Ammonium sulphate, Urea and Other where applicable (N content of Other category is assumed at 0.2, update if necessary)). 
-	In the Baseline scenario, develop appropriate projections. In the default-model these follow 10-year historical trends (2011-2020). 

Rice cultivation
-	Under Current Accounts, update the Area under rice cultivation (variable Activity Level variable in the KEY/Non-energy/Agriculture/Area rice cultivation branch). Add all years for which data is available. 
Suggested Source: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Area Harvested, Items: Crops primary>Rice).
-	In the Baseline scenario, develop appropriate projections. In the default-model these stay constant.
-	Update scaling factors for organic amendment, irrigation scheme during cultivation, and pre cultivation in accordance with national circumstances under Key\Non Energy\IPCC Emission Factors\EF_rice_cultivation_5_4_19R branch (Tables 5.11 and 5.11A in Chapter 5, Volume 4, IPCC Methods 19R) 
-	

Crops
-	Under Current Accounts, update the area and amount harvested for each crop type (variables Activity Level and Area harvested in the KEY/Non-energy/Agriculture/Crops/[CROP TYPE] branch). Add all years for which data is available. 
Suggested Source: National Statistics or FAO Stat (under Production>Crops and livestock products choose Countries: Country in question, Elements: Area Harvested and Yield, Items: Crops primary>Select all). You can use the variable Dry weight under branch KEY/Non-energy/Agriculture/Crops/Total_Yield dry weight to check whether total yield aligns with national statistics.
-	In the Baseline scenario, develop appropriate projections. In the default-model these stay constant.
-	If part of crop residue is removed, or slash and burn practices are used, update variables Slashed and Burnt and Fraction removed under KEY/Non-energy/Agriculture/Crops/[CROP TYPE] branch

