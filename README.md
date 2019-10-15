![Alt text](http://massrealestatelawblog.com/wp-content/uploads/sites/9/2018/11/cropped-airbnbjpg-daa5146c722ed3c1.jpg?raw=true "Boston Airbnb")
# Boston_Airbnb_Analysis
This repository provides a few interesting insights into Boston Airbnb data.
## Introducing the datasets
Data for analyzing trends in Boston Airbnb is available on [kaggle](https://www.kaggle.com/airbnb/boston).
There are 3 datasets. 
  1. Listings, including full descriptions and average review score 
  2. Reviews, including unique id for each reviewer and detailed comments 
  3. Calendar, including listing id and the price and availability for that day
## File Description
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
1. How is price fluctuating over time?
2. How some of the features correlate with the pricing?
3. How to get maximum return by investing in right place/type of property?
4. How some of the features correlate with the reviews?
5. What do home owners emphasize in their descriptions?
6. What are most important things to tenants?
## Data Preparation
This being a real world dataset, requires some data cleaning and wrangling.
1. In order to compute average price with respect to other features, I needed to convert it to float and remove special characters from it.
2. In order to create a year-month column, I needed to convert date column to datetime type and extract only years and months.
3. I converted a few columns to integer for numerical analysis. e.g. number of bedrooms, number of bathrooms etc.
4. I removed the columns with all null values, since they don't provide any information. e.g. neighbourhood_group_cleansed, jurisdiction_names, license, has_availability.
5. I cleaned the city column by cleaning upper case and lower case, spaces, special characters and standardizing them. City column also had one unusual entry in asian script '波士顿' which I dropped. 
## Results
The main observations of the code are published in this blog [on medium.com](https://medium.com/@amrutakulkarni9812/boston-airbnb-analysis-90564e8a44fb?sk=dacbfd0d9cd59060215de3bc7ed3b938).
