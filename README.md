GDP-per-Capita-by-Country
=========================

Data and scripts used to relate a datapoint to the GDP and population of a country

COLUMNS
***

```
US|14586736|313759000|21410|2.17142714897758444175

Country Code
GDP in Geary-Khamis dollars / 1,000,000
Population
Global median GDP per capita in Geary-Khamis dollars 
Ratio of this country's GDP per capita to the global median GDP per capita
```

The ratio in the last column is the result of:

```
echo "scale=20;((${GDP}*1000000)/${POPULATION})/${GLOBALMEDIANGDPPERCAPITA}"|/usr/bin/bc
```

Sources of Population Data
***

    Computer parseable population figures correlated to the ISO-3166-2 country code list are maintained by Dissect Cyber Inc and are sourced from http://en.wikipedia.org/wiki/List_of_countries_by_population. As noted on the Wikipedia page, original sources include Official Census, Official Estimate, UN Estimates, et al. While many are from 2012, some are from previous years. 

Sources of GDP per Capita Data
***

    Computer parseable GDP figures correlated to the ISO-3166-2 country code list are maintained by Dissect Cyber Inc and are sourced from http://databank.worldbank.org/databank/download/GDP_PPP.pdf if a PPP (Purchasing Power Parity) figure is available, and sourced from http://databank.worldbank.org/databank/download/GDP.pdf if not available in PPP form. 

    Purchasing Power Parity (described here: http://en.wikipedia.org/wiki/Purchasing_power_parity) is related to how much money would be needed to purchase the same goods and services in two countries. PPP makes use of the "international dollar" or Geary-Khamis dollar described here: http://en.wikipedia.org/wiki/Geary%E2%80%93Khamis_dollar. 

    Different data sources offer different estimates of GDP and GDP (PPP) for the same countries, as illustrated here http://en.wikipedia.org/wiki/List_of_countries_by_GDP_%28PPP%29_per_capita. GDP per capita rank by the CIA World Factbook is compared to similar data from the International Monetary Fund and the World Bank. Again the year the statistic was tabulated for each country varies. Most, particularly the larger or more developed countries tend to have more recent dates. Dissect Cyber Inc calculates GDP per capita by taking the GDP (PPP where available) and dividing by the population figure. 



