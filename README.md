# Ford GoBike Data Exploration
## by Chukwudi Okereafor

## Dataset
This data set contains information of over 170000 rides taken from one station to another in San Francisco Bay area, with over 4000 bikes used. The attributes included `duration` (in seconds), `user_type`, `start_time`, `end time`, as well as additional information such as `bike_id`, `start_station` (id, name, longitude and latitude),` end station` (id, name, longitude and latitude), `member_birth_year`, and `member_gender`.  Rows with missing values were dropped and 3 features were created (`hour_of_day`, `day_of_week` and `member_age`) from `start_time` and `member_birth_year`. 

## Summary of Findings
Bike ride duration in the dataset take on a very large range of values, from 60 seconds at the lowest to 84548 seconds at the highest. After removing outliers and plotted on a logarithmic scale, the distribution of bike ride duration look more like normal distribution with peak at little less than 550 seconds. Most bike rides are short trips. Majority of the bike users are Subscribers (90.7%) and Customers (for those who do not subscribe) were 9.3%. In the exploration, I found that `user_type` affects bike usage in number of rides and trip duration. Both types share some in common and have some difference. Although subscribers make a lot more trips than customers, customers generally take longer bike trip than subscribers. Both subscribers and customers take longer trips during weekend than weekdays. Subscribers take most of their trips around 7-9am (peak at 8am) and 4-6pm (peak at 5pm), typical commute hours. They are probably commuters to work/school. Subscribers took more trips during the weekdays and less on weekend. There are a high number of trips on Weekdays than on weekends for both Subscribers and Customers.
Male bikers have the highest number of trips as compared to female and other gender across all the times of the day and all the days of the week.
There are distinctions between subscribers and customers. Subscribers and customers have a very different life and work style. Subscribers are more likely to use for workday related purposes while customers more likely to use for fun and do not share bike. 

## Key Insights for Presentation
For the presentation, I start by introducing the numeric variables - duration in seconds and the age of the riders - followed by other categorical variables – user_type, hour of day, day of week and gender. 
I plot to see impacts of user_type on duration and usage (trip count) and focus on how different groups of users use the service. I also plot to see the impact of the age of the riders and the usage.
I used box plot for duration and day of week, looking at when longer bike trips are being taken.
