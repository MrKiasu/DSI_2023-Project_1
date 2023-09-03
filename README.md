Project 1: Exploring climate data of Singapore

Project title: Imapact of Climate Change on Energy Cost for Households in Smaller Dwelling Units

### Contact
Github: https://github.com/MrKiasu/

### Problem Statement
Climate change is affecting Singapore in the form of rising temperature and rainfall. How does this impact our electricity consumption? And if so, how much will the cost impact households with lower income? 
This project aims to make recommendations to policymakers in the Singapore Public Service in order to help support households with lower income.

### Datasets
|Filname|Description|Source|
|---|---|---|
rainfall-monthly-total.csv | Monthly total rainfall in Singapore | NEA, https://beta.data.gov.sg/datasets/1399/view
rainfall-monthly-number-of-rain-days.csv | Monthly number of rain days in Singapore | NEA, https://beta.data.gov.sg/datasets/1398/view
relative-humidity-monthly-mean.csv | Average monthly relative humidity in Singapore | NEA, https://beta.data.gov.sg/datasets/1404/view
surface-air-temperature-monthly-mean.csv | Average monthly surface air temperature in Singapore | NEA, https://beta.data.gov.sg/datasets/1419/view
wet-bulb-temperature-hourly.csv | Average hourly wet bulb temperature in Singapore | NEA, https://beta.data.gov.sg/datasets/1423/view
T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type.csv | Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type in Singapore | EMA, https://www.ema.gov.sg/resources/singapore-energy-statistics
T5.1 - Electricity Tariffs.csv | Average monthly electricity tariffs in Singapore | EMA, https://www.ema.gov.sg/resources/singapore-energy-statistics
average-houshold-size-and-income.csv | Average household size and income in Singapore |DOS, https://www.singstat.gov.sg/publications/reference/cop2020/cop2020-sr2/census20_stat_release2


### Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|**year**|*integer*|rainfall-monthly-total|Year| 
|**month**|*integer*|rainfall-monthly-total|Month|
|**total rainfall**|*float*|rainfall-monthly-total|The monthly total rainfall recorded at the Changi Climate Station in mm(millimeters)|
|**rainy_days**|*float*|rainfall-monthly-total|The number of rain days (day with rainfall amount of 0.2mm or more) in a month recorded at the Changi Climate Station.|
|**wet bulb temperature**|*float*|wet-bulb-temperature-hourly|Average of the hourly wet bulb temperature recorded at the Changi Climate Station in degree Celsius|
|**kwh_per_acc**|*float*|T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type|Average Annual Household Electricity Consumption in kilowatt hours|
|**dwelling_type**|*string*|T3.5 - Average Monthly Household Electricity Consumption by Planning Area & Dwelling Type|Type of dwelling units (e.g. 3-room flat)|
|**elect_tariffs**|*float*|T5.1 - Electricity Tariffs|Annual electricity tariffs (weighted average) in cents/kWh|
|**household_income**|*float*|average-houshold-size-and-income|Average household income|
|**household_size**|*float*|average-houshold-size-and-income|Average household size|


### Conclusion
Climate change causes rising temperatures (surface air) and rainfall, leading to higher wet bulb temperature.
With increasing wet bulb temperature, household electricity consumption is expected to increase with the increased use of air conditioning and fans.
It is also found that electricity cost is a higher proportion of income for those staying in smaller dwelling units despite using less electricity.

Therefore, we expect climate change to disproportionally impact those staying in smaller dwelling in terms of electricity cost.


### Recommendation
A three-pronged approach is recommended:
1. To mitgate climate change, long term policies are recommended (e.g. to reduce waste).
2. Electricity tariffs can be scaled such that those who consume more electricity should be charged a higher tariffs.
3. Provide subsidies directly to those staying in smaller dwelling units (1-3 room flats) 


