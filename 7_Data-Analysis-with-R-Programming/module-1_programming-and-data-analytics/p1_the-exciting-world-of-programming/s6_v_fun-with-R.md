# Video: Fun with R

Video transcript

- Hi, great to see you again.
- When I first learned R, it was the visuals that really got me hooked.
- I still think it's so cool that you can write a little bit of code, press a button and, presto, out pops an awesome data visualization.
- Before we get into all the details, I thought it would be fun to give you a quick sneak peek and show you what R can do.
- What follows will be a preview of what you're going to learn.
- By the end of this course, you'll not only understand all this code, you'll be able to write and execute it as well.
- For now, just sit back, relax and enjoy the show.
- Let's start by loading a library and getting a dataset to work with.
- We can use the palmer penguins dataset, which contains size measurements for three penguin species that live on the Palmer Archipelago in Antarctica.
- This includes data on stuff like body mass, flipper length and bill length.
- The dataset has 344 rows of information sorted into eight columns.
- The palmer penguins data is popular with analysts and is great for fun exploration, visualization and teaching concepts.
- We'll see more of this data set later on in the course.
- Let's say we want to visualize the relationship between body mass and flipper length.
- You may guess the larger the penguin, the longer the flipper.
- We can find out for sure by creating a plot.
- Let's make a scatter plot.
- A scatter plot uses points to display the relationship between two variables.
- So the two variables were going to compare our body mass and flipper length.
- No need to memorize all these details right now.
- You'll have time to learn more about them later on.
- Let's check out the parts of this code and how they fit together.
- The first function starts the plot.
- If we run the code at this point, all we get is a blank plot.
- If we add some more code, R will put labels on each access of our plot and add lines for data.
- Body mass is on the y-axis and flipper length is on the x-axis, but the data points are not yet visible.
- To get the complete plot, we can add some more code that tells R how to represent our data.
- For example, we could use points, bars or lines.
- We'll use points to create a scatter plot.
- We can go further.
- For example, we can change how the plot looks.
- Let's change the color of all of the points to purple.
- You can hit the Up arrow to pull up the last piece of code you ran, so we'll do that now.
- And then we'll add in color equals purple inside geom point.
- Now we can hit Enter to run this.
- We can also add new information to the plot and use color to highlight it.
- Let's tell R to assign a different color to each species of penguin.
- This way we can link data points to each group of penguins.
- Gentoos are the largest.
- The legend just to the right of the plot shows us that the blue points refer to the Gentoos.
- R automatically creates a legend for the plot to help us understand the color-coding.
- R does everything you tell it to do and even does stuff you don't ask for.
- It's just that helpful.
- We can also use shape to highlight the different penguin species.
- Or we can use both color and shape.
- In addition to highlighting our data, we can also reorganize it.
- We can break our data down into smaller groups or subsets and create a plot for each subset.
- Let's say we want to focus on the data for each species.
- Facet functions let us create a separate plot for each species.
- Check this out.
- Facets are so great.
- We can even put text on our plot to point to specific data or communicate a message.
- Let's give our plot a title to clearly indicate its purpose.
- Finally, we can save our plot, so we can access or share it later on.
- Now, if we click on the Files tab, we'll find our file in the list.
- Let's open it up.
- Well, that's the end of the show.
- I hope you enjoyed it as much as I did.
- We were able to take a big dataset and quickly visualize some significant patterns.
- These are some of the basic functions in R.
- In other words, this is just the beginning.
- It's exciting to think of all the ways R can help you realize the full power of data analysis.
- As you move forward, you learn more about each of the functions we use to create our plots.
- By the end of this course, you'll be the one writing and executing all of this code.
- Coming up, we'll learn more about computer programming and how it can help you analyze your data.
- See you soon.

## Questions & Notes

Friendly reminder- the remainder of this video is a preview to show you what R can do, and what you'll be learning throughout this course.

You do not need to follow along. Just sit back, relax, and enjoy the show. `:)`

## Keypoints from **Video: Fun with R**

- The video provides a sneak peek into what learners will explore in the course, showcasing the capabilities of R for data visualization and analysis.
- The Palmer Penguins dataset is introduced, containing size measurements for penguin species living on the Palmer Archipelago in Antarctica.
- A scatter plot is created to visualize the relationship between body mass and flipper length, demonstrating how R can represent data visually.
- Various customization options are explored, such as changing point colors and shapes to differentiate between penguin species.
- The use of facets to create separate plots for each penguin species is demonstrated, along with adding titles and saving plots for future reference.
- The video concludes by emphasizing that this demonstration is just the beginning, with learners set to explore more advanced functions in R throughout the course.