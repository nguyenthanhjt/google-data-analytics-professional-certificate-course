# Practice Quiz: Test your knowledge on aesthetics in analysis

## Question 1:  Which of the following aesthetics attributes can you map to the data in a scatterplot? Select all that apply

- [x] Color
- [x] Size
- [ ] Text
- [x] Shape

> Correct: You can map the color, shape, and size aesthetics to the data in a scatterplot.

## Question 2:  Which of the following functions let you display smaller groups, or subsets, of your data?

- [ ] geom_point()
- [ ] geom_bar()
- [x] facet_wrap()
- [ ] ggplot()

> Correct: The facet_wrap() function lets you display smaller groups, or subsets, of your data.

## Question 3:  What is the role of the x argument in the following code?

```R∂
ggplot(data = diamonds) +
     geom_bar(mapping = aes(x = cut))
```

- [ ] A function
- [ ] A variable
- [x] An aesthetic
- [ ] A dataset

> Correct: X is an aesthetic that refers to the x-axis of the plot. The x aesthetic maps the variable cut from the diamonds dataset to the x-axis of the plot.

## Question 4:  A data analyst creates a scatterplot with a lot of data points. It is difficult for the analyst to distinguish the individual points on the plot because they overlap. What function could the analyst use to make the points easier to find?

- [x] geom_jitter()
- [ ] geom_line()
- [ ] geom_point()
- [ ] geom_bar()

> Correct: The analyst could use the geom_jitter() function to make the points easier to find. The geom_jitter() function adds a small amount of random noise to each point in the plot, which helps deal with the overlapping of points.

