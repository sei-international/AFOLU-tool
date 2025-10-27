---
title: Fictional Example
permalink: /setup/lulucf/fictional-example/
layout: default
---
[Previous]({{ '/setup/lulucf/gain-loss-method/' | relative_url }})

### The fictional example in the AFOLU-tool - Overview of Verdania

The fictional example in the AFOLU tool consists of a small country called Verdania with a total land area of *100,000km^2*. Verdania has a temperate cool climate. 
All  major IPCC land categories: Natural forests, plantation forests, croplands, grasslands or pastures, settlements and other lands are present in the 
in the countries territory:

In the first historical year of the land use inventory (2004), land distribution is as follows:
- Natural forests: 35% of the total land area
- Plantation forests: 3% of the total land area
- Croplands: 37% of the total land area
- Grasslands: 15% of the total land area (incl. pastures) 
- Settlements: 3% of the total land area
- Wetlands: 2% of the total land area
- Other lands: 5% of the total land area (includes deserts and heavily degraded lands)

|Year |Total land area | Natural Forest |	Plantation forest |	Cropland |	Grassland |	Settlement |	Wetland |	Other lands |
|-----|                                  km2                                                                              |
|-----|----------------|---------------|--------------------|----------|------------|------------|----------|-------------|
|2004	|     100000     | 	   35000	   |         3000	      |  37000	 |    15000	  |    3000	   |   2000	  |    5000     |

**Over the historical period some key trends have taken place:**

- Urbanisation: Land area covered by settlements has increased from 3% to 5%, this build up has taken place on former croplands
- Severe degradation of croplands: Loss of 5% of croplands between 2004-2023 (these become _Other Lands_)
- Deforestation: 5% of natural forests have been lost and converted to pastures

| Land Use           | 2004 | 2023 |
|--------------------|------|------|
| Natural Forest     | 0.35 | 0.30 |
| Plantation forest  | 0.03 | 0.03 |
| Cropland           | 0.37 | 0.30 |
| Grassland          | 0.15 | 0.20 |
| Settlement         | 0.03 | 0.05 |
| Wetland            | 0.02 | 0.02 |
| Other lands        | 0.05 | 0.10 |  

_Note: The historical period for the LULUCF sector should always cover 20-years of data, no matter what the definition of 
historical period is in your LEAP model. This is necessary, because emission and sequestration estimates of the present years
depend on land use changes that have taken place over the last 20 years._ 

As a result, land use distribution in Virdania in 2023 looks as follows:

|Year |Total land area | Natural Forest |	Plantation forest |	Cropland |	Grassland |	Settlement |	Wetland |	Other lands |
|-----|                                                         km2                                                       |
|-----|----------------|---------------|--------------------|----------|------------|------------|----------|-------------|
|2023	|     100000     | 	   30000	   |         3000	      |  30000	 |    20000	  |    5000	   |   2000	  |    10000    |


Based on these changes, the conversion matrix looks as follows:

| Year | Natural Forest-to-Grasslands (km²) | Croplands-to-Settlements (km²) | Croplands-to-Other Lands (km²) |
|------|------------------------------------|--------------------------------|--------------------------------|
| 2004 |                                    |                                |                                |
| 2005 | 263                                | 105                            | 263                            |
| 2006 | 263                                | 105                            | 263                            |
| 2007 | 263                                | 105                            | 263                            |
| 2008 | 263                                | 105                            | 263                            |
| 2009 | 263                                | 105                            | 263                            |
| 2010 | 263                                | 105                            | 263                            |
| 2011 | 263                                | 105                            | 263                            |
| 2012 | 263                                | 105                            | 263                            |
| 2013 | 263                                | 105                            | 263                            |
| 2014 | 263                                | 105                            | 263                            |
| 2015 | 263                                | 105                            | 263                            |
| 2016 | 263                                | 105                            | 263                            |
| 2017 | 263                                | 105                            | 263                            |
| 2018 | 263                                | 105                            | 263                            |
| 2019 | 263                                | 105                            | 263                            |
| 2020 | 263                                | 105                            | 263                            |
| 2021 | 263                                | 105                            | 263                            |
| 2022 | 263                                | 105                            | 263                            |
| 2023 | 263                                | 105                            | 263                            |

Some key things to note: 
This is an appoximation/major over-simplification:
- a real conversion matrix will likely have many more conversion categories (typical conversions are already set-up in the AFOLU tool, 
less usual conversions might need to be set up by the user)  
- there is usually some year to year variation in the level of land use change, some years no changes take place other years changes might be major like 
in the case of a major drought event

[Nex]({{ '/setup/lulucf/adding-national-data/' | relative_url }})



