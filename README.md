# Vaccination saves lives: COVID-19 case study
This case study on COVID-19 was based on [Alex Freberg’s Data Analyst Portfolio Project](https://youtu.be/qfyynHBFOsM?si=NCAmQc_-GDOsZLSz) for SQL and Tableau. After watching the tutorial, I decided to explore the data and do my own case study.  
In this case study, I use SQL notions of **window functions, rolling numbers, extract from date, subqueries, aggregation functions**.

## Business task
**Vaccination saves lives**: how does the rise of vaccination correlate with the number of infections and deaths by COVID-19? 

It is expected that the rise of vaccination will decrease the infection and death rates.

## Data source
**[COVID-19 Data Explorer](https://ourworldindata.org/explorers/coronavirus-data-explorer?zoomToSelection=true&time=2020-03-01..latest&facet=none&country=USA~GBR~CAN~DEU~ITA~IND&pickerSort=asc&pickerMetric=location&Metric=Confirmed+cases&Interval=7-day+rolling+average&Relative+to+Population=true&Color+by+test+positivity=false)** (WHO COVID-19 Dashboard. Geneva: World Health Organization, 2020, dataset downloaded through [ourworldindata.org](ourworldindata.org) contains raw data on confirmed COIVD-19 cases and deaths worldwide.
The data includes data on confirmed cases, deaths, hospitalizations, and testing. This dataset was generated by WHO COVID-19 Dashboard between **January 3rd, 2020** and **August 30th, 2023**.  


## Data exploration

In order to get insights on the data, I need to analyse the datasets and identify the correlation between vaccination and infections and deaths.  
I will explore the following questions:  

- What is the likelihood of being infected and likelihood of dying once infected by country?
- How the infection and deaths numbers changed between January 2020 and December 2022 by country?
- What is the total death count per continent?
- What is the likelihood of dying once infected per continent?
- What is the percentage of population who has recieved at least one COVID-19 vaccine?
- How have the infection and death rates changed after vaccination started?



The data exploration was done using **PostgreSQL**.
The codes I wrote to answer the questions above can be seen [here](https://github.com/marianaobmorais/covid_data_exploration/blob/main/covid_data_exploration.sql).  

**Datasets**:  

I split the COVID-19 dataset into two .csv files in order to perform JOIN functions using SQL: covid_deaths.csv and covid_vaccination.csv (this could have been done with self join too, but since the original dataset has too many rows, I decided to follow Alex Freberg's recommendation and split it into two)

## Visualizations

The data visualization was done using **Tableau**. See the original dashboard here.

**Key findings**:

## A few other questions
