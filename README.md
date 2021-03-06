# Ford GoBike System Data Exploration
#### by Sooyeon Won 

### Keywords 

- Real-World Data Analysis 
- Data Visualisation in Data Analysis 
- Univariate, Bivariate, Multivariate Exploration of Data 
- Explanatory Visualisations 


## Introduction

As a project of _Data Visualization_ in [Nanodegree Program for Data Analyst (Udacity)](https://www.udacity.com/course/data-analyst-nanodegree--nd002), I investigated mobility patterns of rental bikes. The data, provided by ['Ford GoBike System'](https://www.lyft.com/bikes/bay-wheels/system-data) contains time, place, and user information of each bike trip since 2017. In this analysis, I used the data collected from 2018 to 2019. Both years include all datapoints from January to December. Since the monthly datasets are initially provided, they are all aggregated before the data exploration stage. You can see how the monthly datasets are appended in "01_Data Wrangling 2018-2019.html". The final dataset includes more than 4 million datapoints. 
<br>

## Summary of Findings

1. General Mobility Patterns <br>
In general, many people use a rental bike less than 15 minutes within the distance of 2.14km. This pattern is consistent over the years. The distributions of trip durations and trip distance are remarkably similar in each year. The overall number of trips increased over the years. This indicates that Ford GoBike shows promising business in 2019, comparing to the previous years. More people rent a bike when the weather is warm (from July to October). Higher demands are shown on weekdays, rather than weekends. Moreover, users more rent a bike during rush hours.
<br><br>
2. Pattern Comparisons based on User Type <br>
There are two types of rental bike users in Ford GoBike dataset: Subscribers and Customers. More than 80 percent of all travel records are generated by "Subscriber" type of users. Both types of users access to the rental bike system mostly through their mobile applications. The number of trips that both subscribers and customers rent a bike are increased from 2018 to 2019. However, the two user groups also show different mobility patterns. The average trip duration of customer user type is longer than that of subscriber user type. Comparing to the users in customer group, more users in subscriber group have similar patterns of mobility.
<br><br>
3. Pattern Comparisons based on User Type under the different Time Dimensions <br>
    - **Monthly-based Analysis** 
The number of trips that subscribe group monthly takes is much more than that of customer group. The average monthly trip duration of subscribers are ca. 600 seconds (10 minutes), and these durations are very similar across all months. The average time duration of customers in a month are much longer than that of subscribers. <br>
    - **Weekly-based Analysis**
The users in subscribe group mostly rent a bike during weekdays. The number of trips in subscribe group on weekends is far less than on weekdays. For these reasons, I guess the most subscriber group has the characteristic of commuters, who regularly need a rental bike as the means of transportation for a certain distance to move from one place to another. On the other hand, there is almost no variation on the number of trips in customer groups. As before, the average trip duration of subscribers is less than that of customers. The customers are more likely ride a bike for a longer time on weekends. <br>
    - **Hourly-based Analysis** 
The subscribers show high demands during the rush hours of day. On the other hand, customers use the rental bikes in the afternoon rather than in the morning. The trip durations of subscriber group are similar over the hours.
<br>

## Key Insights for Presentation

This analysis mainly investigates about the mobility patterns of the rental bikes records. The patterns are explored using univariate, bivariate and multivariate visualizations. The visualizations will help you understand the mobility patterns of rental bike users with different time perspectives. 
<br>

## References 
- [For distance calculation](https://stackoverflow.com/questions/40452759/pandas-latitude-longitude-to-distance-between-successive-rows) <br>
- [seaborn.barplot](https://seaborn.pydata.org/generated/seaborn.barplot.html)<br>
- [seaborn.heatmap](https://seaborn.pydata.org/generated/seaborn.heatmap.html)<br>
