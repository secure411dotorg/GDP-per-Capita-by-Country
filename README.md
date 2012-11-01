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

Details of sources for the population and GDP data will be added here shortly.

