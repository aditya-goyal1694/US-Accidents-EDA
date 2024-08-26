# US-Accidents EDA
This project explores the US-Accidents dataset from Kaggle, performing exploratory data analysis (EDA) to uncover patterns and insights related to traffic accidents in the United States.

## Dataset Information
Source: Kaggle
The dataset contains 7.7 M records.
Note: This dataset does not contain data for New York, which is the most populated city in the U.S.
Downloading the Dataset
To download the dataset, use the Kaggle API key. If you haven't set up the Kaggle API, follow these steps:

## Downloading Dataset
**Install Kaggle CLI:** pip install opendatasets
Place your Kaggle API key in the appropriate location (usually ~/.kaggle/kaggle.json).

**Download the dataset using the following command:**
bash

Copy code

import opendatasets as od

url='https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents'

od.download(url, force=True)


## Ask and Answer Questions
In this analysis, several key questions were addressed:

1. Are there more accidents in warmer or colder areas?
2. Which 5 states have the highest number of accidents?
3. Does New York show up in the data? If yes, why is the count low considering it's the most populated city?
4. What time of the day are accidents more frequent?
5. Which days of the week have the most accidents?
6. Which months have the most accidents?
7. Is the distribution of accidents by hour the same on weekends as on weekdays?


## Summary and Conclusion
### Key Insights:
1. No data for New York: Despite being the most populated city, New York is absent from the dataset.
2. Accident Distribution: The number of accidents per city decreases exponentially.
3. Top Cities with Most Accidents: Miami, Houston, Los Angeles, Charlotte, and Dallas are the top 5 cities with the highest number of accidents.
4. Accident Frequency: Less than 9% of cities have reported more than 1000 accidents, and over 1000 cities have reported only one accident, warranting further investigation.
5. Peak Accident Hours: A significant percentage of accidents occur between 6 am to 8 pm, with extreme peaks between 7 am to 9 am and 3 pm to 6 pm.
6. Weekday vs. Weekend: Accidents are less frequent on weekends. On Sundays, the peak hours are between 11 am and 8 pm, unlike the weekday patterns.
7. Geographical Patterns: Accidents are more common in coastal areas and comparatively less in the central regions of the U.S.

## Areas for Future Work:
1. Accidents per Unit of Traffic: Identify when accidents per unit of traffic are the highest.
2. Year-over-Year Trend: Analyze whether the number of accidents is increasing or decreasing over the years.
3. Accidents per Capita: Determine the 5 states with the most accidents per capita.
4. Top 100 Cities Analysis: Identify the states most frequently represented among the top 100 cities in terms of accident numbers.

## Libraries Used
1. pandas: For data manipulation and analysis.
2. seaborn: For data visualization.
3. folium: For geospatial data visualization.
4. opendatasets: For easy dataset downloading from Kaggle.
