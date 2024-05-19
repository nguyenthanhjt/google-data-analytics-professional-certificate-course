# Capstone: Case Study 1

## Step 1: ASK

Three questions will guide the future marketing program:

1. How do annual members and casual riders use Cyclistic bikes differently?
2. Why would casual riders buy Cyclistic annual memberships?
3. How can Cyclistic use digital media to influence casual riders to become members?

Moreno has assigned you the first question to answer: How do annual members and casual
riders use Cyclistic bikes differently?

You will produce a report with the following deliverables:

1. A clear statement of the business task
2. A description of all data sources used
3. Documentation of any cleaning or manipulation of data
4. A summary of your analysis
5. Supporting visualizations and key findings
6. Your top three recommendations based on your analysis
Use the following Case Study Roadmap as a guide. Note: Completing this case study within a
week is a reasonable goal.

- Guiding questions
  - What is the problem you are trying to solve?:
    - Answer the question `How do annual members and casual riders use Cyclistic bikes differently?` to find out the information to create a marketing strategy to support in turning casual dirver into annual members
  - How can your insights drive business decisions?: `Figure out the difference between Annual Members and Casual Riders when they use the Cyclistic bikes to define strategy and design the marketing campaign to attract more members. By doing so,  profit can increase quickly`
- Key tasks:
  - [x] Identify the business task: `What attracts casual members to become annual members?`
  - [x] Consider key stakeholders:
    - `Direct of Marketing|Manager - Moreno`: who is responsible for the development of campaigns and initiatives to promote the bike-share program.
    - `Executives teams`: The notoriously detail-oriented executive team will decide whether to approve the recommended marketing program.
    - `(Analytics teams)`: the team which are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy.
- Deliverable:
  - A clear statement of the business task: `The key things to attract rider become annual members`

## Step 2: PREPARE

[Download the previous 12 months of Cyclistic trip data here](https://divvy-tripdata.s3.amazonaws.com/index.html)

Now, prepare your data for analysis using the following Case Study Roadmap as a guide:

- Guiding questions
  - Where is your data located?: `Cyclistic's historical data - which is open to the public and kept on cloud. The data has been made available by Motivate International Inc.`
  - How is the data organized? `The data consists of 10 csv files, is organized by quarters in the year from 2013 to 2019 and by month from 2020 to 2024. Each CSV file structured utilizing rows and columns`
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
- Key tasks
  - [x] Download data and store it appropriately.
  - [x] Identify how it’s organized.
  - [x] Sort and filter the data.
  - [x] Determine the credibility of the data.
- Deliverable
  - A description of all data sources used: `The data source comprises 10 CSV files: one for the first quarter, and individual files for each month from April onwards. The data spans from January to December.`

## Step 3: PROCESS

The individual CSV files will be merged into a single file to facilitate easier manipulation and analysis. This combined file will then be cleaned, and additional columns will be added.

Then, process your data for analysis using the following Case Study Roadmap as a guide:

- Guiding questions
  - What tools are you choosing and why?
    - Utilize EXCEL for data processing
    - Utilize SQL for data processing(BigQuery)
    - Utilize R and R Studio for data processing: `I am using R because the dataset is too large for spreadsheets, and R allows for in-depth analysis and manipulation.`
  - Have you ensured your data’s integrity? `I examined the columns after making changes and confirmed that the data types remained consistent following manipulation.`
  - What steps have you taken to ensure that your data is clean? `I remove NA and duplicated, the data columns with dates and time format will be formatted, create new columns for analysis`
  - How can you verify that your data is clean and ready to analyze? `The data has no duplicated, NA, date time columns is formatted with consistently.`
  - Have you documented your cleaning process so you can review and share those results? `The cleaning process has been thoroughly documented.`
- Key tasks
  - [x] Check the data for errors.
  - [x] Choose your tools.
  - [x] Transform the data so you can work with it effectively.
  - [x] Document the cleaning process.
- Deliverable
  - Documentation of any cleaning or manipulation of data
