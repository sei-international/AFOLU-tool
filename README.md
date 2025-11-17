# SEI AFOLU Tool

The SEI **Agriculture, Forestry, and Other Land Use (AFOLU) Tool** is designed to assist policymakers and planners in developing medium- and long-term greenhouse gas (GHG) non-energy emission scenarios for agriculture, forestry, and other land uses.

The tool is integrated into the Low Emissions Analysis Platform (LEAP), which is currently used by over 60,000 users to create medium- and long-term energy systems and GHG emission trajectories. Together, LEAP and the AFOLU tool enable the development of internally consistent energy and non-energy GHG emission reduction strategies. By leveraging LEAP's scenario-building capabilities, user-friendly interface and reporting capacity, users can explore different management strategies, facilitating the prioritization of key areas for mitigation action.
The AFOLU tool applies the Tier 1 methodology in the 2019 Refinement to the 2006 IPCC Guidelines for National Greenhouse Gas Inventories to estimate emissions of methane (CH4), carbon dioxide (CO2), and nitrous oxide (NOX) emissions, ensuring that mitigation scenarios align with national GHG inventories and transparency reporting guidelines. 

The tool consists of a LEAP model of non-energy related GHG emissions from agriculture, forestry and land use in a hypothetical country, that can be easily adapted by users to their specific context. Specific instructions instructions can be found on [the tools' gitPages](https://sei-international.github.io/AFOLU-tool/).


## Features

- **GHG Emissions Estimation**  
  The AFOLU tool facilitates the estimation of methane (CH₄), carbon dioxide (CO₂), and nitrous oxide (N₂O) emissions from:
  - Enteric fermentation (CH4)
  - Manure Management (N₂O and CH4)
  - Soil management
    - Direct emissions from application synthetic and organic fertilizers (application of animal manure, crop residues and grazing (N₂O)
    - Indirect emissions from application synthetic and organic fertilizers  due to atmospheric deposition, and leaching and run-off (N₂O)
  - Urea application (CO₂)
  - Rice cultivation (CH4)
  - Wetlands emissions (CO₂ and CH4)
  - Forestry, other land use and land-use change (LULUCF, CO₂)


- **Adaptable Model:**  The tool is distributed as a LEAP model with branches for non-energy-related GHG emissions from agriculture and LULUCF sectors based on the hypothetical country **Verdania** with dry an cool temperate climate and can be easily adapted to specific national geographic and climatic contexts.

- **IPCC-Compliant Methodology:**  The tool employs a combination of Tier 1 and 2 methods from the **2019 Refinement to the 2006 IPCC Guidelines for National Greenhouse Gas Inventories**, ensuring alignment with National GHG inventories and UN Transparency reporting guidelines

- **Scenario-Building Capabilities:**  Leveraging LEAP's advanced scenario-building features, users can explore various management strategies and prioritize key areas for mitigation action.

## Getting Started

### Download  
The AFOLU tool can be downloaded directly from this GitHub repository.  

### How It Works  
1. Install [LEAP](https://leap.sei.org).
2. Download the AFOLU tool from this GitHub repository and install in LEAP
3. Configure the model for your specific national or regional context following the user manual.
4. Build and compare different mitigation scenarios.
   
### Documentation  
A comprehensive [**User Manual**](https://sei-international.github.io/AFOLU-tool/) is included to guide users through:  
- Identifying and adding national data requirements
- Calibrating to existing GHG emission inventories
- Adjusting for context-specific parameters and climate-specific emission factors  

## Contributing  
If you are interested in contributing to the AFOLU tool, please contact Charlotte Wagner.

## License  
This project is licensed under the [Apache 2.0](LICENSE).

## Contributors
[Chris Malley](https://www.sei.org/people/chris-malley/) and [Eve Palmer](https://www.sei.org/people/eve-palmer/)                     -- development of initial excel-based version

[Charlotte Wagner](https://github.com/ccwagner) -- LEAP-tool development

## Contact  
For questions or further information, please reach out to the maintainers via the [Issues](https://github.com/) tab or contact Charlotte Wagner at charlotte.wagner[at]sei.org.
