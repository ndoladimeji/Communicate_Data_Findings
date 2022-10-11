# Fordgobike Dataset
## by  _Oladimeji Nurudeen_



## Dataset

This dataset is for _Fordgobike bike sharing system_. It contains information about 174952 trips for the month and year, February, 2019. Information in the dataset include trip durations and time, users information, start and end stations. There are 174952 trips in the dataset with 10 features:
> trip duration in seconds, start_station_name, end_station_name, user_type, member_gender, bike_share_for_all_trip, day_of_week, hour, day_part, age

Only duration and age variables are numeric in nature, other variables are one of category, string, integer, float or datetime objects datatypes.


## Summary of Findings

When investigating the age variable, a range of outliers were identified. These outliers can be explained by inconsistencies in data collection. To avoid data distortion when doing further analysis, all of these outliers were removed from the dataset. I created the age, day_of_week, hour of day, day part columns to facilitate my analysis. I also changed the age datatype from float to integer to be consistent with real age, start_time datatype from string to datetime object datatype to enable extraction of hour, day, month and year. I made the day_of_week, day_part into categorical datatypes to make their analysis flexible with more properties. I then removed all unnecessary columns from the dataset. Finally, I removed all null values from the dataset.

The summary effects of features on trip durations and frequencies are as follows:

**Time**:
Morning and evening have the most trips. Trip duration is not necessarily affected by time of day.

**Day of Week**:
There are more trips during the weekdays than in weekends. Trip duration is not necessarily affected by day of week.

**Station Locations**:
Looking at the top 10 most popular stations, there are more trips during the weekdays than in weekends. Thursday is the most popular day in these stations except in Caltrain and Market St. where Tuesday is most popular. Stations in San Francisco dominate the list of top 10. More visits to the tourist attraction at Ferry Building and Embarcadero might be responsible for this.

**Age**:
Most of age population falls between 20 and 40 years old. It might imply they are full time employees and commuters.

**Gender**:
The number of trips in males is way more than the number in females. This needs to be investigated further. Trip duration is not necessarily affected by gender.

**User Type**:
The number of trips in subscribers is more than the number in customers because of pricing and population.



## Key Insights for Presentation

For the presentation, I focus on the influence of time, day of week, gender, age user type and station locations on trip durations and frequencies. I start by introducing the individual distribution of duration and age variables. Afterwards, I looked at the relationships between each of the above features versus trip frequencies and durations. I looked at each of the categorical variables: time, day of week, user type, start and end stations one by one. I then used the scatter plot vs heatplot to explore relationship between age and trip duration. Finally, I used a scatter plot to explore relationships between trip durations and ages across gender.

Key insights from the presentation include:

- Trip duration is not necessarily affected by gender
- The number of trips in males is way more than the number in females. This needs to be investigated further
- All trip durations for customers are greater than the median trip duration for a suscriber. An explanation for this might be that subscribers take rides for their routine short travels. On the other hand, customers take rides seldomly to travel long distances. Very likely, most of these customers are tourists.
- Stations in San Francisco dominate the list of top 10. Apart from being in the city, more visits to the tourist attractions at Ferry Building and Embarcadero might be responsible for this. Many stations in San Francisco connect to these tourist attractions.