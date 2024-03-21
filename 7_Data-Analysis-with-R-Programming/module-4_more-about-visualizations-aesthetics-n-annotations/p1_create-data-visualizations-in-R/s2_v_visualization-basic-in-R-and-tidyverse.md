# Video: Visualization basics in R and tidyverse

Video transcript

- Hi again, in this video we'll focus on ggplot2.
- We'll learn about its main features and functions and how it can help you visualize your data.
- First, let's talk about some different visualization packages you can use with R.
- Base R has its own package and there are other useful packages you can add.
- They'll help you do almost anything you want with your data from making simple pie charts, to creating more complex visuals like interactive graphs and maps.
- General-purpose packages like Plotly let you do a wide range of visualization functions.
- Others like RGL, focus on specific solutions like 3D visuals.
- Some of the most popular include ggplot2, Plotly, Lattice, RGL, Dygraphs, Leaflet, Highcharter, Patchwork, gganimate and ggridges.
- Personally, ggplot2 is my favorite for data analysis.
- It's both powerful and flexible.
- With a little bit of code, you can create all kinds of different plots.
- You can use ggplot2 on its own or extend its powers with other packages.
- Plus it's the most popular visualization package in R.
- A lot of data analysts prefer to use ggplot2 which is why we're using ggplot2 here.
- Ggplot2 was originally created by the statistician and developer Hadley Wickham in 2005.
- Wickham's inspiration for creating ggplot2 came from the 1999 book The Grammar of Graphics, a scholarly study of data visualization by computer scientist Leland Wilkinson.
- The first two letters of ggplot2 actually stand for grammar of graphics.
- And in the same way the grammar of a human language gives us rules to build any kind of sentence, the grammar of graphics gives us rules to build any kind of visual.
- So ggplot2 has some basic building blocks that you can use to create plots.
- In other words when you learn the basic steps for creating a plot in ggplot2, you can reuse these steps to create lots of different kinds of plots.
- Plus, you can add or remove layers of detail to your plot without changing its basic structure or the underlying data.
- This makes ggplot2 really powerful.
- In the next video, we'll go over these steps one by one.
- Ggplot2 has lots of other benefits too.
- You can create all different types of plots including scatter plots, bar charts, line diagrams and tons more.
- You can change the colors, layout and dimensions of your plots and add text elements like titles, captions and labels.
- With just a little bit of code you can create high-quality visuals.
- Plus ggplot2 lets you combine data manipulation and visualization using the pipe operator.
- Ggplot2 also has tons of functions that cover all your data viz needs.
- To give you an idea, check out the ggplot2 cheat sheet, which is a popular reference guide.
- You can find out more about the ggplot2 cheat sheet in an upcoming reading.
- It's not important to learn all these functions right away or even know what they are.
- Over time as you get into more advanced data analysis, you can learn about new functions as you need them.
- Just know that if you need to find a function for something, ggplot2 probably has it.
- And like we discussed, even the basic functions of ggplot2 let you do so much.
- We'll focus on some core concepts in ggplot2: aesthetics, geoms, facets, labels and annotations.
- These might be new concepts to you and that's okay.
- We'll learn about them together and soon we'll explore each in detail.
- For now let's get a quick preview.
- In ggplot2 an aesthetic is a visual property of an object in your plot.
- For example, in a scatter plot aesthetics include things like the size, shape or color of your data points.
- Think of an aesthetic as a connection or mapping between a visual feature in your plot and a variable in your data.
- We'll talk more about mapping later on.
- A geom refers to the geometric object used to represent your data.
- For example, you can use points to create a scatter plot, bars to create a bar chart, or lines to create a line diagram.
- You can choose a geom to fit the type of data you have.
- Points show the relationship between two quantitative variables.
- Bars show one quantitative variable varies across different categories.
- Up next, we'll talk about the facet function.
- Facets let you display smaller groups or subsets of your data.
- With facets, you can create separate plots for all the variables in your dataset.
Finally, the label and annotate functions let you customize your plot.
- You can add text like titles, subtitles and captions to communicate the purpose of your plot or highlight important data.
- That's all for now.
- Coming up, we'll use code to create our own first plot in ggplot2.

## Questions & Notes

### Question: Fill in the blank: In ggplot2, an _____ is a visual property of an object in your plot

- [x] aesthetic
- [ ] argument
- [ ] annotation
- [ ] alpha

> Correct: In ggplot2, an aesthetic is a visual property of an object in your plot.

## My wrapped keypoints

1. **Visualization Packages in R**: Various packages are available in R for creating visualizations, including ggplot2, Plotly, Lattice, RGL, Dygraphs, Leaflet, Highcharter, Patchwork, gganimate, and ggridges. Each package offers different functionalities, ranging from simple charts to complex interactive graphs and maps.

2. **Introduction to ggplot2**: ggplot2 is highlighted as a powerful and flexible visualization package preferred by many data analysts due to its versatility and popularity. It was created by Hadley Wickham in 2005, inspired by the book "The Grammar of Graphics" by Leland Wilkinson.

3. **Grammar of Graphics**: The name ggplot2 stands for "grammar of graphics," which provides a framework for building various types of visualizations using basic building blocks. These building blocks allow users to create different plots by reusing basic steps and adding or removing layers of detail without changing the plot's structure or underlying data.

4. **Benefits of ggplot2**: ggplot2 offers numerous benefits, including the ability to create different types of plots (scatter plots, bar charts, line diagrams, etc.), customize colors, layout, and dimensions, add text elements like titles and labels, and combine data manipulation and visualization using the pipe operator. Additionally, ggplot2 provides a wide range of functions to cover various data visualization needs.

   - Create different types of plots
   - Customize the look and feel of plots
   - Create hight quality visuals
   - Combine data manipulation and visualizations using pipe operator

5. **Core Concepts in ggplot2**: The video previews core concepts in ggplot2, including aesthetics, geoms, facets, labels, and annotations. Aesthetics represent visual properties of plot objects, geoms refer to geometric objects used to represent data, facets allow displaying subsets of data, and labels and annotations enable customization of plots with text elements.

   - **Aesthetics**: a visual property of an object in a plot(example in scatter plot: size, shape of data points,...)
   - **Geoms**: the geometric object used to represent your data
   - **Facets**: let us to display smaller group, or subsets of our data
   - **Labels and annotations**: customize the plot