# Practice Quiz: Test your knowledge on data visualizations in R

## Question 1: In ggplot2, you can use the `ggplot()` function to specify the data frame to use for your plot

- [ ] abs()
- [ ] geom_point()
- [x] ggplot()
- [ ] aes()

> Correct: In ggplot2, you can use the ggplot() function to specify the data frame to use for your plot.

## Question 2: In ggplot2, you use the plus sign (+) to add a layer to your plot

- [x] True
- [ ] False

> Correct: In ggplot2, you use the plus sign (+) to add a layer to your plot.

## Question 3: In ggplot2, what function do you use to map variables in your data to visual features of your plot?

- [x] The aes() function
- [ ] The geom_point() function
- [ ] The geom_bar() function
- [ ] The ggplot() function

> Correct: in ggplot2, you use the aes() function to map variables in your data to visual features of your plot. These features are known as aesthetics.

## Question 4: What type of plot will the following code create?

```R
ggplot(data = penguins) +
     geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```

- [x] Scatterplot
- [ ] Bar chart
- [ ] Boxplot
- [ ] Line diagram

> Correct: The code will create a scatterplot. The function geom_point() uses points to create a scatterplot.