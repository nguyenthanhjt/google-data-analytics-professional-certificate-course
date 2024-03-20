---
title: "Lesson 2: Importing and working with data"
output: html_document
---

## Background for this activity / Introduction

By now, you have some experience manually entering data in `R` to create a data frame. As a data analyst, it will also be common for you to import data from external files into your `R` console and use it to create a data frame to analyze it. In this activity you will learn how to import data from outside of `R` using the `read_csv()` function. Then, once you have imported a data file, you will use `R` functions to manipulate and interact with that data.

You can start importing and exploring data with the code chunks in the RMD space. To interact with the code chunk, click the green arrow in the top-right corner of the chunk. The executed code will appear in the RMD space and your console.

Throughout this activity, you will also have the opportunity to practice writing your own code by making changes to the code chunks yourself. If you encounter an error or get stuck, you can always check the Lesson2_Import_Solutions .rmd file in the Solutions folder under Week 3 for the complete, correct code.

## The scenario

In this scenario, you are a junior data analyst working for a hotel booking company. You have been asked to clean a .csv file that was created after querying a database to combine two different tables from different hotels. In order to learn more about this data, you are going to need to use functions to preview the data's structure, including its columns and rows. You will also need to use basic cleaning functions to prepare this data for analysis.

## Step 1: Load packages

Start by installing your required package. If you have already installed and loaded `tidyverse` in this session, feel free to skip the code chunks in this step.

```{r}
install.packages("tidyverse")
```

Once a package is installed, we can load it by running the `library()` function with the package name inside the parentheses:

```{r}
library(tidyverse)
```

## Step 2: Import data

One of the most common file types data analysts import into `R` is comma separated values files, or .csv files. The `tidyverse` library package `readr` has a number of functions for "reading in" or importing data, including .csv files and other external sources.

In the chunk below, use the `read_csv()` function to import data from a .csv in the project folder called "hotel_bookings.csv" and save it as a data frame called `bookings_df`.

If this line causes an error, copy in the line setwd("projects/Course 7/Week 3") before it.

The results will display as column specifications:

```{r}
bookings_df <- read_csv("hotel_bookings.csv")
```

Now that you have the `bookings_df`, you can work with it using all of the  `R` functions you have learned so far.

## Step 3: Inspect & clean data

One common function you can use to preview the data is the `head()` function, which returns the columns and first several rows of data. Check out the `head()` function by running the chunk below:

```{r}
head(bookings_df)
```

In addition to `head()` there are a number of other useful functions to summarize or preview your data frame. For example, the `str()` and function will provide summaries of each column in your data arranged horizontally. Check out the `str()` function by running the code chunk below:

```{r}
str(bookings_df)
```

To find out what columns you have in your data frame, try running the the `colnames()` function in the code chunk below:

```{r}
colnames(bookings_df)
```

If you want to create another data frame using `bookings_df` that focuses on the average daily rate, which is referred to as `adr` in the data frame, and  `adults`, you can use the following code chunk to do that:

```{r}
new_df <- select(bookings_df, `adr`, adults)
```

To create new variables in your data frame, you can use the `mutate()` function. This will make changes to the data frame, but not to the original data set you imported. That source data will remain unchanged.

```{r}
mutate(new_df, total = `adr` / adults)
```

## Step 4: Import your own data

Now you can find your own .csv to import! Using the RStudio Cloud interface, import and save the file in the same folder as this R Markdown document. To do this, go to the Files tab in the lower-right console. Then, click the Upload button next to the + New Folder button. This will open a popup to let you browse your computer for a file. Select any .csv file, then click Open. Now, write code in the chunk below to read that data into `R`:

```{r}

```

You can check the solutions document for this activity to check your work.

## Activity Wrap Up

Now that you know how to import data using the `read_csv()` function, you will be able to work with data that has been stored externally right in your `R` console. You can continue to practice these skills by modifying the code chunks in the rmd file, or use this code as a starting point in your own project console. As you become more familiar with the process of importing data, consider how importing data from a .csv file changed the way you accessed and interacted with the data. Did you do anything differently? Being able to import data from external sources will allow you to work with even more data, giving you even more options for analyzing data in `R`.  

Make sure to mark this activity as complete in Coursera.
