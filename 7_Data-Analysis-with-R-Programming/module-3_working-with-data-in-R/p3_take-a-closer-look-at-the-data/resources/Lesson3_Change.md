---
title: "Lesson 3: Changing your data"
output: html_document
---

## Background for this activity

In this activity, you’ll review a scenario, and focus on manipulating and changing real data in R. You will learn more about functions you can use to manipulate your data, use statistical summaries to explore your data, and gain initial insights for your stakeholders.

Throughout this activity, you will also have the opportunity to practice writing your own code by making changes to the code chunks yourself. If you encounter an error or get stuck, you can always check the Lesson3_Change_Solutions .rmd file in the Solutions folder under Week 3 for the complete, correct code.

## The Scenario

In this scenario, you are a junior data analyst working for a hotel booking company. You have been asked to clean a .csv file that was created after querying a database to combine two different tables from different hotels. You have already performed some basic cleaning functions on this data; this activity will focus on using functions to conduct basic data manipulation.

## Step 1: Load packages

Start by installing the required packages. If you have already installed and loaded `tidyverse`, `skimr`, and `janitor` in this session, feel free to skip the code chunks in this step. This may take a few minutes to run, and you may get a pop-up window asking if you want to proceed. Click yes to continue installing the packages.

```{r install packages}
install.packages("tidyverse")
install.packages("skimr")
install.packages("janitor")
```

Once a package is installed, you can load it by running the `library()` function with the package name inside the parentheses:

```{r load packages}
library(tidyverse)
library(skimr)
library(janitor)
```

## Step 2: Import data

In the chunk below, you will use the `read_csv()` function to import data from a .csv in the project folder called "hotel_bookings.csv" and save it as a data frame called `hotel_bookings`. Type "hotel_bookings.csv" between the quotation marks in the following code chunk.

If this line causes an error, copy in the line setwd("/cloud/project/Course 7/Week 3") before it.

```{r load dataset}
hotel_bookings <- read_csv("")
```

## Step 3: Getting to know your data

Like you have been doing in other examples, you are going to use summary functions to get to know your data. This time, you are going to complete the code chunks below in order to use these different functions. You can use the `head()` function to preview the columns and the first several rows of data. Finish the code chunk below and run it:

```{r head function}
head()
```

Now you know this dataset contains information on hotel bookings. Each booking is a row in the dataset, and each column contains information such as what type of hotel was booked, when the booking took place, and how far in advance the booking took place (the 'lead_time' column).

In addition to `head()` you can also use the `str()` and `glimpse()` functions to get summaries of each column in your data arranged horizontally. You can try these two functions by completing and running the code chunks below:

```{r str function}
(hotel_bookings)
```

You can see the different column names and some sample values to the right of the colon.

```{r glimpse function}
glimpse()
```

You can also use `colnames()` to get the names of the columns in your dataset. Run the code chunk below to get the column names:

```{r colnames function}
colnames(hotel_bookings)
```

## Manipulating your data

Let's say you want to arrange the data by most lead time to least lead time because you want to focus on bookings that were made far in advance. You decide you want to try using the `arrange()` function; input the correct column name after the comma and run this code chunk:

```{r arrange function}
arrange(hotel_bookings, )
```

But why are there so many zeroes? That's because `arrange()` automatically orders by ascending order, and you need to specifically tell it when to order by descending order, like the below code chunk below:

```{r arrange function descending}
arrange(hotel_bookings, desc(lead_time))
```

Now it is in the order you needed. You can click on the different pages of results to see additional rows of data, too.  

Notice that when you just run `arrange()` without saving your data to a new data frame, it does not alter the existing data frame. Check it out by running `head()` again to find out if the highest lead times are first:

```{r head function part two}
head(hotel_bookings)
```

This will be true of all the functions you will be using in this activity. If you wanted to create a new data frame that had those changes saved, you would use the assignment operator, <- , as written in the code chunk below to store the arranged data in a data frame named 'hotel_bookings_v2':

```{r new dataframe}
hotel_bookings_v2 <-
  arrange(hotel_bookings, desc(lead_time))
```

Run `head()`to check it out:

```{r new dataframe part two}
head(hotel_bookings_v2)
```

You can also find out the maximum and minimum lead times without sorting the whole dataset using the `arrange()` function. Try it out using the max() and min() functions below:

```{r}
max(hotel_bookings$lead_time)
```

```{r}
min(hotel_bookings$lead_time)
```

Remember, in this case, you need to specify which dataset and which column using the $ symbol between their names. Try running the below to see what happens if you forget one of those pieces:

```{r}
min(lead_time)
```

This is a common error that R users encounter. To correct this code chunk, you will need to add the data frame and the dollar sign in the appropriate places.

Now, let's say you just want to know what the average lead time for booking is because your boss asks you how early you should run promotions for hotel rooms. You can use the `mean()` function to answer that question since the average of a set of number is also the mean of the set of numbers:

```{r mean}
mean(hotel_bookings$lead_time)
```

You should get the same answer even if you use the v2 dataset that included the `arrange()` function. This is because the `arrange()` function doesn't change the values in the dataset; it just re-arranges them.

```{r mean part two}
mean(hotel_bookings_v2$lead_time)
```

## Practice Quiz

What is the average lead time?

- [ ] A: 14.0221
- [ ] B: 45.0283
- [ ] C: 100.0011
- [x] D: 104.0114

Remember to select the correct answer to this question on the Coursera platform after you complete this activity.

You were able to report to your boss what the average lead time before booking is, but now they want to know what the average lead time before booking is for just city hotels. They want to focus the promotion they're running by targeting major cities.

You know that your first step will be creating a new dataset that only contains data about city hotels. You can do that using the `filter()` function, and name your new data frame 'hotel_bookings_city':

```{r filter}
 <- 
  filter(hotel_bookings, hotel_bookings$hotel=="City Hotel")
```

Check out your new dataset:

```{r new dataset}
head(hotel_bookings_city)
```

You quickly check what the average lead time for this set of hotels is, just like you did for all of hotels before:

```{r average lead time city hotels}
mean(hotel_bookings_city$lead_time)
```

Now, your boss wants to know a lot more information about city hotels, including the maximum and minimum lead time. They are also interested in how they are different from resort hotels. You don't want to run each line of code over and over again, so you decide to use the `group_by()`and`summarize()` functions. You can also use the pipe operator to make your code easier to follow. You will store the new dataset in a data frame named 'hotel_summary':

```{r group and summarize}
hotel_summary <- 
  hotel_bookings %>%
  group_by(hotel) %>%
  summarise(average_lead_time=mean(lead_time),
            min_lead_time=min(lead_time),
            max_lead_time=max(lead_time))
```

Check out your new dataset using head() again:

```{r}
head(hotel_summary)
```

## Activity Wrap Up

Being able to manipulate data is a key skill for working in `R`. After this activity, you should be more familiar with functions that allow you to change your data, such as `arrange()`, `group_by()`, and `filter()`. You also have some experience using statistical summaries to make insights into your data. You can continue to practice these skills by modifying the code chunks in the rmd file, or use this code as a starting point in your own project console. As you practice, consider how performing tasks is similar and different in `R` compared to other tools you have learned throughout this program.
