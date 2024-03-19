# Video: More on the tidyverse

Video transcript

- Great, you're back.
- Have you ever taken a tour of a famous landmark or an unfamiliar city? It can be pretty exciting.
- You get to learn all about the features of the landmark or city.
- Eventually, you get to know them pretty well, and you can share what you learned with others.
- Well we're here to take a different kind of tour: a tour of the tidyverse.
- For this tour, we won't be traveling anywhere special, but we will help you learn about the exciting tidyverse features.
- And once you know them a little better, you can most definitely share what you learned with others.
- For this tour we'll focus on the core packages of tidyverse we discussed earlier: ggplot2, tidyr, readr, dplyr, tibble, purrr, stringr and forcats.
- We also learned how to install and load them in RStudio.
- Once they're loaded, you won't need to do anything else with their actual packages.
- They'll do their thing as you program.
- So what is their thing? Well, it depends, but there's four packages that are an essential part of the workflow for data analysts: ggplot2, dplyr, tidyr and readr.
- You'll most likely use these more often than the others.
- Ggplot2 is used for data visualization, specifically plots.
- With ggplot2, you can create a variety of data viz by applying different visual properties to the data variables.
- Here's an example of ggplot2 in action.
- You'll have your own chance to use ggplot2 later.
- Tidyr is a package used for data cleaning to make tidy data.
- We covered tidy or clean data earlier, but as a quick reminder, it's data where every part of a data table or data frame is the right type in the right place.
- Tidyr works with wide and long data to make sure this happens.
- Next, we have readr, which is used for importing data.
- The most common function from readr is read_csv.
- This will import a CSV file into R.
- A CSV file contains data separated by commas in a table format.
- To accurately read a dataset with readr, you combine the function with a column specification.
- The column specification describes how each column should be converted to the most appropriate data type.
- It's good to keep in mind this isn't usually necessary because readr will figure it out for you automatically.
- We'll come across readr functions as we continue to explore R.
- Now on to dplyr.
- Dplyr offers a consistent set of functions that help you complete some common data manipulation tasks.
- For example, the select function picks variables based on their names, and the filter function finds cases where certain conditions are true.
- And, yes, dplyr is another package we'll get to later.
- There's plenty to look forward to, so that's the fab four of the tidyverse.
- They'll all make your programming in R more straightforward and efficient.
- The other four packages are definitely useful, too, but you might not use them as often.
- Tibble works with data frames.
- Purrr works with functions and vectors helping make your code easier to write and more expressive.
- Stringr includes functions that make it easier to work with strings.
Play video starting at :4:3 and follow transcript4:03
Forcats provides tools that solve common problems with factors.
- As a quick reminder, factors store categorical data in R where the data values are limited and usually based on a finite group like country or year.
- Using the tidyverse and its packages will help you fine-tune your analysis.
- And besides tidyverse, you also learned the fundamentals of R from variables to vectors and more.
Play video starting at :4:34 and follow transcript4:34
You explored the different operators in R and saw how they can help you complete calculations.
- You had the chance to check out pipes and how they can make your programming more efficient.
- And you unpacked packages to find out how they're a big part of what you can do in R.
Play video starting at :4:54 and follow transcript4:54
We've covered a lot of ground in just a few videos, so this might be a good time for you to do a little review.
- You can rewatch videos and revisit any other resources that can help you get an even better grasp of all the terms, concepts and processes that are part of R.
- Looking ahead, you'll start working with data in R including a more thorough exploration of how tidyverse impacts your process.
- You'll see tibble, readr and other tidyverse packages in action.
- And you'll find out how to clean and organize your data in R.
- All this and more coming up.
- I'll see you soon.
Great, you're back.
- Have you ever taken a tour of a famous landmark or an unfamiliar city? It can be pretty exciting.
- You get to learn all about the features of the landmark or city.
- Eventually, you get to know them pretty well, and you can share what you learned with others.
- Well we're here to take a different kind of tour: a to: Added to Selection.

## Question & Notes

- 4 packages that are an essential part of the workflow for data analyst:
  - **ggplot 2**: is used for visualization, specifically plots
    - Create a variety of data viz by applying different visual properties to the data variable in R
  - **dplyr**: offers a consistent set of functions that help you complete some common data manipulation tasks
  - **tidyr**: a package user for data cleaning to make tidy data
    - work with wide and long data
  - **readr**: user for importing data
    - `read_csv` function
- 4 other packages:
  - **tibble**: work with data frame
  - **purr**: work with functions and vector -> easier to write and expressive
  - **stringr**: easier to write and work with string
  - **forcats**: provide tools solve common problems with factors
- Factor (R): factors store categorical data in R where the data values are limited and usually based on a finite group like country or year

### Question 1: Which tidyverse package is used for data visualization?

- [ ] tidyr
- [ ] readr
- [x] ggplot2
- [ ] dplyr

> Correct: The ggplot2 package is used for data visualization, specifically plots. You can use ggplot2 to create a lot of different visualizations by applying different properties to the data variables.

### Question 2: The read_csv() function is a part of the dplyr package

- [ ] True
- [x] False

> Correct: The read_csv() function is a part of the readr package. It imports a .CSV file for use in R.

## **Key Points:**

- The video introduces the viewer to the tidyverse, a collection of R packages designed for data manipulation, exploration, and visualization.
- Core packages of tidyverse include ggplot2, dplyr, tidyr, readr, tibble, purrr, stringr, and forcats.
- These packages streamline various data analysis tasks, such as visualization, data cleaning, data importing, and data manipulation.
- Each package serves a specific purpose within the data analysis workflow, contributing to making R programming more straightforward and efficient.

**Definitions:**

- **Tidyverse:** A collection of R packages with a common design philosophy for data manipulation, exploration, and visualization.
- **Vignette:** Documentation that serves as a guide to an R package, providing details about the problem the package solves and how its functions can be utilized.
