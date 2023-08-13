# Bikeshare

Table of Contents

1  Exordium<br>
2  Notebook Configuration<br>
&nbsp;2.1  Packages<br>
&nbsp;2.2  Warning<br>
&nbsp;2.3  Random seed<br>
3  Data Preprocessing<br>
&nbsp;3.1  Data Description<br>
&nbsp;3.2  Loading Capital Bikeshare Data<br>
&nbsp;3.3  Feature Engineering - Dealing with time and date<br>
&nbsp;3.4  Check weather data<br>
&nbsp;3.5  Check missing values<br>
&nbsp;3.6  Drop variables of choice<br>
4  Exploratory analysis<br>
5  Prepare X and y<br>
6  Models selections by comparing the performances between Linear, Ridge, LASSO, Elastic Net, KNN<br>
7  Model selection<br>
8  Conclusion<br>
<br>
Data source:<br>
Capital Bikeshare Data - https://ride.capitalbikeshare.com/system-data<br>
From January to April 2022, including 13 columns and 828,621 rows

Weather Data - https://www.visualcrossing.com/weather-history/washington,%20dc/us/2022-01-01/2022-12-31<br>
From January to December 2022, and includes 33 columns and 365 rows<br>
<br>
Introduction:<br>I'd like to explore the relationship between the demand of the bikeshare station near my school and the weather in Spring 2022, and whether it needs to be further rebalanced based on the forecasted difference of the drop off times and the pick up times in a given day. Here I will not take time series into account.


