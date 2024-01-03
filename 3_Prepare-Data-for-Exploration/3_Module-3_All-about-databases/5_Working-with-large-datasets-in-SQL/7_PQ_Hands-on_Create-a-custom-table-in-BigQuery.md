# Hands-On Activity: Create a custom table in BigQuery

## Activity overview

Recently, you’ve been thinking about identifying good data sources that would be useful for analysis. You also spent some time in a previous activity exploring a public dataset in BigQuery and writing some basic SQL queries. In addition to using public data on BigQuery, you will need to be able to import data from other sources. In this activity, you will create a custom table and dataset, which you’ll load into a new table and query. 

By the time you complete this activity, you will be able to load your own data into BigQuery for analysis. This will enable you to import your own data sources into BigQuery, which is a skill you will need in order to analyze data from different sources.

What you will need

To get started, download the baby names data zip file. This file contains about 7 MB of data about popular baby names from the US Social Security Administration website.

Click the link to the baby names data zip file to download it.

Link to baby names data: [names.zip](./resources/names.zip)

## Create a custom table

Once you have the zip file downloaded, you can import it into BigQuery to query and analyze. In order to do that, you will need to create a new dataset and a custom table.

**Step 1: Unzip the file**
You will need to **unzip the file you downloaded** onto your computer in order to access it on BigQuery. Once you have unzipped the file, you will find a .pdf file titled NationalReadMe that contains more information about the dataset. This dataset tracks the popularity of baby names for each year; you can find text files labelled by the year they contain. Open **yob2014.txt** to preview the data. You will notice that it’s a .csv file with three columns. **Remember where you saved this folder** so you can reference it later.
**Step 2: Create a dataset**
Before you can upload your txt file and create a table to query, you will need to create a dataset to upload your data into and store your tables.

1. Go to the Explorer pane in your workspace and click the three dots next to your pinned project to open a menu. From here, select Create dataset.
