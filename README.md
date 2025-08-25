# Air_quality_index_capstone






## Table of Contents
* [PowerBI Dashboard](#powerbi-dashboard)
* [Motivation](#motivation)
* [Questions](#questions)
* [Normalizing the Data](#normalizing-the-data)
* [Problems and Hurdles](#problems-and-hurdles)
* [Technologies Used](#technologies-used)
* [Data Sources](#data-sources)
* [Conclusion](#conclusion)


## PowerBI Dashboard
Link:https://app.powerbi.com/reportEmbed?reportId=8b6ea46e-71de-4297-92ec-51b6ae394e72&autoAuth=true&ctid=101da587-1843-4f52-8b8a-17b069c66d33

## Motivation:
Air pollution continues to be a pressing issue in urban areas, directly affecting public health, climate, and overall quality of life. Through this capstone project, I wanted to take the opportunity to research and analyze the Air Quality Index (AQI) across Tennessee and its neighboring states. This region offers a meaningful case study as it brings together rapidly growing urban centers with higher population density and surrounding rural areas with lower density, enabling valuable comparisons of air quality patterns.

## Questions:
1) How has the AQI changed across different years in Tennessee and surrounding states?
2) Which 5 cities have the highest AQI values (worst air quality) and lowest AQI values (best air quality)?
3) How does air pollution vary by season or month in each city
4) Which population categories (small, medium, large cities) show higher AQI levels on maps? 
5) Analysing the correlation between population,density,area and AQI?

## Normalizing the Data

For this project, I collected AirNow datasets for the 1st day of each month from 2019 to 2024 using API calls, stored them as CSV files, and filtered the data to include Tennessee and its neighboring states (GA, AL, MS, AR, NC, SC, VA, MO, KY). Data cleaning involved deriving AQI from the highest pollutant value per city, handling null values, removing spaces with str.strip, and creating additional time-based fields (date, year, month, weekday). AQI categories were assigned based on standard thresholds, and user-defined functions were developed to automate data retrieval and processing.
In addition, population and density data (2019–2024) was retrieved via API, cleaned, and merged with the AirNow dataset to analyze correlations and evaluate how demographic factors influence air quality.

## Problems and Hurdles
The analysis faced several challenges, including large and inconsistent AirNow data, which required selecting only the 1st of each month, missing AQI values that needed cleaning, and combining multiple files that caused alignment issues.It took quite bit of time.

## Technologies Used
1) Python / Pandas - for exploration, normalizing and aggregation of the dataset
2) PowerBI- for creating interactive dashboard
3) canva - for introduction of Project
4) Git - for version control

## Data Sources
To answer the above questions I used the following sources to collect datasets for my analysis

1) Air Quality Data:
 https://files.airnowtech.org/?prefix=airnow

2) Population Data: 
https://www.macrotrends.net/globalmetrics/cities/22922/atlanta/population-scrapped 

34) Population Density Data:  
https://www.governing.com/archive/population-density-land-area-cities-map.html

## Conclusion
The data analysis shows 2020 and early 2021 show lower AQI values — potentially influenced by reduced activity during the COVID-19 pandemic.Summer is the most critical season for air quality management due to consistently higher AQI values.
Winter tends to offer relatively cleaner air, although the degree of improvement varies.High population density does not automatically mean poor air quality.
Other factors such as industrial activity, geography, regulations, and transportation patterns likely play a significant role in AQI outcomes.Population and AQI are essentially uncorrelated.Density might have a small effect on AQI, but it’s weak.
overall tenessese and surrounding cities mostly fall under good and moderate air quality category.
