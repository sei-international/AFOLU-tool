---
title: Fictional Example
permalink: /setup/lulucf/fictional-example/
layout: default
---
[Previous]({{ '/setup/lulucf/gain-loss-method/' | relative_url }})

### The fictional example in the AFOLU-tool - Overview of Verdania

The fictional example in the AFOLU tool consists of a small country called Verdania with a total land area of *1,100,000km^2*. Verdania has a temperate cool climate. 
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

Other lands: 5% of the total land area (includes deserts and heavily degraded lands)

| Year | Total land area (km²) | Natural forest | Plantation forest | Cropland | Grassland | Settlement | Wetland | Other lands |
|-----:|----------------------:|---------------:|------------------:|---------:|----------:|-----------:|--------:|------------:|
| 2004 |             1,000,000 |       350,000  |            30,000 |  370,000 |   150,000 |     30,000 |  20,000 |     50,000  |  


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

| Year | Total land area (km²) | Natural Forest | Plantation forest | Cropland | Grassland | Settlement | Wetland | Other lands |
|------|------------------------|----------------|-------------------|-----------|------------|-------------|----------|--------------|
| 2023 | 1,000,000              |        300,000 |            30,000 |   300,000 |    200,000 |      50,000 |   20,000 |      100,000 |  

Based on these changes, the conversion matrix looks as follows:

| Year | Natural Forest-to-Grasslands (km²) | Croplands-to-Settlements (km²) | Croplands-to-Other Lands (km²) |
|-----:|-----------------------------------:|-------------------------------:|-------------------------------:|
| 2004 |                                    |                                |                                |
| 2005 | 2630                               | 1050                           | 2630                           |
| 2006 | 2630                               | 1050                           | 2630                           |
| 2007 | 2630                               | 1050                           | 2630                           |
| 2008 | 2630                               | 1050                           | 2630                           |
| 2009 | 2630                               | 1050                           | 2630                           |
| 2010 | 2630                               | 1050                           | 2630                           |
| 2011 | 2630                               | 1050                           | 2630                           |
| 2012 | 2630                               | 1050                           | 2630                           |
| 2013 | 2630                               | 1050                           | 2630                           |
| 2014 | 2630                               | 1050                           | 2630                           |
| 2015 | 2630                               | 1050                           | 2630                           |
| 2016 | 2630                               | 1050                           | 2630                           |
| 2017 | 2630                               | 1050                           | 2630                           |
| 2018 | 2630                               | 1050                           | 2630                           |
| 2019 | 2630                               | 1050                           | 2630                           |
| 2020 | 2630                               | 1050                           | 2630                           |
| 2021 | 2630                               | 1050                           | 2630                           |
| 2022 | 2630                               | 1050                           | 2630                           |
| 2023 | 2630                               | 1050                           | 2630                           |  

**Some key things to note:**  
This is an appoximation/major over-simplification of real land use change observed in any given country:
- A real conversion matrix will likely have many more conversion categories (typical conversions are already set-up in the AFOLU tool, 
less usual conversions might need to be set up by the user)  
- There is usually some year to year variation in the level of land use change. Whereas in some years no changes will take place, other years changes might be major like in the case of a major drought event
- Ideally, national experts have access to year-by-year land use conversion data for all land types but this is often not the case. This is an example on how such a simplified matrix can be developed when only land use data and major trends are available. Experts will have to judge which simplifications are acceptable and which might require additional data collection using national experts or analysis of primary data such as satellite data.

[Next]({{ '/setup/lulucf/adding-national-data/' | relative_url }})



