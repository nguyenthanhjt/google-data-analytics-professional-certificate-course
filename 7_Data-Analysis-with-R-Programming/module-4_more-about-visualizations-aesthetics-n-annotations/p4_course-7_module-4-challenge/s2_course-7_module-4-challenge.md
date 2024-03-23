# Course 7 Module 4 challenge

## Question 1:  Which of the following are operations you can perform in ggplot2? Select all that apply

- [x] Create scatterplots and bar charts
- [x] Automatically clean data before creating a plot
- [x] Add a title and subtitle to your plot
- [ ] Change the colors and dimensions of your plot

## Question 2:  In ggplot2, what symbol do you use to add layers to your plot?

- [ ] The ampersand symbol (&)
- [ ] The pipe operator (%>%)
- [ ] The equals sign (=)
- [x] The plus sign (+)

## Question 3:  A data analyst creates a plot using the following code chunk

```R
ggplot(data = buildings) +
geom_bar(mapping = aes(x = construction_year, color = height))
```

Which of the following represents an aesthetic attribute in the code chunk?

- [ ] ggplot
- [ ] construction_year
- [x] x
- [ ] buildings

## Question 4:  Which code snippet will make all of the bars in the plot purple?

- [ ]

    ```r
    ggplot(data = buildings) +
    geom_bar(mapping = aes(x = construction_year, color=height))
    ```

- [ ]

    ```r
    ggplot(data = buildings) + 
    geom_bar(mapping = aes(x = construction_year, color=”purple”))
    ```

- [x]

    ```r
    gplot(data = buildings) +
    geom_bar(mapping = aes(x = construction_year), color=”purple”)
    ```

- [ ]

    ```r
    ggplot(data = buildings) + 
    geom_bar(mapping = aes(x = construction_year)) +
    color(“purple”)
    ```

## Question 5:  A data analyst is working with the following plot and gets an error caused by a bug. What is the cause of the bug?

```R
ggplot(data = penguins) %>%
  geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```

- [ ] The pipe should be at the beginning of the second line.
- [x] The code uses a pipe instead of a plus sign.
- [ ] A missing closing parenthesis needs to be added.
- [ ] A function name needs to be capitalized.

## Question 6:  You are working with the penguins dataset. You create a scatterplot with the following code

```R
ggplot(data = penguins) +
    geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g))
```

You want to highlight the different years of data collection on your plot. Add a code chunk to the second line of code to map the aesthetic size to the variable year.

```R
geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g, size = year))
```

What years does your visualization display?

- [x] 2007-2009
- [ ] 2006-2010
- [ ] 2007-2011
- [ ] 2005-2009

> Correct : You add the code chunk size = year to map the aesthetic size to the variable year. The correct code is ggplot(data = penguins) + geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g, size = year)). Inside the parentheses of the aes() function, after the comma that follows y = body_mass_g, write the aesthetic (size), then an equals sign, then the variable (year). The data points for the different years now appear in different sizes.
>
> Your visualization displays the years 2007-2009.

## Question 7:  Which aesthetic of the geom_smooth function can be used to change the style of the line?

- [ ] linestyle
- [ ] linelook
- [x] linetype
- [ ] line

## Question 8:  You are working with the diamonds dataset. You create a bar chart with the following code

```R
ggplot(data = diamonds) +
    geom_bar(mapping = aes(x = color, fill = cut))
```

You want to use the facet_wrap() function to display subsets of your data. Add the code chunk that lets you facet your plot based on the variable cut.

```R
    facet_wrap(~ cut)
```

How many subplots does your visualization show?

- [ ] 4
- [ ] 3
- [ ] 6
- [x] 5

> Correct: You add the code chunk facet_wrap(~cut) to facet your plot based on the variable cut. The correct code is ggplot(data = diamonds) + geom_bar(mapping = aes(x = color, fill = cut)) + facet_wrap(~cut). Inside the parentheses of the facet_wrap() function, write a tilde symbol (~) followed by the name of the variable you want to facet. The facet_wrap() function lets you display subsets of your data.
>
> Your visualization shows 5 subplots.

## Question 9:  A data analyst uses the annotate() function to create a text label for a plot. Which attributes of the text can the analyst change by adding code to the argument of the annotate() function? Select all that apply

- [x] Change the color of the text.
- [x] Change the size of the text.
- [x] Change the font style of the text.
- [ ] Change the text into a title for the plot.

## Question 10: You are working with the penguins dataset. You create a scatterplot with the following lines of code

```R
ggplot(data = penguins) +
  geom_point(mapping = aes(x = flipper_length_mm, y = body_mass_g)) +
```

What code chunk do you add to the third line to save your plot as a png file with “penguins” as the file name?

- [x] ggsave(“penguins.png”)
- [ ] ggsave(“penguins”)
- [ ] ggsave(penguins.png)
- [ ] ggsave(“png.penguins”)
