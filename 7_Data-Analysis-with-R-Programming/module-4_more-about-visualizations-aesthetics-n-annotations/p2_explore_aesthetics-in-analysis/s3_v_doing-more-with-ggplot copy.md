# Video: Doing more with ggplot

Video transcript

- Great to see you again.
- In this video, we'll learn how to use different geom functions to create different types of plots, such as scatter plots and bar charts.
- There are lots of different geoms available.
- You can choose a specific geom based on how you want to represent your data and your goals for communicating it.
- This lets you tell the story of your data in different ways and communicate effectively to different audiences.
- Let's start with two visualizations.
- Both visuals contain the same x-variable and the same y-variable.
- Both use the same data, but each plot uses a different visual object to represent the data.
- One uses points.
- The other uses a smooth line.
- In other words, they use different geoms.
- In ggplot2, a geom is the geometrical object used to represent your data.
- Geoms include points, bars, lines, and more.
- The geom underscore point function uses points to create scatter plots.
- The geom underscore bar function uses bars to create bar charts and so on.
- To change the geom in our plot, we need to change the geom function in our code.
- For example, take the plot that shows the relationship between body mass and flipper length.
- The code uses geom underscore point to create a scatter plot.
- Let's log into RStudio Cloud and watch what happens when we change geoms.
- First, let's load the ggplot2 package and the penguins dataset.
- Now, we can put geom underscore smooth in place of geom underscore point.
- We still have the same data, but now the data's got a different visual appearance.
- Instead of points, there's a smooth line that fits the data.
- The geom underscore smooth function's useful for showing general trends in our data.
- The line clearly shows the positive relationship between body mass and flipper length.
- The larger the penguin, the longer the flipper.
- We can even use two geoms in the same plot.
- Let's say we want to show the relationship between the trend line and the data points more clearly.
- We can combine the code for geom underscore point and the code for geom underscore smooth by adding a plus symbol after geom underscore smooth.
- Let's write the code and run it.
- Let's say we want to plot a separate line for each species of penguin.
- We can add the line type aesthetic to our code and map it to the variable species.
- Geom underscore smooth will draw a different line with a different line type for each species of penguin.
- The legend shows how each line type matches with each species.
- The plot clearly shows the trend for each species.
- Finally, let's check out the geom underscore jitter function.
- The geom underscore jitter function creates a scatter plot and then adds a small amount of random noise to each point in the plot.
- Jittering helps us deal with over-plotting, which happens when the data points in a plot overlap with each other.
- Jittering makes the points easier to find.
- I'll show you what I mean.
- Let's replace geom underscore point with geom underscore jitter.
- Now that we've seen what ggplot2 can do with scatter plots, let's explore bar charts.
- We'll use the diamonds dataset that you're already familiar with.
- This includes data like the quality, clarity, and cut for over 50,000 diamonds.
- This dataset comes with the ggplot2 package, so it's already loaded.
- To make a bar chart, we use the geom underscore bar function.
- Let's write some code that plots a bar chart of the variable cut in the diamonds dataset.
- Cut refers to a diamond's proportions, symmetry, and polish.
- Notice that we didn't supply a variable for the y-axis.
- When you use geom underscore bar, R automatically counts how many times each x-value appears in the data, and then shows the counts on the y-axis.
- The default for geom underscore bar is to count rows.
- But that's only one of the many different applications for bar charts.
- For example, the x-axis of our plot shows five categories of cut quality: fair, good, very good, premium, and ideal.
- The y-axis shows the number of diamonds in each category.
- Over 20,000 diamonds have a value of ideal, which is the most common type of cut.
- Geom underscore bar uses several aesthetics that you're already familiar with, such as color, size, and alpha.
- Let's add the color aesthetic to our plot and map it to the variable cut.
- We write the code the same way as we did with scatter plots and add color equals cut after x equals cut.
- Don't forget to put a comma after x equals cut to add a new aesthetic.
- The color aesthetic adds color to the outline of each bar.
- R also supplies a legend to show the color-coding.
- Let's say, we want to highlight the difference between cuts even more clearly to make our plot easier to understand.
- We can use the fill aesthetic to add color to the inside of each bar.
- In our code, we put fill equals cut in place of color equals cut. R automatically chooses the colors and supplies a legend.
- That looks great.
- I really enjoy using the fill aesthetic.
- If we map fill to a new variable, geom underscore bar will display what's called a stacked bar chart.
- Let's map fill to clarity instead of cut.
- Our plot now shows 40 different combinations of cut and clarity.
- Each combination has its own colored rectangle.
- The rectangles that have the same cut value are stacked on top of each other in each bar.
- The plot organizes the complex data.
- Now we know the difference in volume between cuts and we can figure out the difference in clarity within each cut.
- This is just the beginning of what you can do with geoms.
- Ggplot2 has over 30 geom functions that you can use to make plots, and extension packages give you even more.
- The ggplot2 cheat sheet is a great resource for learning more about geoms.
- As you move forward and do more advanced data analysis, you'll find plenty of new geoms to work with.
- Until then, the geoms we just reviewed will keep you busy and let you do a lot with your data.
- Coming up, we'll learn how to use the facet functions to display our data in different ways.
- Bye for now.

## My wrapped keypoints

Section 3 of the course covers "Doing more with ggplot," focusing on the utilization of different geom functions to create various types of plots in R. Here's a breakdown of the key points from the video transcript:

1. **Introduction to Geoms**: Geoms (geometrical objects) are used in ggplot2 to represent data visually. Examples include points, bars, lines, and more. Different geoms are chosen based on the data and the desired method of communication.

2. **Scatter Plots with Geoms**: The video starts by demonstrating scatter plots using `geom_point` to represent data points. It then introduces `geom_smooth` to fit a smooth line to the data, providing a general trend.

3. **Combining Geoms**: Users can combine multiple geoms in the same plot to highlight different aspects of the data. For example, combining `geom_point` and `geom_smooth` shows both data points and trend lines.

4. **Customizing Geoms**: Geoms can be customized using aesthetics such as color, shape, size, and alpha. These aesthetics help differentiate data points or add additional layers of information to the plot.

5. **Dealing with Over-plotting**: Over-plotting occurs when data points overlap, making it difficult to distinguish individual points. `geom_jitter` adds random noise to each point, making them easier to identify.

6. **Bar Charts with Geoms**: The video transitions to creating bar charts using `geom_bar` with the diamonds dataset. By default, `geom_bar` counts the frequency of each category on the x-axis and displays it on the y-axis.

7. **Customizing Bar Charts**: Aesthetics like color and fill can be applied to bar charts to enhance visual appeal and highlight differences between categories. Stacked bar charts can be created by mapping the `fill` aesthetic to a variable other than the x-axis variable.

8. **Exploring More Geoms**: ggplot2 offers over 30 geom functions, providing a wide range of options for creating plots. The ggplot2 cheat sheet is recommended for further exploration of geoms.

Overall, the video provides a comprehensive overview of how to utilize different geoms to create visually appealing and informative plots in R using ggplot2. It demonstrates practical examples and encourages further exploration of geoms for advanced data analysis.