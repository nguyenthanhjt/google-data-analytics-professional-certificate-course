# Practice Quiz: Hands-On Activity: Using ggplot

## Activity Overview

In the last activity, you got an introduction to visualizing data in ggplot2. In this activity, you’ll dive deeper with ggplot2 to quickly create data visualizations that allow you to explore your data and gain new insights.

By the time you complete this activity, you will have strengthened your understanding of ggplot2 and visualizing data in R. You will be able to use basic ggplot2 syntax and troubleshoot some common errors you might encounter. This will enable you to easily demonstrate and share your insights throughout your career as a data analyst.

### Working in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: `Course 7` -> `Week 4` -> `Lesson2_GGPlot.Rmd`.

The .csv file you will need, hotel_bookings.csv, is also located in this folder.

If you have trouble finding the correct activity, check out this [step-by-step guide](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly:

- [Lesson2_GGPlot.md](./resources/Lesson2_GGPlot.md)
- [Lesson2_GGPlot_Solutions.md](./resources/Lesson2_GGPlot_Solutions.md)
- [hotel_bookings.csv](../../module-3_working-with-data-in-R/p1_explore-data-and-R/resources/hotel_bookings.csv)

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

### Confirmation

In Step 5 of this activity, you mapped columns to the x and y axes of a scatter plot. What syntax did you use to do this?

1 point

- [x] aes(x = stays_in_weekend_nights, y = children)
- [ ] aes(x = ‘stays_in_weekend_nights’, y = ‘children’)
- [ ] aes(x = children, y = stays_in_weekend_nights)
- [ ] aes(x = ‘children’, y = ‘stays_in_weekend_nights’)

> Correct: The correct syntax for mapping columns to axes in this activity is aes(x = stays_in_weekend_nights, y = children). Going forward, you can use the knowledge of mapping and the ggplot2 package to create many kinds of visualizations in RStudio.
