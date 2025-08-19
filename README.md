
## Introduction
This repository contains the data for assessing global trends in financial inclusion before and after the COVID-19 pandemic with a specific focus on Mexico, Canada, and the United States. These countries are members of the USCMA commercial agreement. And the main objective is to analyze how was their performance during the pandemic.
The primary data sources is:

- [The World Bank’s Global Findex Database](https://databank.worldbank.org/databases)

The secondary data sources are: 

- [Macroeconomic indicators from the World Bank API](https://documents.worldbank.org/en/publication/documents-reports/api)

- [Geospatial data from The North American Cartographic Information Society (NACIS)](https://www.naturalearthdata.com)

---

## Data Structure
### Directories
- `raw_data/`: Contains raw data collected directly from the online sources, including:
  - `findex_data/`: Global Findex indicators from 2011 to 2022
  - `API_data/`: Macroeconomic indicators retrieved from the World Bank API for the USMCA countries
  - `shape_data/`: Geospatial shapefiles for visualizing data globally

- `processed_data/`: Contains cleaned and transformed datasets for analysis.

-  `outputs/`: Contains graphics for the analysis.

### The transformed datasets are the following: 
- `processed_data/`:
  - `all_indicators.csv`: Combined dataset of Findex indicators and macroeconomic variables
  - `USMCA_indicators.csv`: Macroeconomic variables for USMCA countries from 2011 to 2022
  - `findex_indicators_long.csv`: Financial inclusion indicators for all countries from 2011 to 2022 



## Transformations
After reshaping data from wide to long format for time series analysis, five transformations were performed on the combined dataset:

1. Calculating GDP growth

2. Creating a categorical variable for pre and post COVID-19

3. Calculating the amount of government expenditure in education

4. Calculating gender gap: difference between male and female account ownership

5. Normalizing inflation rates for comparative analysis



## Outputs
1. Global map in financial inclusion for 2017 and 2021/2022

2. Trends in borrowing and inflation for USMCA

3. Gender gap in account ownership for USMCA

4. Main trends for account ownership, savings and borrowings


## How to Use
To reproduce this analysis:

1. Clone this repository. 

2. Run the script