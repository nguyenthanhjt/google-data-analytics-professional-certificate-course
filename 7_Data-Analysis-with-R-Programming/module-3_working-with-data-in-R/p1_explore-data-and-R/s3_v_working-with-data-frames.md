# Video: Working with data frames

Video transcript

- Hey there.
- Earlier, we learned about data frames and their key characteristics.
- Now we'll actually start working with them.
- As a data analyst a lot of your work will depend on data frames.
- If you don't create a data frame, your ability to work with your data will be limited.
- Think about spreadsheets.
- That basic structure of columns and rows carries over to R.
- Data frames are basically the data analyst's default way to interact with data.
- That's why knowing how to create and work with data frames is so important.
- So let's check out an example.
- Here we'll use R's built-in data frames.
- One of the great things about R and R packages is that there's a lot of interesting, easy-to- access datasets built in.
- These datasets that you practice some of the tools we've been learning.
- Let's open RStudio and get started.
- We'll use a preloaded dataset with information about diamonds.
- This data set is part of the ggplot2 package in the tidyverse.
- So make sure you first load ggplot2.
- We'll learn how to load our own datasets later too.
- But diamonds is a good dataset to practice with.
- We can load this data now by using data open and closed parentheses.
- You might notice that when we start to type diamonds, RStudio gives us the option to select it from its drop-down menu.
- That's because this dataset already exists in our library.
- Okay, now let's add this data frame to our data viewer.
- There's ten columns and 100 rows in this data frame but we might not want to see all of it.
- We can use the head function to give us just the first six rows.
- This is a nice preview of the entire dataset.
- Accidentally printing the full data frame to the console can be annoying and can take a long time to compute.
- You can avoid printing the full data frame by using functions like head to get a quick preview.
- We can also get the structure of the data frame using functions like str() and colnames().
- These are just two functions you can use to check out your data.
- We'll explore other functions like glimpse later on.
- For example, we could use the structure function to highlight the structure of this data frame.
- This gives us some high-level info like the column names and the type of data contained in those columns.
- But if we just want to know the column names we can use colnames instead.
- Here we have carat, cut, color, clarity, depth, all of the columns included in this data set.
- We can also use the mutate function to make changes to our data frame.
- The mutate function is part of the dplyr package which is in the tidyverse.
- So you'll need to load the tidyverse library before you test out mutate.
- Let's add a new column first.
- All we have to do is input mutate and then tell R we want to add a new column to the diamonds data frame.
- We'll first call mutate followed by the name of the data frame we want to change.
- Then we'll add a column and the name of the new column we want to create.
- Then we want to calculate this new column.
- In this case, to make it easier to read the carat column we'll multiply it by 100 to create a new column carat_2.
- And when we run this, presto, our data frame has a new column.
- You won't lose any columns when you create the new one.
- The rest of the data frame will still be the same.
- Data frames are usually the starting point for analyzing data in R.
- So it's important to understand the characteristics of data frames and how to create them.
- Great job, and I'll see you next time.

## Question & Notes

**Correction**: if you look closely at the bottom of the diamonds data set, you will see there are actually 53,940 entries (or observation rows) in total and not 100.

In order to get a much shorter and simpler overview of the data observations, we will use the head() function introduced next.

### Question 1: Which R function should you use if you want to preview just the first six rows of a data frame?

- [ ] mutate()
- [x] head()
- [ ] str()
- [ ] colnames()

> Correct: The head() function provides a preview of the first six rows of a data frame. This is useful if you want to quickly check out the data, but don’t want to print the entire data frame.

### Source codes

```r
library(ggplot2) ## load

data("diamonds") ## load dataset

View(diamonds) ## preview the dataset

head(diamonds) ## preview the first 6 rows

str(diamonds) ## get structure of data frame

colnames(diamonds) ## Get columns' names


## make changes to  data frame (part of dplyr package in the `tidyverse`)
library(tidyverse)
mutate(diamonds, carat_2=carat*100)
```

### **Key Points:**

- Data frames are essential for data analysis in R, providing a structured way to interact with data similar to spreadsheets.
- R offers built-in datasets for practice and analysis, such as the diamonds dataset in the ggplot2 package.
- Functions like `data()`, `head()`, `str()`, and `colnames()` allow for data exploration, providing insights into the structure and content of data frames.
- The `mutate()` function, part of the dplyr package in the tidyverse, enables the addition of new columns to data frames and the transformation of existing columns.
- Loading the tidyverse library is necessary to use functions like `mutate()`.
- Understanding data frame characteristics and how to manipulate them is crucial for effective data analysis in R.
