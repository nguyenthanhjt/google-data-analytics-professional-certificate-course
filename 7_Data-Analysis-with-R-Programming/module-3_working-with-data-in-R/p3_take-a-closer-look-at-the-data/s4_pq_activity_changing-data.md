# Practice Quiz: Hands-On Activity: Changing your data

## Activity Overview

By now, you have learned many ways to change and work with data in a variety of settings, including spreadsheets and RStudio. In this activity, you’ll follow through a real-world scenario and practice manipulating and changing real data in R.

Upon completing this activity, you will know how to use functions to manipulate your data and use statistical summaries to explore your data. This will enable you to use R for more complex tasks in your career as a data analyst and help you gain initial insights into data that you can share with your stakeholders.

### Working in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: Course 7 -> Week 3 -> Lesson3_Change.Rmd.

The .csv file that you will need, hotel_bookings.csv, is also located in this folder.

If you have trouble finding the correct activity, check out this [step-by-step guide](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly:

- [Lesson3_Change.Rmd](./resources/Lesson3_Change.Rmd)
- [Lesson3_Change_Solutions.Rmd](./resources/Lesson3_Change_Solutions.Rmd)
- [hotel_bookings.csv](../p1_explore-data-and-R/resources/hotel_bookings.csv)

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

### Confirmation

What is the average lead time for a hotel booking in this data set?

- [x] 104.0114
- [ ] 14.0221
- [ ] 100.0011
- [ ] 45.0283

> Correct: The average lead time is 104.0114 days. You were able to calculate this using the mean() function on the lead_time column in the data set. Going forward, you can apply the functions you used in this activity to future projects to change and analyze your data.