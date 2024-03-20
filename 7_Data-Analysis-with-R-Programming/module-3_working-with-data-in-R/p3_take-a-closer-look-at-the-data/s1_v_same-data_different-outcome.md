# Video: Same data, different outcome

Video transcript

- Great to have you back.
- Earlier, we talked about summarizing data in R.
- We even used the summarize function to calculate the mean for one of our penguin data variables.
- Now, we'll work with a very famous data example: Anscombe's quartet.
- Anscombe's quartet has four datasets that have nearly identical summary statistics.
- But those summary statistics might be misleading.
- Data visualizations, especially for datasets like these, are so important.
- They help us discover things in our data that would otherwise remain hidden.
- Plus, you'll discover some of the ways R can create awesome visualizations.
- Let's install the packages.
- This may take a few minutes to load.
- Let's load the Anscombe's quartet data now.
- When we view this data, we notice that there's four sets of x and y axis in the data frame.
- That's the quartet.
- Data can be summarized by different statistical measures.
- We'll get a summary of each set with the mean, standard deviation, and correlation for each of these datasets.
- We'll start by indicating that we want to group our data by set.
- Then we'll input our summarize function.
- When we run this, we'll get a summary of these statistical measures.
- In our summary table, we can check the mean.
- The mean for x in each dataset is nine, and the mean for y is 7.5.
- The standard deviation can help us understand the spread of values in a dataset and show us how far each value is from the mean.
- The standard deviation for x and y in every set in the quartet is the same, 3.32 and 2.03.
- Finally, we've got our correlation, which shows us how strong the relationship between two variables is.
- Here, it looks like the correlation between x and y in all four sets is around 0.816.
- Based on the summaries we created with our statistical measures, these datasets are identical, but sometimes just looking at the summarized data can be misleading.
- Let's put together some simple graphs to help us visualize this data and check if the datasets are actually identical.
- You'll learn more about plotting data in R later.
- But for now, we'll just get a quick idea of how this data appears.
- Check it out.
- These four datasets appear quite different when we visualize them.
- If we just gone with a statistical summaries, we never would have known that this data is actually really different.
- I want to show you one more really cool thing.
- The datasauRus package.
- The datasauRus creates plots with the Anscombe data in different shapes.
- But let's run it to see that for ourselves.
- First, you'll start off with installing and loading the package.
- Then we'll create a chart.
- It's okay at these commands seem complicated.
- You'll be creating your own plot soon.
- This is just a sneak peek at how R can help you create data visualizations.
- When we run this, it shows us several different plots.
- There's the famous dinosaur, a bull's eye, a star, R is a pretty powerful visualization tool.
- You could use the relationships between data points to create many other shapes.
- As you can see, you can do a lot of things with R.
- Data visualizations like the ones we just explored help you discover so much more about the data you're working with.
- It's important to explore your data in multiple ways to learn a little more about its story.
- Next, we'll learn how to use R functions to check for bias.

## Questions & Notes

Anscomebe's quartet: have four datasets that have nearly identical summary statistics

**Note**: You will have a chance in later lessons to create more plots using the datasauRus and ggplot packages. If you are currently following along in R Studio, here is the code syntax that will create the datasauRus plots shown in the video:

```r
install.packages('datasauRus') #run the code

library('datasauRus') #run the code

ggplot(datasaurus_dozen,aes(x=x,y=y,colour=dataset))+geom_point()+theme_void()+theme(legend.position = "none")+facet_wrap(~dataset,ncol=3)  #run the code
```

## My wrapped Keypoints

In this section, titled "Same data, different outcome," the video explores Anscombe's quartet, a famous example demonstrating the importance of data visualization in understanding datasets. Here's a breakdown of the key points from the video:

1. **Introduction to Anscombe's Quartet:**
   - Anscombe's quartet consists of four datasets that have nearly identical summary statistics but exhibit different patterns when visualized.

2. **Importance of Data Visualization:**
   - While summary statistics might suggest datasets are identical, visualizations help uncover hidden patterns and differences within the data.

3. **Working with the Quartet Data:**
   - The quartet data contains four sets of x and y coordinates, representing different datasets.
   - Statistical measures such as mean, standard deviation, and correlation are calculated for each dataset.

4. **Creating Visualizations:**
   - Simple graphs are generated to visually represent the datasets and observe their differences.
   - Despite identical summary statistics, the datasets appear distinct when visualized.

5. **Introduction to DatasauRus Package:**
   - The DatasauRus package is introduced, which creates plots of the Anscombe data in various shapes.
   - Running the package generates plots resembling shapes such as a dinosaur, a bull's eye, and a star.

6. **Importance of Data Exploration:**
   - Exploring data through visualizations helps uncover insights and understand the story behind the data.
   - Multiple approaches to data exploration, including statistical summaries and visualizations, are essential for gaining a comprehensive understanding of datasets.

Overall, the section highlights the significance of data visualization in complementing statistical analysis and emphasizes the value of exploring data from different perspectives to gain deeper insights.