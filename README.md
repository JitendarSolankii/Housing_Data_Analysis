# Housing_Data_Analysis

## California Housing Data Analysis
## Introduction
The California housing dataset provides insights into housing prices in various districts of California, based on the 1990 census. Features such as median house value, median income, total rooms, total bedrooms, population, households, latitude, longitude, and ocean proximity contribute to the dataset's richness. The objective of this analysis is to explore the dataset and answer questions related to housing prices in California.

## Features
Median House Value: continuous
Median Income: continuous
Total Rooms: discrete
Total Bedrooms: discrete
Population: discrete
Households: discrete
Latitude: continuous
Longitude: continuous
Ocean Proximity: nominal
Median Housing Age: discrete

## Data Overview
The dataset consists of 20,640 entries with information on various housing features. It includes both numerical and categorical data. Some entries in the 'total_bedrooms' column contain missing values.

## Data Cleaning
The dataset underwent cleaning to handle missing values. Specifically, the 'total_bedrooms' column was addressed using two methods:

Deletion of Rows: Rows with missing 'total_bedrooms' values were removed.
Imputation with Mean: Missing 'total_bedrooms' values were filled with the mean value of the column.

## Exploratory Data Analysis
## 1. Median Income Distribution
The Kernel Density Estimate (KDE) plot illustrates the distribution of median incomes. The plot shows the density of values at different income levels.

## 2. Housing Median Age Distribution
A distribution plot was created to visualize the spread of housing median ages. This provides insights into the age distribution of houses in California.

## 3. Median Income vs. Median House Values
A scatter plot was used to showcase the relationship between median income and median house values. This visual representation helps identify potential correlations.

## 4. Data Set Operations
Deleting Rows: Rows with missing 'total_bedrooms' values were removed, resulting in a cleaned dataset.
Filling Missing Values: Missing 'total_bedrooms' values were filled with the mean value of the column, creating a dataset with imputed values.

## 5. Create a Dataset by Filling Missing Data with Mean Value
To address missing data in the 'total_bedrooms' column, the mean value of 'total_bedrooms' in the original dataset was calculated and used to fill missing values.

## 6. User-Defined Function for Median Calculation
A user-defined function, calculate_median, was created to calculate the median value of a given dataset or column.

## 7. Latitude vs. Longitude Plot
A scatter plot of latitude vs. longitude was generated to visually represent the geographical distribution of housing locations in California.

## 8. Creating a Dataset with 'Near Ocean' Ocean Proximity
A new dataset was created by filtering entries with 'NEAR OCEAN' in the 'ocean_proximity' column, resulting in a dataset focusing on areas near the ocean.

## 9. Mean and Median of Median Income in 'Near Ocean' Dataset
For the dataset created with 'NEAR OCEAN' ocean proximity, both the mean and median of the 'median_income' column were calculated.

## 10. Creating a Categorical Column for Total Bedroom Size
A new categorical column, 'total_bedroom_size,' was created based on the total number of bedrooms:

'small' for 10 or fewer bedrooms
'medium' for more than 10 but fewer than 1000 bedrooms
'large' for 1000 or more bedrooms
