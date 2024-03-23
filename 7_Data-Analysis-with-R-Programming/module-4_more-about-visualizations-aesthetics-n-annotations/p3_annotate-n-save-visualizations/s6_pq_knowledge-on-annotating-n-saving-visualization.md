# Practice Quiz: Test your knowledge on annotating and saving visualizations

## Questions 1:  Which of the following are benefits of adding labels and annotations to your plot? Select all that apply

- [x] Indicating the main purpose of your plot
- [x] Highlighting important data in your plot
- [x] Helping stakeholders quickly understand your plot
- [ ] Choosing a geom for your plot

> Correct: The benefits of adding annotations to your plot include indicating the main purpose of your plot, highlighting important data in your plot, and helping stakeholders quickly understand your plot.

## Questions 2:  A data analyst is creating a plot for a presentation to stakeholders. The analyst wants to add a caption to the plot to help communicate important information. What function could the analyst use?

- [ ] The geom_bar() function
- [x] The labs() function
- [ ] The facet_wrap() function
- [ ] The geom_point() function

> Correct: The analyst could use the labs() function to add a caption to the plot.

## Questions 3:  What function can you use to put a text label inside the grid of your plot to call out specific data points?

- [ ] The aes() function
- [ ] The facet_wrap() function
- [x] The annotate() function
- [ ] The labs() function

> Correct: You can use the annotate() function to put a text label inside the grid of your plot to call out specific data points.

## Questions 4:  You are working with the penguins dataset. You create a scatterplot with the following code

```R
ggplot(data = penguins) +
geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```

You want to use the labs() function to add the title “Penguins” to your plot. Add the code chunk that lets you add the title "Penguins" to your plot.

Where does your visualization display the title?

- [ ] The lower left
- [ ] The upper right
- [x] The upper left
- [ ] The lower right

> Correct: You add the code chunk labs(title = “Penguins”) to add the title "Penguins" to your plot. Inside the parentheses of the labs() function, write the word title, then an equals sign, then the specific text of the title in quotation marks. The labs() function lets you add labels to your plot.
>
> Your visualization displays the title in the upper left.
