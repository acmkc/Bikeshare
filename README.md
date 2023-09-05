<html>
<head>
<meta charset="UTF-8">
</head>
<body>
  <p>
 
&#128204;&nbsp;&nbsp;Table of Contents

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
&#128204;&nbsp;&nbsp;Data source:<br>
Capital Bikeshare Data - https://ride.capitalbikeshare.com/system-data<br>
From January to April 2022, including 13 columns and 828,621 rows

Weather Data - https://www.visualcrossing.com/weather-history/washington,%20dc/us/2022-01-01/2022-12-31<br>
From January to December 2022, and includes 33 columns and 365 rows<br>
<br>
&#128204;&nbsp;&nbsp;Data description:<br>
<table>
    <tr>
        <th>Features</th>
        <th></th>
    </tr>
    <tr>
        <td>ride_id</td>
        <td>Bike number</td>
    </tr>
    <tr>
        <td>rideable_type</td>
        <td>The types of bike, including classic_bike, electric_bike, docked_bike</td>
    </tr>
    <tr>
        <td>started_at</td>
        <td>Includes start date and time</td>
    </tr>
    <tr>
        <td>ended_at</td>
        <td>Includes end date and time</td>
    </tr>
    <tr>
        <td>start_station_name</td>
        <td>Starting station name</td>
    </tr>
    <tr>
        <td>start_station_id</td>
        <td>Starting station number</td>
    </tr>
    <tr>
        <td>end_station_name</td>
        <td>Ending station name</td>
    </tr>
    <tr>
        <td>end_station_id</td>
        <td>Ending station number</td>
    </tr>
    <tr>
        <td>start_lat</td>
        <td>Starting station latitude</td>
    </tr>
    <tr>
        <td>start_lng</td>
        <td>Starting station longitude</td>
    </tr>
    <tr>
        <td>end_lat</td>
        <td>Ending station latitude</td>
    </tr>
    <tr>
        <td>end_lng</td>
        <td>Ending station longitude</td>
    </tr>
    <tr>
        <td>member_casual</td>
        <td>Indicates whether user was a "registered" member (Annual Member, 30-Day Member or Day Key Member) or a "casual" rider (Single Trip, 24-Hour Pass, 3-Day Pass or 5-Day Pass)</td>
    </tr>
    <tr>
</table>

&#128269;&nbsp;&nbsp;Methodology:<br>
I utilized open-source weather data to investigate potential correlations between weather conditions and bike demand at the bike share station near my school. I examined the heatmap and the coefficiences between the weather variables and the pick up & drop off times using five regression models. Finally, after fine tuning hyperparameters, I selected the best performance by calculating the MSE of each model. With the best performance model, I predicted the pick up & drop off times using the first occurrence from the test data.<br>
<br>
&#128681;&nbsp;&nbsp;Limitation:<br>
This project introduces preliminary concepts for bike allocation and explores the potential impact of weather conditions on ridership. However, its scope is constrained by its concentration on a specific season, a single bike-share station, and simplified linear assumptions that also do not account for seasonality or other potential factors affecting ridership.<br>
<br>
&#128202;&nbsp;&nbsp;Conclusion:<br>
The predicted number of drop-offs is greater than the predicted number of pick-ups at the bikeshare station near my school, suggesting that there might not be an immediate need for reallocation. On a given day, we can see that the UV index is positively related to pick-up times, implying that more people tend to use bikes when the UV index is higher. This may also raise concerns about sun exposure and potential risks of skin-related diseases. The negative relationship between windspeed and pick-up times suggests that bike demand decreases on windy days. This could be due to discomfort and safety concerns while riding in strong winds. The Bikeshare could strategically plan maintenance or repair activities for bikes and docks on forecasted windy days, maximizing efficiency while minimizing the impact on ridership.

</body>
</html>
