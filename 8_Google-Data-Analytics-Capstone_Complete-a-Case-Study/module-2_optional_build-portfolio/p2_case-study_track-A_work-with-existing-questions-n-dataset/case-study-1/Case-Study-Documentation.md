# Google Data Analytics Capstone Project - Case Study

Hi there, over the few months, I've been working on the Google Data Analytics Professional Certificate through Coursera.

With 8 courses including, Google team takes me through the Data analytics phases:

At the last course, we have capstone projects which are required as a part of the certificate - junior data analyst skill.

- Case study 1:
- Case study 2:
- My own case study: //TODO: choose the topics  that related to COVID-19

This article would be sharing how I approached and completed the Case Study 1 which I encapsulated-applied all of the learned| achieved skills from the course, I will perform many real-worlds tasks of a junior data analyst

## Table of Contents

- [Google Data Analytics Capstone Project - Case Study](#google-data-analytics-capstone-project---case-study)
  - [Table of Contents](#table-of-contents)
  - [Case Study 1: How does a bike-share navigate speedy success?](#case-study-1-how-does-a-bike-share-navigate-speedy-success)
    - [Introduction](#introduction)
      - [Scenario](#scenario)
      - [Background](#background)
    - [1. ASK](#1-ask)
    - [2. PREPAE](#2-prepae)
      - [Data Organization](#data-organization)
      - [PREPARE: step by step](#prepare-step-by-step)
    - [3. PROCESS](#3-process)
    - [4. ANALYZE](#4-analyze)
    - [5. SHARE](#5-share)
    - [6. ACT](#6-act)
  - [Case Study 2](#case-study-2)

## Case Study 1: How does a bike-share navigate speedy success?

### Introduction

#### Scenario

I am assuming to be/play the role as a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, my team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve our recommendations, so they must be backed up with compelling data insights and professional data visualizations.

#### Background

Cyclistic

A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day.

About the company

In 2016, Cyclistic launched a successful bike-share oering. Since then, the program has grown
to a eet of 5,824 bicycles that are geotracked and locked into a network of 692 stations
across Chicago. The bikes can be unlocked from one station and returned to any other station
in the system anytime.

Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.

Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno (the director of marketing and my manager) believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.

Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends.

This case study will be analyzed using 6 steps of Data Analysis process: ASK, PREPARE, PROCESS, ANALYZE, SHARE, and ACT.

I will utilize R and RStudio for data analysis processing. I am using R because the dataset is too large for spreadsheets, and R allows for in-depth analysis and manipulation.

### 1. ASK

> Main objective for this project: To understand how casual riders and annual members use Cyclistic bikes differently.

In the “Ask” phase, these are the questions/business task that would guide the future of the marketing program:

- Key tasks:
  - [x] Identify the business task: `What attracts casual members to become annual members?`
  - [x] Consider key stakeholders:
    - `Direct of Marketing|Manager - Moreno`: who is responsible for the development of campaigns and initiatives to promote the bike-share program.
    - `Executives teams`: The notoriously detail-oriented executive team will decide whether to approve the recommended marketing program.
    - `(Analytics teams)`: the team which are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy.
- Deliverable:
  - A clear statement of the business task: `The key things to attract rider become annual members`
  - What is the problem you are trying to solve?: Answer the question `How do annual members and casual riders use Cyclistic bikes differently?` to find out the information to create a marketing strategy to support in turning casual dirver into annual members
  - How can your insights drive business decisions?: `Figure out the difference between Annual Members and Casual Riders when they use the Cyclistic bikes to define strategy and design the marketing campaign to attract more members. By doing so,  profit can increase quickly`

### 2. PREPAE

- In the “Prepare” phase, there are some key tasks need to be completed
  - [x] Download data and store it appropriately.
  - [x] Identify how it’s organized.
  - [x] Sort and filter the data.
  - [x] Determine the credibility of the data.

Answer some guiding questions before delve into the data to ensure the data is ready for analysis:

- Are there issues with bias or credibility in this data? Does your data ROCCC?
  - `The data is Reliable: data is provided by the first party - Lyft Bikes and Scooter company which operate the City of Chicago's Divvy bicycle sharing service.`
  - `The data is original: it was created by Motivate International Inc. as the primary party that was validated as the orginal source.`
  - `Comprehensive: data contain completed information for analysis`
  - `Current: data is up-to-date until the current time in 2024`
  - `Cited: The data is cited & credible which from Lyft Bikes and Scooters, LLC (“Bikeshare”) operates the City of Chicago’s (“City”) Divvy bicycle sharing service. Bikeshare and the City are committed to supporting bicycling as an alternative transportation option. As part of that commitment, the City permits Bikeshare to make certain Divvy system data owned by the City (“Data”) available to the public.`
- How are you addressing licensing, privacy, security, and accessibility?:
  - `The data is open and , is maintained & made available by Motivate International Inc, and follow the issued Data License Agreement on https://divvybikes.com/data-license-agreement`
- How did you verify the data’s integrity?: `The data was examined and integrity with the consistency of column (name, quantity,.. ), data type`
- How does it help you answer your question? `The data will enable us to analyze both annual members and casual riders to identify any significant traits related to the riders, their bike usage, and their requirements.`
  - The information can be found in the data will examine annual members and casual riders to determine their main characteristics such as: rider's bike type, trip info, riding time,... which
- Are there any problems with the data?
  - `It can be better if the data provides more information regarding measuring unit of time, stations,...`

Cyclistic's historical data - which is open to the public and kept on cloud. The data has been made available by Motivate International Inc.

The Cyclistic trip data is available [here](https://divvy-tripdata.s3.amazonaws.com/index.html) that are historical trip data from 2013 to 2024.

#### Data Organization

The data consists of csv files, is organized by quarters in the year from 2013 to 2019 and by month from 2020 to 2024. Each CSV file structured utilizing rows and columns

At the time I perform this analysis June 2024, I use Cyclistic’s historical trip data in 2023 to analyze.

There are 12 files with naming convention of `YYYYMM-divvy-tripdata.csv` and each file includes information for one month:

- Ride id: ride_id - the identity of each data record
- Bike type: rideable_type
- Start time: started_at
- End time: ended_at
- Start station: start_station_id, start_station_name, start_lat, start_lng
- End station: end_station_id, end_station_name, end_lat, end_lng
- Start location:
- End location:
- Whether the rider is a member or not: member_casual

#### PREPARE: step by step

- Firstly, we would need to install & load the packages required for this process, which in this case will be: Tidyverse, Janitor & Lubridate.

  ```R
  install.packages('tidyverse')
  install.packages('janitor')
  install.packages('lubridate')
  ```

- Subsequently, We need to take a step to collect data from downloaded data files. The data is stored in .zip files, so we have to extract them, as I chose the 2023 dataset, then I will get 12 .csv files, one file represent one month of trip data.
- We will use function `read.csv()` of package:utils to import csv into RStudio, before this we must know the working directory to input the right path of csv files as paramter to `read.csv()`

  ```R
  #=====================
  # STEP 1: COLLECT DATA
  #=====================
  getwd() # Get working directory
  setwd("./input-data/") # Set working directory

  m01 <- read.csv("./input-data/202301-divvy-tripdata.csv")
  m02 <- read.csv("./input-data/202302-divvy-tripdata.csv")
  m03 <- read.csv("./input-data/202303-divvy-tripdata.csv")
  m04 <- read.csv("./input-data/202304-divvy-tripdata.csv")
  m05 <- read.csv("./input-data/202305-divvy-tripdata.csv")
  m06 <- read.csv("./input-data/202306-divvy-tripdata.csv")
  m07 <- read.csv("./input-data/202307-divvy-tripdata.csv")
  m08 <- read.csv("./input-data/202308-divvy-tripdata.csv")
  m09 <- read.csv("./input-data/202309-divvy-tripdata.csv")
  m10 <- read.csv("./input-data/202310-divvy-tripdata.csv")
  m11 <- read.csv("./input-data/202311-divvy-tripdata.csv")
  m12 <- read.csv("./input-data/202312-divvy-tripdata.csv")
  ```

- Merge the 12 into 1 data frame

### 3. PROCESS

- Key tasks
  - [x] Check the data for errors.
  - [x] Choose tools.
  - [x] Transform the data so you can work with it effectively.
  - [x] Document the cleaning process.

As mentioned above, I will utilize R & RStudio for data processing.

I examined the columns after making changes and confirmed that the data types remained consistent following manipulation.

To ensure that the data is clean and ready to analyze, I will do steps with some R packages(tidyverse, dplyr):

- Remove NA and duplicated
- The data columns with dates and time format will be formatted
- Create new aggregation columns for analysis

The cleaning process has been thoroughly documented.


### 4. ANALYZE

- Key tasks
  - [x] Aggregate the data so it’s useful and accessible.
  - [x] Organize and format your data.
  - [x] Perform calculations.
  - [x] Identify trends and relationships.

### 5. SHARE

- Key tasks
  - [x] Determine the best way to share your findings.
  - [x] Create effective data visualizations.
  - [x] Present your findings.
  - [x] Ensure your work is accessible

### 6. ACT

- Key tasks
  - [x] Determine the best way to share your ndings.
  - [x] Create eective data visualizations.
  - [x] Present your ndings.
  - [x] Ensure your work is accessible.


## Case Study 2
