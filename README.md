# Ford Go Bike Trip Data Exploration
## by Chukwuemeka Nwokocha

## Dataset

The dataset contains durations and other features (including but not limited to user_type, member_birth_year, member_gender and bike_share_for_all_trip) for ford go bike trips in February 2019.
Dataset can be found [here](https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv)

Wrangling:
Converted start_time and end_time to datetime objects
Converted start_station_id and end_station_id to int datatype
Convert start_station_name, end_station_name, user_type, member_gender and bike_share_for_all_trip to category datatype

## Summary of Findings

In summary, I have been able to come to the following conclusions:
1. With log-transformed histograsm, I was able to discover that the average ride is between 300 to 1000 seconds and that most riders were born between 1980 and 2000
2. Through countplots, I found out that the Male riders (member_gender) and subscribers (user_type) are highly dominant in the dataset
3. From a countplot, I saw that the peak hours are 8 - 10 in the morning and 15 - 19 in the evening
4. With a pairplot, I discovered a correlation between duration_sec and member_birth_year, after using a bivariate scatterplot between them, I found that the longest rides were found with riders born between 1980 and 2000
5. From a scatter plot between member_birth_year and start_time (hour), I discovered that older people ride more during the day
6. With a log transformed boxplot between user_type and duration_sec, I found that the customers generally have longer rides than subscribers
7. Through a log-transformed facetgrid of lineplots of duration_sec, member_birth_year and member_gender as the 'col', I found that the longest rides in the dataset are found with young female riders
8. From a log-transformed facetgrid of lineplots of duration_sec, member_birth_year and user_type as the 'col', I discovered that the Subscribers are generally older riders than the customers, I also found out that the younger customers have longer rides than the older customers and subscribers.
9. From my discovery in N0. 8, I decided to see how the gender of the customer affects the ride duration, with a log-transformed facetgrid of boxplots of duration_sec, meber_gender and user_type as the 'col'; I discovered that female subscribers have longer rides.
10. Coupled with the data and results earlier, I decided to plot a log-transformed facetgrid containing duration_sec, member_birth_year, member_gender on the 'col' and user_type as the 'row'; I discovered that the younger female subscribers are the ones with the longest rides.

From this research, I have concluded that the Member_gender, member_birth_year and the user_type columns all have a direct effect and impact on the duration of the ride. They either increase or decrease the length of the ride.

## Key Insights for Presentation

In my presentation, I start by showing the distribution of the duration_sec column (target value). Following this up is a histogram showing how the member birth years are distributed. After this, i plot a scatterplot comparing the values in the first and second plot. Following this is a box plot of duration_sec and the categorical variable member_gender. With a multivariate plot, i compare the ride duration, birth year and gender. I go further and create another facetgrid of lineplots with ride duration, gender and faceting on a new variable; user_type.

Finally, I compare all variables with a facetgrid of duration_sec and member_birth_year, with member_gender on the 'col' and user_type on the 'row'.
