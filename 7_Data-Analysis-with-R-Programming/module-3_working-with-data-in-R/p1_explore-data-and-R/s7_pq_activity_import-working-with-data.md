# Practice Quiz: Hands-On Activity: Importing and working with data

## Activity overview

By now, you have some experience manually entering data in R to create a data frame. In this activity you will import data from outside of R using the `read_csv()` function, then use R functions to manipulate and interact with that data.

Upon completing this activity, you will be able to import data into RStudio so you can analyze it. This will enable you to bring your own .csv files into RStudio and use this environment for personal projects, which will help you hone your data skills. As a data analyst, it will also be common for you to import data from external files into your R console and use it to create a data frame to analyze it.

## Work in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: Course 7 -> Week 3 -> Lesson2_Import.Rmd.

The .csv file you will need, hotel_bookings.csv, is also located in this folder.

If you have trouble finding the correct activity, check out this [step-by-step guide](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly [here](desktop_link).

You can also find the Rmd file with the solutions for this activity [here](solutions_link).

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

If you have trouble completing the exercise or don't know how to proceed, navigate to Course 7 -> Week 3 -> Solutions -> Lesson2_Import_Solutions.Rmd in the exercise files.

```r
install.packages("tidyverse")

library(tidyverse)

# set working directory
setwd(dir = "./goolge-data-analytics-professional-certificate/Course 7/Week 3/")

# read and assign csv data to a dataframe
booking_df <- read_csv("hotel_bookings.csv")

# inpect dataframe
head(booking_df)

str(booking_df)

colnames(booking_df)

# create new DF to working with
new_df <- select(booking_df, `adr`, adults)

# modify df to create a new column for calculation

mutate(new_df, total = adr/adults)
```

## Confirmation

Which syntax would you use to import a dataset called quarter_earnings.csv into RStudio?

- [x]:

    ```R
    earnings_df <- read_csv("quarter_earnings.csv")
    ```

- [ ]:

    ```R
    earnings_df <- read_csv(“quarter_earnings”)
    ```

- [ ]:

    ```R
    earnings_df <- read_csv(quarter_earnings.csv)
    ```

- [ ]:

    ```R
    earnings_df <- read_csv(quarter_earnings)
    ```

> Correct:
The proper syntax to use for importing the “quarter_earnings.csv” dataset is `earnings_df <- read_csv("quarter_earnings.csv")`. The results of this function display as column specifications of the data frame it creates. Going forward, you can import data into RStudio with read_csv() for projects throughout your career as a data analyst.
