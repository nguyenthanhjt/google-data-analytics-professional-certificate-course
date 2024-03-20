# Practice Quiz: Hands-On Activity: Create your own data frame

## Activity overview

Earlier, you learned about data frames. In this activity, you will create and use data frames in R.

As a refresher, a data frame is a collection of columns containing data, similar to a spreadsheet or SQL table. Data frames are one of the basic tools you will use to work with data in R. And you can create data frames from different data sources.

By the time you complete this activity, you will be able to create data frames with the `data.frame()` function and use data frames to complete tasks in R. This will enable you to summarize and organize data in R, which will help give your R analyses more structure as you complete more advanced data analysis tasks.

## Working in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](link), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: `Course 7 -> Week 3 -> Lesson2_Dataframe.Rmd`.

If you have trouble finding the correct activity, check out this [step-by-step guide](step-by-step guide link) on how to navigate in RStudio Cloud. Make sure to select the correct R markdown (.Rmd) file. The other .Rmd files will be used in different activities.

If you are using RStudio (Posit) Desktop, you can download the .Rmd file [here](desktop link).

You can also find the .Rmd file with the solutions for this activity [here](solutions link).

Carefully read the instructions in the comments of the .Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the .Rmd file, return here to confirm that your work is complete.

```r
install.packages("tidyverse")

library(tidyverse)

names <- c("jt", "trangle", "thutrang", "jay")

age <- c(10, 13, 12, 16)

people <- data.frame(names, age)

# inspect the data frame

head(people)

str(people)

glimpse(people)

colnames(people)

mutate(people, age_in_later_20_years = age + 20)

############PRACTICE########

fruits <- c("apple", "orange", "banana", "mango", "watermelon")

fruit_rank <- c("2", "3", "5", "4", "1")

my_fruits <- data.frame(fruits, fruit_rank)

head(my_fruits)

```

## Confirmation

Which summary functions can you use to preview data frames in R? Select all that apply.

- [x] `str()`

- [x] `head()`

- [x] `glimpse()`

- [ ] `mutate()`

> Correct: The `head()`, `glimpse()`, and `str()` summary functions allow you to preview data frames in R. The `head()` function returns the columns and the first several rows of data.The `mutate()` function lets you change the data frame, not preview it. Going forward, you can use summary functions to inspect the data frames you create in your career as a data analyst
