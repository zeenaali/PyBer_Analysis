# PyBer_Analysis
# Project Overview
## Purpose
The purpose of this analysis is to perform data analysis for Ride-Share company PyBer and to tell a compelling story with data visualization. This analysis showcases the relationship between the type of the city -- urban, suburban and rural -- and their correlation between rides, drivers and fares, and congregates data from January to early May of 2019 and focuses on the following:

- The total number of rides for each city type.
- The total number of drivers for each city type.
- The sum of the fares for each city type.
- The average fare per ride for each city type.
- The average fare per driver for each city type.
- The total fares for each week by city type.
 
## Background
The data is gathered in two different CSV files (the city data and the ride data). In this analysis I am using Jupyter notebook and Pandas Library to inspect data, merge datasets, perform calculations an create data series and data frames. In addition to this I am using Python’s plotting library Matplotlib in order to tell visual story and to present complex findings in more informative and engaging way. Data Visualization allows audience to absorb information quickly and detect patterns, trends, correlations and outliers in more effective way.

## Overview the methods and code
**Matplotlib**

Matplotlib is a Python graphing library and offers wide range of graphs, from line plots to 3D plots and it is widely used amongst data analysts. It also has rich styling options and customizable annotations. Matplotlib has two graphing methods: Pandas MATLAB and The object-oriented method. MATLAB plotting is used for quick and simple plots that require little coding, while the object-oriented method is used for more complex graphs, including those with multiple plots on the same graph and require more coding (1).

Besides official Matplotlib documentation, Matplotlib offers many default plot settings that already have integrated many features and require little coding and results in sophisticated graphs. For example, Stylesheets offer a number of default styles with the ability to create and package your own styles. One of them is FiveThiryEight style and it is typified by bold colors, thick lines, and transparent axes (2). Those styles can save us lots of time and coding.

![image](https://user-images.githubusercontent.com/99419112/159200576-c5b6e556-003e-40d8-8057-161d1fa4b9b8.png)
        
    An example of FiveThirtyEight StyleSheet from Matplotlib default plots.
    
## Exploratory data analysis or EDA

EDA is an important step in data analytics. This critical step can save roughly 15–50% of time on a project because it provides a targeted plan for how to clean, sort, and create smaller datasets, that is easier to work with (3). Also, we could describe EDA as in “A first look at the data” and it is used to understand and summarize the content of the dataset, such as initial look at the columns, datatypes, data quality, data statistics and data relationships (4). Besides checking data in "non-graphical" way, it is a good practice to check data "graphically". For example, box and whiskers graph below quickly determine outlier(s), that are harder to determine by "non-graphical" way. Inspecting data quality (missing values, possible duplicates, outliers and other anomalies) it is an important step and can have big impact on the data analysis and the story we want to tell. We can decide how to treat those by including them or omitting them from the further data analysis

![image](https://user-images.githubusercontent.com/99419112/159200712-58e1a9d6-f8bc-4bcf-bf56-7ed76b4d8492.png)

          Determine an outlier(s) with box and whiskers plot.
       
# Resources

- **Data Source:**
  - city_data.csv
  - ride_data.csv
- **Software:**
  - Jupyter Notebook 6.0.3 
- **Environment:**
  - Python 3.7 
- **Dependencies:**
  - Matplotlib Library 3.2.1 
  - Pandas Library 1.0.5 

# Results

From the table The Summary Data Frame per City Type we can see the results for each city type – urban, suburban and rural in correlation to the amount of rides, drivers and fares from January to early May of 2019.

![image](https://user-images.githubusercontent.com/99419112/159200939-df3d6d8b-997c-428e-871f-f17535862092.png)


1. The total number of rides for each city type.

   - The total amount of rides is 2.6-times higher in urban cities than in suburban cities.
   - The total amount of rides is 13-times higher in urban cities than in rural cities.
2. The total number of drivers for each city type.

   - The total amount of drivers is almost 5-times higher in urban cities than in suburban cities.
   - The total amount of drivers is almost 31-times higher in urban cities than in rural cities.
3. The sum of the fares for each city type.

   - The total amount of fares is 2-times higher in urban cities than in suburban cities.
   - The total amount of fares is 9-times higher in urban cities than in rural cities.
4. The average fare per ride for each city type.

   - The average fare per ride is 1.3-times lower in urban cities than in suburban.
   - The average fare per ride is 1.4-times lower in urban cities than in rural cities.
5. The average fare per driver for each city type.

   - The average fare per driver is about 2.4-times lower in urban cities than in suburban cities.
   - The average fare per driver is about 3.3-times lower in urban cities than in rural cities.
6. The total fares for each week by city type.

From the table The Summary Data Frame per City Type we can see the results for each city type – urban, suburban and rural in correlation to the amount of rides, drivers and fares from January to early May of 2019.

![image](https://user-images.githubusercontent.com/99419112/159201072-18202e6a-9a58-495d-85c9-5e8e2ba085ff.png)

- Urban cities have the highest total fares overall. The amount is ranging from the lowest at about $1,600 per week to the highest at about $2,500 per week.
- Rural cities have the lowest total fares overall. The amount is ranging from the lowest at about $250 per week to the highest at about $500 per week.
- Suburban cities fall in between. The total fares amount is ranging from the lowest at about $650 per week to the highest at about $1,450 per week.
- All cities have pretty steady flow of total fares from week to week with a matching spike in the third week in February.

# Summary
The obvious point from the result above is disproportional distribution rides and drivers amongst the city type. Urban cities have much higher number of rides and drivers; however, the average fare per ride and per driver is lower than in suburban and rural cities.

1- Rural cities have the lowest amount of the rides and drivers, yet the ratio ride to driver is the highest (1.6 compare to 0.67 in urban cities). This indicates fewer drivers in rural cities per ride than in the urban cities. Increasing number of drivers could have positive affect on total amount of fares, yet some additional questions need to be answered before making final suggestions.
- Is PyBer profitable in rural cities compare to the suburban and urban cities? Although the sum of total fares is low, it could still be profitable.
- What is the ride count per capita compare to other types of the cities? Lower population could cause low ride and driver count and lower need for PyBer service.
- What is the average length of the ride? High amount of the average fare can be affected by lengthy rides that results in higher average fare per ride.
- How frequently do residents of rural cities use public transportation? Some rural cities might require more PyBer services than others, so focus on increasing service could go to those specific cities.

2- There is a matching peak in third week in February for each city type. Based on this information I would suggest to research this peak in more detail that can help determine what caused the jump. Therefore, the analsis can be used as a business strategy in the future. For example, if the total amount of fares were increased due to certain event, PyBer could use future events for promotion of their services.

3- Urban cities have the highest ride and driver count and the lowest average fare per driver, that is $16.57. I would suggest deeper research on this area by finding out what is the employee satisfaction rate and the company profit on this number (total fare amount is $39,854.38). If employee rate is high and PyBer is profitable, that would indicate a good bussiness strategy for urban cities. In addition, I would suggest to take a closer look into the peaks and dips that appear from late February to early April in order to find out what is causing them. This could reveal important information for future business planning.

In this bussines proposal I have also included scatter plot that includes data per each city within the city type and reads the average fare in correlation to total numbers of rides and drivers per city and city type. The size of the bubbles correlates with the driver count per city. This visualization, besides the obvious disparities among the city types, suggest that looking into each city separetely could reveal important information about specific cities and aid to future bussines strategies.

![image](https://user-images.githubusercontent.com/99419112/159201448-1c03f6fe-1a94-48cf-912e-2471ef3c8341.png)
     
     Ride-Sharing data in correlation to average fare to total number of rides and drivers per city type.
