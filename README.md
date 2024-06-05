
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

Power BI file is available on Github Release of this Repository.
           
#### Snapshots of the report

![image](https://github.com/noor2560/Google-Data-Analytics-Capstone-Project-Cyclistic-Ride-Share/assets/108732316/90334f17-91f3-48b8-91f9-8c28dce9db3c)

