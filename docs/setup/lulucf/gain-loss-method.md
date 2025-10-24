---
title: The Gain-Loss Method
permalink: /setup/lulucf/gain-loss-method/
layout: default
---
[Previous]({{/setup/agriculture/calibrating-to-nghgi/' | relative_url }})
## LULUCF
### General approach and the Gain-Loss-method

The Land Use, Land-Use Change, and Forestry (LULUCF)-component of the AFOLU tool tracks emissions from each of the key IPCC land use categories, namely:
- Forest
- Cropland
- Grassland
- Wetlands
- Settlements
- Other Land

The AFOLU-tool applies the _Gain–Loss_-method rather than the _Stockchange_-method typically used in National GHG Inventories that apply Tier 1 methods. The key benefit of this approach is that gross emissions and sequestration associated with land use changes as well as management practices can be accounted for, which is key for quantifying mitigation benefits, whereas the Stockchange Method, which is based on the land area remaining within a land category, will only track net changes in land area and average carbon stocks by land use type. The _Gain-Loss_-method on the other hand allows tracking carbon fluxes of gross changes not only due to land use changes, but also due to changes in management practices within a certain land use category across three carbon pools: 

1) (Above and below ground) biomass, 
2) Dead organic matter, and
3) Soil carbon

Biomass losses due to land conversions are accounted for in the same year, whereas carbon changes in dead organic matter and soils will accrue over a 20-year transition period, corresponding to reequilibration time to a new steady state of the disturbed carbon pool. The exception are biomass pools on conventionally farmed agricultural land, which are assumed to grow within a single year consistent with annual cropping.

Changes in carbon pools from a specific land use change are tracked in the land use type to which the conversion takes place, e.g. carbon sequestration in reforested land is tracked under _Forested lands_, carbon releases from forested lands converted to pastures are tracked under _Grasslands_.

#### Developing a land use conversion matrix

Applying the _Gain-Loss_ method requires knowledge of land conversions between the key land categories that have taken place over the last 20 years in order to estimate present day emissions/sequestrations from the LULUCF sector. This requires developing a land conversion matrix that tracks gross changes between the major land categories over the past 20-years.

Forested land | Cropland-to-Forest | Grassland-to-Forest | ... | Cropland | Forest-to-Cropland | Grassland-to-Cropland | ...



|           | Forest land                 | Cropland-to-Forest | Grassland-to-Forest | … | Cropland                    | Forest-to-Cropland | Grassland-to-Cropland | … | Total national area         |
| --------- | --------------------------- | ------------------ | ------------------- | - | --------------------------- | ------------------ | --------------------- | - | --------------------------- |
| 2000 | [fill]                      | [fill]             | [fill]              | … | [fill]                      | [fill]             | [fill]                | … | [fill]                      |
| 2001 | [fill]                      | [fill]             | [fill]              | … | [fill]                      | [fill]             | [fill]                | … | [fill]   


Two major approaches are commonly been used to develop such a land conversion matrix.
- **Approach 1** uses national land and forest cadasters that collect data on the area of land use over time, supplemented by historical time series on key land conversions such as deforestation and refforestation, land degradation. Expert judgement is used to develop likely historical conversion scenarios that explain the observed land use inventory, f.e. defforested land may primarily be converted to cropland, cropland area lost may be victim to settlement pressures or land degradation etc. The conversion matrix should align with the land use inventory and total area of land withing the geographic boundary needs to be respected. It is recommended that experts developing the conversion matrix clearly identify and justify their assumptions and choices. If national data is not available, time series of land areas under specific uses can be retrieved from FAOStat.

- **Approach 2**

[Next]({{/setup/lulucf/adding-national-data/' | relative_url }})
