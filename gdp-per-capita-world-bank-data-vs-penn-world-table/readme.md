# GDP per capita: Comparing data from World Bank and Penn World Table - Data package

This data package contains the data that powers the chart ["GDP per capita: Comparing data from World Bank and Penn World Table"](https://ourworldindata.org/grapher/gdp-per-capita-world-bank-data-vs-penn-world-table?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The remaining columns are the data columns, each of which is a time series. If the CSV data is downloaded using the "full data" option, then each column corresponds to one time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data columns are transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

### How we process data at Our World In Data
All data and visualizations on Our World in Data rely on data sourced from one or several original data providers. Preparing this original data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/)

## Detailed information about each time series


## GDP per capita – In constant 2017 international $ – World Bank
This data is adjusted for inflation and for differences in the cost of living between countries.
Last updated: May 20, 2024  
Next update: May 2025  
Date range: 1990–2022  
Unit: international-$ in 2017 prices  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
World Bank (2023) – with minor processing by Our World in Data

#### Full citation
World Bank (2023) – with minor processing by Our World in Data. “GDP per capita – World Bank – In constant 2017 international $” [dataset]. World Bank, “World Bank World Development Indicators” [original data].
Source: World Bank (2023) – with minor processing by Our World In Data

### What you should know about this data
* This GDP per capita indicator provides information on economic growth and income levels from 1990.
* This data is adjusted for inflation and for differences in the cost of living between countries.
* This data is expressed in international-$ at 2017 prices.
* For GDP per capita estimates in the very long run, see the [Maddison Project Database's indicator](https://ourworldindata.org/grapher/gdp-per-capita-maddison).

### How is this data described by its producer - World Bank (2023)?
GDP per capita based on purchasing power parity (PPP). PPP GDP is gross domestic product converted to international dollars using purchasing power parity rates. An international dollar has the same purchasing power over GDP as the U.S. dollar has in the United States. GDP at purchaser's prices is the sum of gross value added by all resident producers in the country plus any product taxes and minus any subsidies not included in the value of the products. It is calculated without making deductions for depreciation of fabricated assets or for depletion and degradation of natural resources. Data are in constant 2017 international dollars.

For the concept and methodology of 2017 PPP, please refer to the [International Comparison Program (ICP)’s website](https://www.worldbank.org/en/programs/icp).

### Source

#### World Bank – World Bank World Development Indicators
Retrieved on: 2023-05-29  
Retrieved from: https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators  


## GDP per capita – Penn World Table
This data is adjusted for inflation and for differences in the cost of living between countries.
Last updated: November 28, 2022  
Next update: December 2024  
Date range: 1950–2019  
Unit: international-$ in 2017 prices  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Feenstra et al. (2015), Penn World Table (2021) – with major processing by Our World in Data

#### Full citation
Feenstra et al. (2015), Penn World Table (2021) – with major processing by Our World in Data. “GDP per capita – Penn World Table” [dataset]. Feenstra et al. (2015), Penn World Table (2021), “Penn World Table” [original data].
Source: Feenstra et al. (2015), Penn World Table (2021) – with major processing by Our World In Data

### What you should know about this data
* This GDP per capita indicator provides information on economic growth and income levels in the medium run. Some country estimates are available as far back as 1950.
* This data is adjusted for inflation and for differences in the cost of living between countries.
* This data is expressed in international-$ at 2017 prices, using multiple benchmark years to adjust for differences in the cost of living between countries over time.
* For GDP per capita estimates in the very long run, see the [Maddison Project Database's indicator](https://ourworldindata.org/grapher/gdp-per-capita-maddison).
* For more up-to-date estimates of GDP per capita, see the [World Bank's indicator](https://ourworldindata.org/grapher/gdp-per-capita-worldbank).

### How is this data described by its producer - Feenstra et al. (2015), Penn World Table (2021)?
Output-side real GDP at chained PPPs (in mil. 2017US$) [From GDP description]

### Source

#### Feenstra et al. (2015), Penn World Table (2021) – Penn World Table
Retrieved on: 2022-11-28  
Retrieved from: https://www.rug.nl/ggdc/productivity/pwt/  

#### Notes on our processing step for this indicator
Estimated as the GDP (output, multiple price benchmarks) divided by the population of each country.

This variable uses ICP PPP benchmarks from multiple years to correct for changing prices over time.

Values for Bermuda have been replaced by estimates on GDP per capita (output, single price benchmark) due to the unusual changes on prices in this country.

Values considered outliers from the original dataset (`i_outlier = "Outlier"`) have been excluded from the dataset, due to implausible relative prices (PPPs divided by exchange rates).



## Population (historical)
Population by country, available from 10,000 BCE to 2023, based on data and estimates from different sources.
Last updated: July 15, 2024  
Next update: July 2026  
Date range: 10000 BCE – 2023 CE  
Unit: people  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World in Data

#### Full citation
HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World in Data. “Population (historical)” [dataset]. PBL Netherlands Environmental Assessment Agency, “History Database of the Global Environment 3.3”; Gapminder, “Population v7”; United Nations, “World Population Prospects”; Gapminder, “Systema Globalis” [original data].
Source: HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World In Data

### What you should know about this data

### Sources

#### PBL Netherlands Environmental Assessment Agency – History Database of the Global Environment
Retrieved on: 2024-01-02  
Retrieved from: https://doi.org/10.24416/UU01-AEZZIT  

#### Gapminder – Population
Retrieved on: 2023-03-31  
Retrieved from: http://gapm.io/dpop  

#### United Nations – World Population Prospects
Retrieved on: 2024-07-11  
Retrieved from: https://population.un.org/wpp/Download/  

#### Gapminder – Systema Globalis
Retrieved on: 2023-03-31  
Retrieved from: https://github.com/open-numbers/ddf--gapminder--systema_globalis  

#### Notes on our processing step for this indicator
The population data is constructed by combining data from multiple sources:

- 10,000 BCE - 1799: Historical estimates by HYDE (v3.3).

- 1800 - 1949: Historical estimates by Gapminder (v7).

- 1950-2023: Population records by the UN World Population Prospects (2024 revision).


## World regions according to OWID
Last updated: January 1, 2023  
Date range: 2023–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Our World in Data – processed by Our World in Data

#### Full citation
Our World in Data – processed by Our World in Data. “World regions according to OWID” [dataset]. Our World in Data, “Regions” [original data].
Source: Our World in Data

### What you should know about this data

### Source

#### Our World in Data – Regions


    