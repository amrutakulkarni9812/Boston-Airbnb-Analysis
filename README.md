# Boston_Airbnb_Analysis
This repository provides a few interesting insights into Boston Airbnb data.

## Introducing the datasets
Data for analyzing trends in Boston Airbnb is available on [kaggle](https://www.kaggle.com/airbnb/boston).
There are 3 datasets. 
  1. Listings, including full descriptions and average review score 
  2. Reviews, including unique id for each reviewer and detailed comments 
  3. Calendar, including listing id and the price and availability for that day
  
## File Descriptions
### Readme
This file provides high level overview of the work done in project.
### Code
The jupyter notebook available here includes the code required to load, clean, explore and visualize the data and answer the questions.
### Data
1. calendar.csv 
2. listings.csv
3. reviews.csv

## Project Motivation
Motivation behind this project is to answer some of the business questions and to understand the trends if any for future decision making.

### A few questions answered in this project:
1. How some of the features correlate with the pricing?
2. How to get maximum return by investing in right place/type of property?
3. How some of the features correlate with the reviews?

## Data Preparation
This dataset has 3,585 observations and 95 features. The target features for analysis are price, review_scores_rating. To proceed with the analysis, data wrangling should be done as this data set is really messy.

1. I had to clean up the values in several columns: the price column had a dollar sign ($) and comma (,) characters and was in object format. I removed these so the data can be translated into an integer.
2. The data types for other columns like the number of bedrooms, bathrooms, accommodates also required a change so they can be used in calculations.
3. Few columns such as neighbourhood_group_cleansed, jurisdiction_names, license, has_availability were dropped from the dataset as there were no recordings associated with them. These were all empty columns present in the data.
4. City column had a lot of duplicate entries with few case-sensitive entries, space addition issues, etc. All replicates were replaced with a single city code name and this cleaned data was put into a new column called city_cleansed in listings data. 5. City column also had an unusual entry in some native language which was considered for dropping because there was only one entry as such and I was not losing so much data dropping it.

## Results
The main observations of the code are published in this blog here {}.
