# Practice Quiz: Hands-On Activity: Filters and plots

## Activity overview

So far, you have learned a lot about ggplot2 and how to create data visualizations in R. In this activity, you’ll follow through a scenario and use the filters and facets features of ggplot2.

By the end of this activity, you will be able to customize your visualizations by applying filters and highlighting facets. This will enable you to emphasize certain aspects of your insights to create comparisons and more nuanced insights in your presentations.

## Working in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: Course 7 -> Week 4 -> Lesson3_Filters.Rmd.

The .csv file that you will need, hotel_bookings.csv, is also located in this folder.

If you have trouble finding the correct activity, check out this [step-by-step guide](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly here:

- [Lesson3_Aesthetics.md](./resources/Lesson3_Filters.md)
- [hotel_bookings.csv](../../module-3_working-with-data-in-R/p1_explore-data-and-R/resources/hotel_bookings.csv)

You can also find the Rmd file with the solutions for this activity here:

- [Lesson3_Aesthetics_Solutions.md](./resources/Lesson3_Filters_Solutions.md)

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

## Confirmation

In Step 5 of this activity, you created a data frame onlineta_city_hotels_v2. What is the lead time in the first row created in this data frame?

- [ ] 65
- [x] 88
- [ ] 92
- [ ] 100

> Correct: The lead time in the first row of the onlineta_city_hotels_v2 data frame is 88. By using a filter with ggplot2, you are able to select specific segments of your data and plot them using R. Going forward, you can use filters and facets to compare visualizations of different aspects of the same data to gain even deeper insights from your analyses.
