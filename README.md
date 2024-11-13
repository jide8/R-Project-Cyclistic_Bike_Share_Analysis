# Google Data Analytics Cyclistic Bike Share Analysis Project Using R
## About the company
In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system at any time.

Cyclistic's finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, the Director of Marketing Moreno believes that maximizing the number of annual members will be critical to future growth.

Customers who purchase single-ride or full-day passes are called "casual riders". Customers who purchase annual memberships are Cyclistic "members".


### scenario and role
As a junior data analyst on the marketing team at Cyclistic, a bike-share company in Chicago, I am tasked with helping the company maximize its future success by increasing the number of annual memberships. The marketing director believes that achieving this goal depends on understanding the differences in bike usage between casual riders and annual members. My team's goal is to analyze this data and develop insights that will inform a new marketing strategy aimed at converting casual riders into annual members.
In order to answer the business questions, I will follow the steps of the data analysis process: 
1. Ask
2. Prepare
3. Process
4. Analyze
5. Share
6. Act

## Ask
### Business Task
Design marketing strategies aimed at converting casual riders into annual members
### Business Questions:
1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

### Stakeholders
- Lily Moreno — Director of the marketing team and my manager
- Cyclistic marketing analytics team 
- Cyclistic executive team

## Prepare
I will be using Cyclistic’s historical trip data from the past 12 months to analyze customer usage trends. [This public dataset](https://divvy-tripdata.s3.amazonaws.com/index.html), provided by Motivate International Inc. under this [license](https://www.divvybikes.com/data-license-agreement), allows exploration of different customer types while respecting data privacy—no personally identifiable information is included, so individual identities and payment details are not accessible.
Due to the large number of observations in each file, handling the combined dataset in Excel posed challenges, as it took considerable time to perform calculations across all rows. Therefore, R programming will be used for data cleaning and wrangling. Additionally, to manage computational limitations, we decided to work with a sample of the combined dataset (Divvy_Trips_2019_Q1 and Divvy_Trips_2020_Q1).
The ROCCC approach was applied to assess potential bias or credibility issues within the data.

**Dataset Limitations**

An initial review of the datasets for completeness showed that some rides are missing values for 'start_station_name,' 'start_station_id,' 'end_station_name,' and 'end_station_id.' Further examination suggests that most of the missing data for "start station name" is associated with electric bikes.

## Process
### Data Wrangling Combination Into A Single File
- Imported data in R studio
- Compared column names each of the files
- Renamed columns to make them consistent
- Inspected the dataframes and looked for incongruencies
- Converted data types to character so that they can stack correctly
- Added new columns

## Analyze
### Summary of actions taken to identify trends and relationships within the data, followed by exporting a summary file for further analysis.
- Descriptive Analysis of Ride Length
- Comparison Between Members and Casual Users
- Average Ride Time by Day for Members vs Casual Users
- Ridership Analysis by Type and Weekday

## Share
R studio visualization was utilized to visualize key trends and patterns, while Microsoft PowerPoint was used to present the main insights derived from the analysis.

## Act
I prepared the deliverables requested by the Director of Marketing, including the top three recommendations based on my analysis.

**Final Conclusions**

Based on the key findings, here are my top three recommendations:
- Make annual memberships include more unlimited number of rides for a certain extended time frame
- Create in between tier for memberships that includes annual benefits only on weekends
- Create in between tier for memberships that includes annual benefits only during summer months
