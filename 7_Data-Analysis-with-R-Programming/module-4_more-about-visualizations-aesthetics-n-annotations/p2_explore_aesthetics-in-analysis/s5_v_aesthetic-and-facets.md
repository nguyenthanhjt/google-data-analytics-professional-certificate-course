# Video: Aesthetics and facets

Video transcript

- Welcome back.
- In this video, we'll learn how to use the ggplot2 facet functions to display our data in new ways.
- Facet functions let you display smaller groups or subsets of your data.
- A facet is a side or section of an object, like the sides of a gemstone.
- Facets show different sides of your data by placing each subset on its own plot.
- Faceting can help you discover new patterns in your data and focus on relationships between different variables.
- For example, let's say you're looking at sales data for a clothing company.
- You might want to break down your data by category to show specific trends: children's clothing versus adult clothing, or spring fashions versus fall fashions.
- Or if you are running an employee engagement survey, you might want to break down your data by tenure and compare senior employees to new employees.
- Ggplot2 has two functions for faceting; Facet underscore wrap and facet underscore grid.
- Let's explore them both.
- We will start with facet underscore wrap.
- To facet your plot by a single variable, use facet underscore wrap.
- Let's say we wanted to focus on the data for each species of penguin.
- Take our plot that shows the relationship between body mass and flipper length in each penguin species.
- The facet underscore wrap function lets us create a separate plot for each species.
- To add a new layer to our plot, we'll add a plus symbol to our code.
- Then inside the parentheses of the facet underscore wrap function, type a tilde symbol, followed by the name of the variable.
- Let's log into RStudio Cloud and check it out.
- As a reminder, we'll start by loading the ggplot2 package and the penguins dataset.
- You can find the tilde symbol in the upper-left corner of your keyboard, just below the escape key.
- The separate plots show the relationship between body mass and flipper length within each species of penguin.
- Pretty cool, right? Facets help us focus on important parts of our data that we might not notice in a single plot.
- If your is visual is too busy, for example, if it's got too many variables or levels within variables, faceting can be a good option.
- Let's try faceting the diamonds dataset.
- Earlier, we made a bar chart that showed the number of diamonds for each category of cut.
- Fair, good, very good, premium, and ideal.
- We can use facet underscore wrap on the cut variable to create a separate plot for each category of cut.
- Let's check it out.
- To facet your plot with two variables, use the facet underscore grid function.
- Facet underscore grid will split the plot into facets vertically by the values of the first variable and horizontally by the values of the second variable.
- For example, we can take our penguins plot and use facet underscore grid with the two variables, sex and species.
- In the parentheses following the facet underscore grid function, we write sex, then the tilde symbol, then species.
- Let's run the code.
- There are nine separate plots, each based on a combination of the three species of penguin and three categories of sex.
- Facet underscore grid lets you quickly reorganize and display complex data and makes it easier to spot relationships between different groups.
- If we want, we can focus our plot on only one of the two variables.
- For example, we can tell R to remove sex from the vertical dimension of the plot and just show species.
- Let's check it out.
- You can easily spot differences in the relationship between flipper length and body mass between the three species.
- In the same way, we can focus our plot on sex instead of species.
- Facets let you reorganize your data to show specific relationships between variables and reveal important patterns and trends in subsets of your data.
- That's all for now.
- Next up, we'll learn how to customize our plots using labels and annotations.
- Until next time.

## Questions & Notes

- Facets: display smaller groups, or subsets of the data
  - A facet is a side or section of an object. Ex: like the sides of a gemstone
  - Facets show different side of the data by placing each subset on its own plot

- **Note**: Since the 'tilde' (~) is a new symbol being introduced for the first time, the definition is as follows:
  - Tilde operator is used to define the relationship between dependent variable and independent variables in a statistical model formula. The variable on the left-hand side of tilde operator is the dependent variable and the variable(s) on the right-hand side of tilde operator is/are called the independent variable(s). So, tilde operator helps to define that dependent variable depends on the independent variable(s) that are on the right-hand side of tilde operator. (retrieved from tutorialspoint.com)
  - In the case of this example, the independent variable at the end of the syntax line would be species, and the dependent variable in this case is facet_wrap. The facet_wrap is actually a function that is being called to separate and distribute the independent data within the plot. 

### Question 1: Facet functions let you display smaller groups, or subsets, of your data

- [x] True
- [ ] False

> Correct:Facet functions let you display smaller groups, or subsets, of your data.

## My wrapped keypoints

Section 5 of the course focuses on "Aesthetics and facets" in ggplot2, introducing how to use facet functions to display data subsets in different plots. Here's a breakdown of the key points from the video transcript:

1. **Introduction to Faceting**: Facet functions in ggplot2 allow users to display smaller groups or subsets of data by placing each subset on its own plot. Faceting helps in discovering new patterns and relationships between variables.

2. **Facet Functions in ggplot2**: There are two main facet functions in ggplot2: `facet_wrap` and `facet_grid`.
    - `facet_wrap`: Facets plots by a single variable, creating separate plots for each level of that variable.
    - `facet_grid`: Facets plots by two variables, splitting the plot into facets vertically and horizontally based on the values of these variables.

3. **Using `facet_wrap`**: To facet a plot by a single variable, such as species in a penguins dataset, users can use `facet_wrap` function followed by the variable name inside parentheses. This creates separate plots for each level of the specified variable.

4. **Example with `facet_wrap`**: The video demonstrates faceting the penguins dataset by species, creating separate plots for each species to visualize the relationship between body mass and flipper length.

5. **Benefits of Faceting**: Faceting helps in focusing on important parts of the data that might not be noticeable in a single plot. It is particularly useful when the visual is too busy or when there are too many variables or levels within variables.

6. **Using `facet_grid`**: To facet a plot by two variables, such as sex and species in the penguins dataset, users can use `facet_grid` function followed by the variables separated by a tilde symbol inside parentheses. This creates a grid of plots based on combinations of the specified variables.

7. **Example with `facet_grid`**: The video demonstrates faceting the penguins dataset by sex and species, creating a grid of plots to visualize relationships between these variables.

8. **Customizing Faceted Plots**: Users can customize faceted plots to focus on specific variables or combinations of variables, allowing for better visualization of patterns and trends in the data.

Faceting provides a powerful tool for exploring and visualizing complex datasets, allowing users to identify patterns and relationships between variables more effectively.
