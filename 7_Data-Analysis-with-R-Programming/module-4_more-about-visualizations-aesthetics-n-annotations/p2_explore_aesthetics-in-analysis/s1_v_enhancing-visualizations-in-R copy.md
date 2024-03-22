# Video: Enhancing visualizations in R

Video transcript

- Hello again.
- In this video, you'll learn how to change the aesthetics of your visuals, which can help you present your data in a more compelling way.
- With aesthetics, you can highlight key points in your data and communicate more clearly and effectively with your stakeholders.
- Earlier, we learned that an aesthetic is a visual property of an object in your plot.
- For example, in a scatter plot, aesthetics include the size, shape or color of your data points.
- You can display a point in different ways by changing its aesthetics or the way it looks.
- You can make a point small, triangular or blue or a combination of these.
- Let's go back to our penguins dataset and review the code for our plot that shows the relationship between body mass and flipper length.
- As a quick refresher the mapping equals aes part of the code tells R what aesthetics to use for the plot.
- You use the aes function to define the mapping between your data and your plot.
- Mapping means matching up a specific variable in your dataset with a specific aesthetic.
- For example, you can map a variable to the x-axis of your plot or you can map a variable to the y-axis of your plot.
- To map an aesthetic to a variable, set the name of the aesthetic equal to the name of the variable inside the parentheses of the aes function.
- Our code tells R to map flipper length to the x-axis and body mass to the y-axis.
- Let's log into RStudio Cloud and run the code.
- As a quick reminder, let's start by loading the ggplot2 package and the penguins dataset.
- R will automatically place the appropriate label on each axis of our scatter plot.
- After you map a variable to an aesthetic R takes care of the rest.
- You can also map data to other aesthetics, like color, size and shape.
- Right now, our plot's in black and white.
- It clearly shows the positive relationship between the two variables.
- As the values on the x-axis increase, the values on the y-axis increase.
- But it's also got some limitations.
- For example, we can't tell which data points refer to each of the three penguin species.
- To solve this problem, we can map a new variable to a new aesthetic.
- Let's add a third variable to our scatter plot by mapping it to a new aesthetic.
- We'll map the variable species to the aesthetic color by adding some code inside the parentheses of the aes function.
- We'll add a comma after the body mass variable and type color equals sign species.
- Our code tells R to assign a different color to each species of penguin.
- Let's check it out.
- The Gentoo are the largest of the three penguin species.
- The legend just to the right of the plot shows us that the blue points refer to the Gentoo penguins.
- Not only does R automatically apply different colors to each data point, it also gives a legend to show us the color-coding.
- That's what I love about R.
- Give it just a little bit of code, and it will go the extra mile to help you out.
- We can also use shape to highlight the different penguin species.
- Let's map the variable species to the aesthetic shape.
- To do this, we can change the code from color equal species to shape equal species.
- Instead of colored points, R assigns different shapes to each species.
- Now the legend shows us a circle for the Adelie species, a triangle for the Chinstraps and a square for the Gentoos.
- You might notice that our plot's in black and white again because we removed the code for color.
- Let's put some color back into our plot.
- If we want we can map more than one aesthetic to the same variable.
- Let's map both color and shape to species.
- We'll add the code color equals species while keeping the code shape equal species.
- Now our plot shows a different color and a different shape for each species.
- We can keep going.
- Let's add size as well and map three aesthetics to species.
- If we add size equal species, each colored shape will also be a different size.
- Using more than one aesthetic can also be a way to make your visuals more accessible because it gives your viewers more than one way to make sense of your data.
- We can also map species to the alpha aesthetic, which controls the transparency of the points.
- Our first plot showed the relationship between body mass and flipper length in black and white.
- Then we mapped the variable species to the aesthetic color to show the difference between each of the three penguin species.
- If we want to keep our graph in black and white, we can map the alpha aesthetic to species.
- This will make some points more transparent or see-through than others.
- This gives us another way to represent each penguin species.
- Let's try it.
- Alpha is a good option when you've got a dense plot with lots of data points.
- You can also set the aesthetic apart from a specific variable.
- Let's say we want to change the color of all the points to purple.
- Here we don't want to map color to a specific variable like species.
- We just want every point in our scatter plot to be purple.
- So we need to set our new piece of code outside of the aes function and use quotation marks for our color value.
- This is because all the code inside of the aes function tells R how to map aesthetics to variables.
- For example, mapping the aesthetic color to the variable species.
- If we want to change the appearance of our overall plot without regard to specific variables, we write code outside of the aes function.
- Let's write the code and run it.
- That's all for now.
- We just learned about the most common aesthetics for points: x y, color, shape, size and alpha.
- We also discovered how aesthetics can change the look of our plot and highlight important data.
- We've covered a lot so far and learned a bunch of new concepts.
- It takes time to process new information and learn new skills, so feel free to watch any of these videos again if you need a refresher or want to practice in RStudio.
- Coming up, we'll learn more about geoms.
- See you then.

## Questions & Notes & Practice along with video

### Question 1: In ggplot2, which of the following concepts refers to the shape, color, and size of data points in a plot?  

- [ ] Geoms
- [ ] Annotations
- [x] Aesthetics
- [ ] Facets

> Correct: In ggplot2, the shape, color, and size of data points in a plot refers to the concept of aesthetics.

```r
#install.packages("ggplot2")
#install.packages("palmerpenguins")

library(ggplot2)
library(palmerpenguins)

data("penguins")
View(penguins)

# basic
ggplot(data = penguins) +
  geom_point(
    mapping = aes(x = flipper_length_mm,  y = body_mass_g)) 

# Limitations: data points do not refer to each of the three penguin species
# -> add color mapping in aes()
ggplot(data = penguins) +
  geom_point(
    mapping = aes(x = flipper_length_mm,  y = body_mass_g, color = species)) 

# -> use shape to highlight each species
ggplot(data = penguins) +
  geom_point(
    mapping = aes(x = flipper_length_mm,  y = body_mass_g, shape = species)) 

# map both color and shape
ggplot(data = penguins) +
  geom_point(mapping = aes(
    x = flipper_length_mm,
    y = body_mass_g,
    shape = species,
    color = species
  )) 

# add size 
ggplot(data = penguins) +
  geom_point(mapping = aes(
    x = flipper_length_mm,
    y = body_mass_g,
    shape = species,
    color = species,
    size = species
  )) 

## other syntax
ggplot(data = penguins) +
  geom_point(
    mapping = aes(
      x = flipper_length_mm,
      y = body_mass_g,
      shape = species,
      color = species,
      size = species
    )
  ) 

# add `alpha` mapping in aes() when getting dense plot with lots of data points
ggplot(data = penguins) +
  geom_point(
    mapping = aes(
      x = flipper_length_mm,
      y = body_mass_g,
      alpha = species
    )
  ) 

# change appearence of overall plot without regard to specific variables,
# -> write code inside geom_fn() but outside the aes() fn 

# change color of all data point: add color ='color-name'
ggplot(data = penguins) +
  geom_point(
    mapping = aes(
      x = flipper_length_mm,
      y = body_mass_g,
      alpha = species
    ), color = "purple"
  ) 

```

## My wrapped keypoint

Section 1 of Part 2 focuses on enhancing visualizations in R through the manipulation of aesthetics. Here are the key points from the video transcript:

1. **Introduction to Aesthetics**: Aesthetics are visual properties of objects in plots, such as size, shape, or color of data points. By changing aesthetics, users can effectively highlight key points in their data and communicate more clearly with stakeholders.

2. **Mapping Aesthetics**: Mapping involves matching specific variables in the dataset with specific aesthetics in the plot. The `aes()` function is used to define these mappings, specifying which variable corresponds to which aesthetic property.

3. **Example with Penguins Dataset**: Using the penguins dataset, the video demonstrates how to create a scatter plot showing the relationship between body mass and flipper length. Initially, the plot is in black and white, making it challenging to distinguish between data points representing different penguin species.

4. **Color Aesthetic**: To differentiate between penguin species, the `color` aesthetic is mapped to the `species` variable. This assigns different colors to each species and includes a legend for clarity.

5. **Shape Aesthetic**: Similarly, the `shape` aesthetic is mapped to the `species` variable, assigning different shapes to each species. This also includes a legend for reference.

6. **Multiple Aesthetics**: Multiple aesthetics can be mapped to the same variable, providing additional layers of distinction in the plot. In the example, both color and shape are mapped to the `species` variable.

7. **Additional Aesthetics**: Other aesthetics such as `size` and `alpha` can also be utilized to further enhance the plot. The `alpha` aesthetic controls the transparency of points, which is particularly useful for dense plots with many data points.

8. **Customizing Appearance**: Aesthetics can be customized not only based on variables but also independently to change the overall appearance of the plot. This involves setting properties outside the `aes()` function using quotation marks.

9. **Summary and Next Steps**: The video concludes by summarizing the aesthetics covered (x, y, color, shape, size, alpha) and their role in enhancing visualizations. Viewers are encouraged to review the content and practice in RStudio to reinforce their understanding.

Overall, the video provides a comprehensive overview of aesthetics in R visualizations and demonstrates their practical application using the ggplot2 package.