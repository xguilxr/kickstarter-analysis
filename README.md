# Kickstarting with Excel

## Overview of Project

### The purpose of this project was to analyze all the data and break it down in order to use it in our favor. Excel offers many tools for management of information and easy visualization of the results that can also be easily manipulated to provided a wider scope or a more specific and detailed explication. In this project the information provided was that of many films, plays, tv series, and other types of multimedia entertainment. They had information regarding release dates, economic goals, if they were successful, failures or canceled. Using Excel tools all the data was prepared by months and by types to see if there was any type of correlation between dates and success rates.  

## Analysis and Challenges

#### For the interpretation of data two models were used. The first compares outcomes to the launch date to see if the cause came from temporal circumstances. The second one is the outcomes based on goals to see where there is a higher tendency to fail or succeed.  

### Analysis of Outcomes Based on Launch Date

#### This analysis used the Pivot table tool to be able to manipulate the results to enter specific searches. The two main filters were Parent category of the media and the year it was released. The date information was presented in epoch format which had to be converted to be able to use it. Secondly it was necessary to extract the years and months to make the table. The rows of the table were comprised by the extracted months and the columns by the outcomes; successful, failed or canceled. 

![Table of Outcomes based on launch date](/Resources/Theater_Outcomes_vs_Launch.png)   

### Analysis of Outcomes Based on Goals

#### In this analysis the COUNTIFS function was utilized to count using the next sequence of criteria:
1. Goal range (this went from below 1,000 to above 50000, with intervals that ranged 5,000 each. 
2. Outcome (whether they were successful, failed or canceled)
3. Target category and subcategory (in this case theater/plays)

![Table of Outcomes based on Goals](/Resources/Outcomes_vs_Goals.png) 

### Challenges and Difficulties Encountered

#### In the making of both analyses few true difficulties were encountered. Nonetheless, the first trouble found was the date format. The numbers seemed to be just random serial numbers but after converting them from epoch to standard date, everything went more smoothly. Secondly, the Category & Subcategory came as a single entry and for an analysis that took into consideration the main category as a filter it was necessary to extract a part of the string. This was solved by using the LEFT function and using the FIND function to find the "/" character and retrieve the part of the string that belonged to the parent category. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
The first conclusion to draw just from observing the graph presented in the analysis is that the months of May and June present higher chances of having successful outcomes. May and October present the highest threat to releases being the months with highest number of failures. January, March, September, and November have the lowest failures. 


- What can you conclude about the Outcomes based on Goals?
The highest percentage of failures are for plays with goals higher than 45000 while the higher percentage of success are for plays with goals lower than 1000. 

- What are some limitations of this dataset?
One limitation is that there is no insight into time of preparation or production to have a better insight into the preparation and how that affects outcomes. 

- What are some other possible tables and/or graphs that we could create?
A graph of category & subcategory vs. money pledged to see the trend line and make recommendations for future shows and what their goals should be to maximize the probability of success. 
