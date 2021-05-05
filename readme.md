# Ford GoBike Dataset
## by Ahmed Osama


## Dataset

> This data set includes 183412 records about individual rides information made in a bike-sharing system covering the greater San Francisco Bay area in February 2019. It contains information like the start and end stations of the trip, start and end dates, Bike ID, Memebers birth date, Trips Duration and etc.. 

Data Wrangling Process: 

- Unneeded columns: [start_station_latitude, start_station_longitude ,end_station_latitude, end_station_longitude, bike_id , start_station_id, end_station_id]

- Missing values: *start_station_id*, *start_station_name*, *end_station_id*, *end_station_name*, *member_birth_year* , *member_gender*

- Wrong datatype: *start_time*, *end_time*, *start_station_id*, *end_station_id*,*member_birth_year*, *member_gender*, *bike_share_for_all_trip*, *user_type* columns 

- Extracting the `Day`, `Hour` from start_date column in individual column for analysis purpose
- Making a new column for the age
- Making a new column for `duration_minute` values in minutes instead of seconds.


## Summary of Findings

> Univariate Exploration: For the Duration and times. The Most of trips have a rush hour range around `8-9am` and `17-18pm` during a day, there were more trips on work days `(Thursday - Tuesday)` working days compared to weekends. Most of trips were within `30 Minutes Duration` and the peaks within `5 to 15 Minutes`. For the members, there were more `Male riders than Female`, and most members were `Subscribers` not `Customers`. The majority of the members `did not use bike share for all of their trips`, and most of the riders were around `30 to 50` years old.

> Bivariate Exploration: The `gender` doesn't affect so much on the trip duration compared to the `User type`, Also the average trip durations are almost the same over the week days except for `Saturday and Sunday`, They have a higher average. Also the Age doesn't affect the trip duration so much. just a litte effect for the older ages. Also the Subscribers user type have a little high average ages than the Customer types.

> The Multivariate Exploration: strengthened some of the patterns discovered in the previous bivariate exploration as well as univariate exploration and it discovered some new insights, the relationship between the multiple variables `Age - Duration - Gender` are plotted. Showing some new insights like the average age for the `Other` gender type and the average duration trip.

## Key Insights for Presentation

> It seems that the gender doesn't affect so much on the duration compared to the User type. the genders are all close to each other. But for the types, the majority of the subscribers take a `1 to 10` trip duration. And the majority of the customer take a `8 to 20` trip duration.
> The multi variate plot is inspiring! it shows that majority  of the `other` type of genders are between `25 to 50` years old, and they spend from `5 to 30` minutes in the trip. But for females due to the very small number of them there is no interesting insights
