
# Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share


## Introduction

This is a capstone project in the Google Data Analytic Certificate Course on Coursera. In this project data analysis process: ask, prepare, process, analyze, share, and act are implemented in order to answer the key business questions pertaining to Cyclistic, a bike-share company in Chicago.




### Steps followed 

#### 1) ASK : Business task

#### Problem Statement

-	Cyclistic is a bike-share program that features more than 5,800 bicycles and 600 docking stations. 
-	Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. 
-	The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. 
-	Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day. 

Business task include:
To find out how annual members and casual riders use Cyclistic bikes differently.

#### 2) PREPARE : Data source description and Data Collection


The data has been made available by Motivate International Inc.

![image](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/assets/108732316/130744a1-53ba-4218-95f4-d5d70bace004)

Metadata:
The data includes 13 different variables listed below, each with a small description. 
-	ride_id: Unique ID assigned to each individual ride
-	rideable_type: Type of bicycle (classic, docked, electric)
-	started_at: Date and time at the start of the trip
-	ended_at: Date and time at the end of the trip
-	start_station_name: Name of the station the trip started at
-	start_station_id: ID number of the station the trip started at
-	end_station_name: Name of the station the trip ended at
-	end_station_id: ID number of the station the trip ended at
-	start_lat: Latitude of starting location
-	start_lng: Longitude of the start location
-	end_lat: Latitude of ending location
-	end _lng: Longitude of ending location
-	member_casual: Type of membership (Casual or Cyclistic Member)

#### 3) DATA PROCESSING : Cleaning the data
-	Checked all rows in each file for duplicates using the built-in feature on Excel
-	Added a new column “trip_duration” using a simple formula =end_trip - start_trip
-	Created two new columns: day and month using function TEXT(C2,”dddd”) and TEXT(C2,”mm”) respectively
-	Formatted this column in hh:mm format
-	Checked all rows' max and min values to look for outliers
-	Removed all the rows with blanks

#### 4) ANALYZE : Analysis of data using SQL  

Due to the large volume of rows (> 1,000,000), I moved my analysis from Excel to SQL to handle the large volume of data. 

I used the open-source platform DB Browser with SQLite to UNION all the tables from each month into one table.

Complete list of SQL code can be found [here](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/blob/main/SQL%20code).


#### 5) SHARE : Visualize data using Microsoft Power BI

[Dashboard Link](https://app.powerbi.com/groups/me/dashboards/d61cc99e-0a7f-4887-a076-a17e6e33e39c?experience=power-bi)

![image](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/assets/108732316/fd95fb6f-c4a5-4861-91b7-2fde6d604643)

![image](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/assets/108732316/4905729c-f45b-4ed6-8c1f-84dee4763181)

Power BI file is available on Github Release of this Repository.
           
#### Snapshots of the report

![image](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/assets/108732316/90334f17-91f3-48b8-91f9-8c28dce9db3c)

#### ACT: Findings and Recommendations

### Insights from the report


- The Average trip duration for casual riders is 16 minutes 32 seconds while trip duration for member riders is 11 minutes and 22 seconds.

- Preferred days member riders ride is weekdays (Tuesday, Wednesday and Thursday).

- The Casual riders ride the most on weekends (Saturday and Sunday).

- The highest number of trips by member riders in the year 2022 is in September while for Casual members it is in the month of July.

- Member riders start their ride in the early hours of morning at around 6:00 AM  possibly commuting to work or school. We can also see a sharp peak at 18:00 PM in the evening which aligns with typical end-of-workday hours, indicating that members are likely riding home from work. This high frequency of riders at these times indicats regular use for commuting to and from work or school.

- Casual riders start their rides at around 12 noon. There is a gradual rise in the line chart at around 6:00 PM which suggests that casual riders may be using the bikes for leisure activities, such as lunchtime rides, sightseeing, or casual outings during the day.

- The most popular bike type is Classic bike with 58% of riders choosing this type. Hence, majority of riders' needs and expectations in terms of comfort, ease of use, and suitability for both commuting and leisure activities.

-Wells St and Concord Ln is the most popular destination for both casual and member riders. The location serves as a central hub for both commuting and leisure activities. For commuters, it could be near workplaces, while for casual riders, it is close to parks, shops, or entertainment venues.

#### How Members Use Bikes Differently Than Casual Riders?

Member Riders use bikes for: 

- Commuting
- Shorter rides  
- More frequent usage

Casual Riders use bikes for: 
- Recreational purposes
- Longer rides 
- Less frequent usage





#### Why would casual riders buy Cyclistic annual memberships?

Reasons for Buying Annual Memberships:

- Cost savings for frequent users.
- Access to bikes during peak times.
- Special promotions or discounts.
- Benefits such as cost savings, convenience, and additional perks could entice casual riders.

#### How can Cyclistic use digital media to influence casual riders to become members?

- Use targeted social media campaigns to highlight the convenience and cost-effectiveness of memberships.

- Provide special offers and discounts for frequent riders.



### Repository Contents:

- README file
- Sql file
- Power BI report files (.pbix)













        
