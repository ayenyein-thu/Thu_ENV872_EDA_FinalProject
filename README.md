# The Impact of Institutions on Economic Growth, Development and Poverty

## ENVIRON 872: Final Project (Fall 2024)

## Summary

This repository contains the study submitted to fulfill the requirements of the course titled “Environmental Data Exploration (ENVIRON 872)” offered by the Nicholas School of the Environment, Duke University. The dataset used in this study is compiled from seven publicly available sources. The study analyzes the impact of political and economic institutions on poverty, economic growth, and development. It covers data from 133 countries over the period between 2000 and 2021. To analyze the relationships between institutions and development outcomes, the study employs both a linear model and a fixed effects regression model. The findings contribute to understanding the role of governance and economic freedom in shaping poverty reduction, growth, and overall development across different nations.

## Investigator

-   Aye Nyein Thu, [ayenyein.thu\@duke.edu](mailto:ayenyein.thu@duke.edu){.email}

## Keywords

Institutions, Governance, Economic Freedom, Poverty, Growth, Development

## Database Information

All the data were accessed between 16th and 19th November 2024 from the below-mentioned data sources. All the downloaded datasets are uploaded in the Data/Raw folder with making any. The dataset processed and updated by the author are saved in the Data/Processed folder.

| Variable Names                                               | Column Names      | Units                                             | Data Sources                                       |
|---------------------|----------------|------------------|-------------------|
| Poverty Headcount                                            | Poverty.Headcount | \% of Population                                  | World Bank's Poverty and Inequality Platform (PIP) |
| Human Development Index                                      | HDI               | Score ranging from 0 (lowest) to 1 (highest)      | United Nations Development Programme (UNDP)        |
| Gross Domestic Product (GDP) per capita (Constant 2015 US\$) | GDP.Capita        | USD                                               | World Bank's World Development Indicators (WDI)    |
| Governance                                                   | Governance        | Score ranging from -2.5 (lowest) to 2.5 (highest) | World Bank's World Development Indicators (WDI)    |
| Economic Freedom                                             | Econ.Freedom      | Score ranging from 0 (lowest) to 10 (highest)     | Fraser Institute (FI)                              |
| Government Expenditure                                       | Gov.Expense       | \% of GDP                                         | World Bank's World Development Indicators (WDI)    |
| Population                                                   | Population        | No. of People                                     | World Bank's World Development Indicators (WDI)    |
| Landlocked                                                   | Lanlocked         | 0(not landlocked) or 1 (landlocked)               | CEPII                                              |
| Area                                                         | Area              | Square kilometers                                 | CEPII                                              |

## Folder Structure, File Formats, and Naming Conventions

This repository contains three main folders: Code, Data, and Output. Each folder is organized to ensure easy navigation and reproducibility of the analysis.

-   Code: This folder contains separate code files for data exploration, data analysis, and a combined code file that includes all the analysis steps.
-   Data: The Data folder is divided into two subfolders:
    -   Raw: This folder contains the original datasets downloaded from various sources without any modifications.
    -   Processed: This folder contains the datasets that have been processed, cleaned, and updated by the author for analysis.
-   Output: This folder includes the final project in both Rmd and HTML formats, along with the plots generated during the analysis, stored as PNG files.

## Metadata

Files saved in the Raw folder contains 7 datasets as follow:

**CEPII_GeogrphicClassification.csv**

-   Information: Contains geographic information such as country names, country codes, continent, area, latitude, and longitude.

-   Data Source: CEPII

-   Data Link: <https://www.cepii.fr/CEPII/fr/bdd_modele/bdd_modele_item.asp?id=41>

**FI_EconomicFeedom.csv**

-   Information: Contains an economic freedom index in 5 key different areas and their sub-areas.

-   Data Source: Fraser Institute (FI)

-   Data Link: <https://efotw.org/economic-freedom/dataset?geozone=world&year=2022&page=dataset&min-year=2&max-year=0&filter=0>

**UNDP_HDI.csv**

-   Information: Contains human development index scores for each country from 1990 to 2022.

-   Data Source: United Nations Development Programme (UNDP)

-   Data Link: <https://hdr.undp.org/data-center/documentation-and-downloads>

**WB_CountriesClassification_2024.csv**

-   Information: Contains the World Bank’s classification of countries by income and regional groups.

-   Data Source: World Bank

-   Data Link: <https://datahelpdesk.worldbank.org/knowledgebase/articles/906519-world-bank-country-and-lending-groups>

**WB_PovertyInequalityPlatform.csv**

-   Information: Contains different measures of poverty and inequality.

-   Data Source: World Bank's Poverty and Inequality Platform (PIP)

-   Data Link: <https://pip.worldbank.org/poverty-calculator>s

**WB_WorldGovernance.csv**

-   Information: Contains governance indicators in 6 different dimensions.   

-   Data Source: World Bank's Worldwide Governance Indicators

-   Data Link: <https://www.worldbank.org/en/publication/worldwide-governance-indicators>

**WDI_GrowthPopulation.csv**

-   Information: Contains economic growth, expenditure, and population.

-   Data Source: World Bank's World Development Indicators (WDI)

-   Data Link: <https://databank.worldbank.org/source/world-development-indicators>

## Scripts and Code

The raw files above are cleaned and changed to longitudinal/panel data format. Then, all of them are combined and saved in the Data/Processed folder.

1.  Combined.csv file combines all the 7 processed datasets.

2.  Combined_CommonYear.csv file filters the year from 1996 to 2021 that is common across all the datasets.

3.  Combined_dropNA.csv file removes all the missing values in the dataset, and this file is used for further analysis.

## Quality assurance/quality control

The study uses the simple statistical tools, linear and fixed effects models, to analyze the relationship between institutions and poverty, growth, and development. The outliers are not removed and missing values are not interpolated. The further studies using different and advanced analysis tools are suggested for robustness.
