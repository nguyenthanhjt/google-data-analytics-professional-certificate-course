# Practice Quiz: Hands-On Activity: Annotating and saving visualizations

## Activity overview

So far, you have used ggplot2 to create different kinds of visualizations. In this activity, you’ll follow through a scenario and add annotations to a data visualization with ggplot2. You will also learn how to save images from ggplot2 visualizations.

By the end of this activity, you will be able to enhance a visualization with annotations and save it as an image so that you can add it directly to a presentation. This will enable you to demonstrate your findings more clearly and better explain your insights in your career as a data analyst.

## Working in RStudio Cloud

To start, log into your RStudio Cloud account. Open the project you will work on in the activity with [this link](link), which opens in a new tab. If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click the following: Course 7 -> Week 4 -> Lesson4_Annotations.Rmd.

The .csv file that you will need, hotel_bookings.csv, is also located in this folder.

If you’re having trouble finding the correct activity, check out this [step-by-step guide](guide link) on how to navigate in RStudio Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file and the data for this activity directly here:

- [Lesson4_Annotations.md](./resources/Lesson4_Annotations.md)
- [hotel_bookings.csv](../../module-3_working-with-data-in-R/p1_explore-data-and-R/resources/hotel_bookings.csv)

You can also find the Rmd file with the solutions for this activity here:

- [Lesson4_Annotations_Solutions.md](./resources/Lesson4_Annotations_Solutions.md)

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

## Confirmation

After running the following code below to save the plot as a .png file in Step 5,  what dimensions (inches) would the image be saved?

```R
ggsave('hotel_booking_chart.png',width=7,height=7)
```

- [ ] 5x5
- [x] 7x7
- [ ] 10x10
- [ ] 25x25

> Correct: The dimensions you put in ggsave() image were 7x7. You can see these dimensions listed after you run the code chunk. Going forward, you can add annotations to enhance and clarify your visualizations with axis labels, chart titles, and more. You can then save images of your visualizations to share in reports and presentations.
