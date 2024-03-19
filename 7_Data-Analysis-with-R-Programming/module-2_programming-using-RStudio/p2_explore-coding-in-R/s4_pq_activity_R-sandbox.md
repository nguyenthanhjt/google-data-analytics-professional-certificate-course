# Practice Quiz: Hands-On Activity: R sandbox

## **Activity overview**

So far, you’ve learned about the R programming language and why data analysts use it. In this activity, you will preview some of the cool things you can do in R. You will also learn more about working with packages and data and try out some important functions.

By the end of this activity, you will know how to install and load R packages, practice using functions to view, clean, and visualize data, and learn more about using R markdown to document your analysis. This will enable you to use R markdown, which helps to facilitate collaboration and document analysis which is needed for more complex projects.

## **Work in RStudio Cloud**

To start, log into your RStudio (Posit) Cloud account. Open the project you will work on in the activity with [this link](https://posit.cloud/content/6208304). At the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy. Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons. Once that is completed, navigate to the file explorer in the bottom right and click the following: Course 7 -> Week 2 -> Lesson3_Sandbox.Rmd.

If you’re having trouble finding the correct activity, check out this [step-by-step guide](https://scribehow.com/shared/Access_and_Install_Course_Material_for_Lesson_3__JGhlL8PLSxuqtK2KRWZkJw) on how to navigate in RStudio (Posit) Cloud. Make sure to select the correct R markdown (Rmd) file. The other Rmd files will be used in different activities.

If you are using RStudio Desktop, you can download the Rmd file directly [here](https://d3c33hcgiwev3.cloudfront.net/k7wCfkohTdG8An5KIU3R_g_c39319760e5344c1916586dbc1594af1_Lesson3_Sandbox.Rmd?Expires=1710979200&Signature=VbIqQOUsHiDP-9VtAGv~tRgCsZgONFGBh2IFlxhgf6BVr2bhZoBfwpiy~O5mHrp9LDaQNw0PfICld50trVub~JDDGROLgp0aFJHA7sbii5qUzTOSXun6kmZC-XCc5EDCzWFsxUh4hv-0keJ2WC~sshTFiZ6GTO1Bf56pic0ZUYs_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A).

```md
---
title: "Lesson 3: R Sandbox Activity"
output: html_document
---

## Background for this activity
Welcome to the sandbox! This activity is going to provide you with the opportunity to preview some of the cool things you can do in `R` that you will be learning in this course. You will learn more about working with packages and data and try out some important functions.  

In this activity, you are going to install and load `R` packages; practice using functions to view, clean, and visualize data; and learn more about using `R markdown` to document your analysis. `R` is a powerful tool that can do a lot of different things; this sandbox activity will help you get more comfortable using `R` while demonstrating some of its functions in action. In later activities, you will also get the opportunity to write your own R code!   

## Step 1: Using `R packages`
`Packages` are a key part of working with `R.`They contain bundles of code called `functions` that allow you to perform a wide range of tasks in `R.` Some of them even contain datasets that you can use to practice the skills you have been learning throughout this course.

Some `packages` are installed by default, but many others can be downloaded from an external source such as the Comprehensive R Archive Network, or CRAN.

In this activity, you will be using a package called `tidyverse.` The `tidyverse` package is actually a collection individual `packages` that can help you perform a wide variety of analysis tasks.

To install the `tidyverse` package, execute the code in the code chunk below by clicking on the green arrow button in the top right corner. When you execute a code chunk in RMarkdown, the output will appear in the .rmd area and your console.

```{r}
install.packages("tidyverse")
```

Once a package is installed, you can load it by running the `library()` function with the package name inside the parentheses, like this:

```{r}
library(tidyverse)
```

Installing and loading the `tidyverse` package may take a few minutes-- be sure to wait for it to finish running before moving on to the next steps!

Once the chunk above has finished running, you will get a report that summarizes what packages were loaded because you ran the `library()` function. The report will also let you know you if there are any `functions` that have a conflict, but you don't need to worry about that for now.  

Now that you have loaded an `R package,` you can start exploring some data. 

# Step 2: Viewing data

Many of the `tidyverse` packages contain sample datasets that you can use to practice your `R` skills. The `diamonds` dataset in the `ggplot2` package is a great example for previewing `R` functions. 

Because you already loaded this package in the last step, the `diamonds` dataset is ready for you to use.

One common function you can use to preview the data is the `head()` function, which displays the columns and the first several rows of data. You can test out how the `head()` function works by running the chunk below:

```{r}
head(diamonds)
```

In addition to `head()` there are a number of other useful functions you can use to summarize or preview the data. For example, the `str()` and `glimpse()` functions will both return summaries of each column in your data arranged horizontally. You can try out these two functions by running the code chunks below:

```{r}
str(diamonds)
```

```{r}
glimpse(diamonds)
```

Another simple function that you may use regularly is the `colnames()` function. It returns a list of column names from your dataset. You can check out this function by running the code chunk below:

```{r}
colnames(diamonds)
```

After running the code chunk, you may have noticed a number in brackets. This number helps you count the number of columns in your dataset. If you have data with lots of columns and `colnames()` prints the results on multiple lines, each line will have a number in brackets at the start of the line indicating what number column that is! So, for example, "carat" is the first column in the `diamonds` dataset. On the second line, there is the number seven in brackets; "price" is the seventh column. 

## Step 3: Cleaning data

One of the most frequent tasks you will have to perform as an analyst is to clean and organize your data. `R` makes this easy! There are many functions you can use to help you perform important tasks easily and quickly. 

For example, you might need to rename the columns, or variables, in your data. There is a function for that: `rename().` You can check out how it works in the chunk below:

```{r}
rename(diamonds, carat_new = carat)
```

Here, the function is being used to change the name of `carat` to `carat_new`. This is a pretty basic change, but `rename()` has many options that can help you do more complex changes across all of the variables in your data.

For example, you can rename more than one variable in the same `rename()` code. The code below demonstrates how:

```{r}
rename(diamonds, carat_new = carat, cut_new = cut)
```

Another handy function for summarizing your data is `summarize().` You can use it to generate a wide range of summary statistics for your data. For example, if you wanted to know what the mean for `carat` was in this dataset, you could run the code in the chunk below:

```{r}
summarize(diamonds, mean_carat = mean(carat))
```

These functions are a great way to get more familiar with your data and start making observations about it. But sometimes, previewing tables isn't enough to understand a dataset. Luckily, `R` has visualization tools built in. 

## Step 4: Visualizing data
With `R,` you can create data visualizations that are simple and easy to understand or complicated and beautiful just by changing a bit of code. `R` empowers you to present the same data in so many different ways, which can help you create new insights or highlight important data findings.  One of the most commonly used visualization packages is the `ggplot2` package, which is loaded automatically when you install and load `tidyverse.` The `diamonds` dataset that you have been using so far is a `ggplot2` dataset.

To build a visualization with `ggplot2` you layer plot elements together with a `+` symbol. You will learn a lot more about using `ggplot2` later in the course, but here is a preview of how easy and flexible it is to make visuals using code:

```{r}
ggplot(data = diamonds, aes(x = carat, y = price)) +
  geom_point()
```

The code above takes the `diamonds` data, plots the carat column on the X-axis, the price column on the Y-axis, and represents the data as a scatter plot using the `geom_point()` command. 

`ggplot2` makes it easy to modify or improve your visuals. For example, if you wanted to change the color of each point so that it represented another variable, such as the cut of the diamond, you can change the code like this:

```{r}
ggplot(data = diamonds, aes(x = carat, y = price, color = cut)) +
  geom_point()
```

Wow, that's a busy visual! Sometimes when you are trying to represent many different aspects of your data in a visual, it can help to separate out some of the components. For example, you could create a different plot for each type of cut. `ggplot2` makes it easy to do this with the `facet_wrap()` function:

```{r}
ggplot(data = diamonds, aes(x = carat, y = price, color = cut)) +
  geom_point() +
  facet_wrap(~cut)
```

You will learn many other ways of working with `ggplot2` to make functional and beautiful visuals later on. For now, hopefully you understand that it is both flexible and powerful!

## Step 5: Documentation

You have been working in an `R markdown` file, which allows you to put code and writing in the same place. Markdown is a simple language for adding formatting to text documents. For example, all of the section headers have been formatted by adding `##` to the beginning of the line. Markdown can be used to format the text in other ways, such as creating bulleted lists:

- So if you have a list of things
- Or want to write bullets for another reason
- You can do that using markdown

When you have written, executed, and documented your code in an `R markdown` document like this, you can use the `knit` button in the menu bar at the top of the editing pane to export your work to a beautiful, readable document for others. 

## Activity Wrap-up
You have had a chance to explore more `R` tools that you can start using on your own. You learned how to install and load `R packages`; functions for viewing, cleaning, and visualizing data; and using `R markdown`to export your work. Feel free to continue exploring these functions in the rmd file, or use this code in your own RStudio project space. As you practice on your own, consider how `R` is similar and different from the tools you have already learned in this program, and how you might start using it for your own data analysis projects. `R` provides a lot of flexibility and utility that can make it a key tool in a data analyst's tool kit. 

Make sure to mark this activity as complete in Coursera.



```

Carefully read the instructions in the comments of the Rmd file and complete each step. Some steps may be as simple as running pre-written code, while others may require you to write your own functions. After you finish the steps in the Rmd file, return here to confirm that your work is complete.

## **Reflection**

Which function can you use to create a different plot for each type of cut of diamond?

1. str()
2. facet_wrap()
3. summarize()
4. geom_point()
