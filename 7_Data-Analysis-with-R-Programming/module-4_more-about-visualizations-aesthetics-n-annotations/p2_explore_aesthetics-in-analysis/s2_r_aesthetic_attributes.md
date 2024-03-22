# Reading: Aesthetic attributes

In this reading, you will learn about the three basic aesthetic attributes to consider when creating ggplot2 visualizations in R: color, size, and shape. These attributes are essential tools for creating data visualizations with ggplot2 and are built directly into its code.

![Image of a triangle, sphere, and cube that are different colors and sizes. The shapes all have eyes and smiling expressions.](./resources/img-1.png)

## Aesthetics in ggplot2

ggplot2 is an R package that allows you to create different types of data visualizations right in your R workspace. In ggplot2, an aesthetic is defined as a visual property of an object in your plot.

There are three aesthetic attributes in ggplot2:

- Color: this allows you to change the color of all of the points on your plot, or the color of each data group
- Size: this allows you to change the size of the points on your plot by data group
- Shape: this allows you to change the shape of the points on your plot by data group

Here’s an example of how aesthetic attributes are displayed in R:

```R
ggplot(data, aes(x=distance, y= dep_delay, color=carrier, size=air_time, shape = carrier)) 
      geom_point()
```

By applying these aesthetic attributes to your work with ggplot2, you can create data visualizations in R that clearly communicate trends in your data.

## Additional resources

For more information about aesthetic attributes, check out these resources:

- [Data visualization with ggplot2 cheat sheet](https://ggplot2.tidyverse.org/): RStudio’s cheat sheet is a great reference to use while working with ggplot2. It has tons of helpful information, including explanations of how to use geoms and examples of the different visualizations that you can create.
- [RDocumentation aes function](https://www.rdocumentation.org/packages/ggplot2/versions/3.3.3/topics/aes): This guide describes the syntax of the aes function and explains what each argument does.
