# Practice Quiz: Hands-On Activity: Aesthetics and visualizations

## Activity overview

In previous activities, you learned about and worked with ggplot2, an R package for data visualization. In this activity, you’ll follow through a scenario and continue to apply ggplot2 to tailor aesthetic features of visualizations.

By the end of this activity, you will be able to use R to create bar charts, update chart labels, and customize the aesthetics of a visualization by specific criteria. This will enable you to make more complex visualizations to demonstrate your findings.

## Working in RStudio Cloud

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click on the following: Course 7 -> Week 4 -> Lesson3_Aesthetics.Rmd.

The .csv file that you will need, hotel_bookings.csv, is also located in this folder.

If you have trouble finding the correct activity, check out this [step-by-step guide]([guide link](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw)) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly here:

- [Lesson3_Aesthetics.md](./resources/Lesson3_Aesthetics.md)
- [hotel_bookings.csv](../../module-3_working-with-data-in-R/p1_explore-data-and-R/resources/hotel_bookings.csv)

You can also find the Rmd file with the solutions for this activity here:

- [Lesson3_Aesthetics_Solutions.md](./resources/Lesson3_Aesthetics_Solutions.md)

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

*Note:* In Step #6 of the .RMD exercise attachment, be sure to add the chart variable name deposit_type within the facet_wrap function parentheses. Your code lines should look like this in your R editor:

```R
{r creating a plot} 

ggplot(data = hotel_bookings) +   

geom_bar(mapping = aes(x = distribution_channel)) +   

facet_wrap(~deposit_type)
```

## Confirmation

Based on the bar chart you created in Step 4, which distribution type has the most number of bookings?

- [ ] Corporate
- [ ] GDS
- [ ] Direct
- [x] TA/TO

> Correct: The TA/TO distribution type has the most number of bookings. By using ggplot2, you were able to customize the visualization so that it plainly shows which distribution type has the most number of bookings. Going forward, you can change the aesthetics of your visualization to emphasize different aspects of your findings, respond to stakeholder requests, and improve your presentations.
