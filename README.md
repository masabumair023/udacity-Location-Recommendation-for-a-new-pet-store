# Location Recommendation for a new pet store
This project is the part of udacity's Nanodegree program (Predictive Analytics for Business Nanodegree)

## Project Overview
This project is divided into two parts. In the first part, you will blend and format data and deal with outliers.

For the second part, you will use your cleaned up dataset to create another linear regression model. The difference this time is that you will have to choose which variable(s) are the most important for the model using new techniques learned in the Selecting Predictor Variables section.

## Scenario
Pawdacity is a leading pet store chain in Wyoming with 13 stores throughout the state. This year, Pawdacity would like to expand and open a 14th store. Your manager has asked you to perform an analysis to recommend the city for Pawdacity’s newest store, based on predicted yearly sales.

## Skills Required
In order to complete this project, you must be able to:
- Understand different data types.
- Deal with a variety of data issues.
- Format data appropriately.
- Blend data together using joins and unions.

## The Business Problem
Pawdacity is a leading pet store chain in Wyoming with 13 stores throughout the state. This year, Pawdacity would like to expand and open a 14th store. Your manager has asked you to perform an analysis to recommend the city for Pawdacity’s newest store, based on predicted yearly sales.

Your first step in predicting yearly sales is to first format and blend together data from different datasets and deal with outliers.

Your manager has given you the following information to work with:
- The monthly sales data for all of the Pawdacity stores for the year 2010.
- NAICS data on the most current sales of all competitor stores where total sales is equal to 12 months of sales.
- A partially parsed data file that can be used for population numbers.
- Demographic data (Households with individuals under 18, Land Area, Population Density, and Total Families) for each city and county in the state of Wyoming. For people who are unfamiliar with the US city system, a state contains counties and counties contains one or more cities.

## Steps to Success
### Step 1: Business and Data Understanding
Your project should include a description of the key business decisions that need to be made.
### Step 2: Building the Training Set
To properly build the model, and select predictor variables, create a dataset with the following columns:
- City
- 2010 Census Population
- Total Pawdacity Sales
- Households with Under 18
- Land Area
- Population Density
- Total Families
This dataset will be your training set to help you build a regression model in order to predict sales in the Practice Project in the next lesson. Every row should have sales data because we're trying to predict sales.

### Step 3: Dealing with Outliers
Once you have created the dataset, look for outliers and figure out how deal with your outliers. Use the IQR method to determine if there are outlier cities for each of the variables and then justify which city that has at least one outlier value should be removed.
## IQR Steps
To calculate the upper fence and the lower fence, here are the exact steps:

- Calculate 1st quartile Q1 and 3rd quartile Q3 of the dataset. You can use the Excel function QUARTILE.INC or QUARTILE.EXC

- Calculate the Interquartile Range: IQR = Q3 - Q1

- Add 1.5 IQR to Q3 to get the upper fence: Upper Fence = Q3 + 1.5 IQR

- Subtract 1.5 IQR to Q1 to get the lower fence: Lower Fence = Q1 - 1.5 IQR

- Values above the Upper Fence and values below the Lower Fence are outliers

## Data
- p2-2010-pawdacity-monthly-sales.csv - This file contains all of the monthly sales for all Pawdacity stores for 2010.

- p2-partially-parsed-wy-web-scrape.csv - This is a partially parsed data file that can be used for population numbers.

- p2-wy-453910-naics-data.csv - NAICS data on the sales of all competitor stores where total sales is equal to 12 months of sales

- p2-wy-demographic-data.csv - This file contains demographic data for each city and county in Wyoming.
## Author 
[@masabumair](https://github.com/masabumair023)

  
