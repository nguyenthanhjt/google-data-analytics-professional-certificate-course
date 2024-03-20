# Video: R data frames

Video transcript

- Hey, welcome back.
- Before we can start cleaning and organizing our data or even check it for bias, we need to get our data into a usable format.
- This is where data frames come in.
- You might remember we talked a little bit about data frames before.
- In this video, we'll learn more about what data frames are and how you can use them.
- Let's get started.
- First, let's talk about what a data frame is.
- A data frame is a collection of columns.
- It's a lot like a spreadsheet or a SQL table.
- Here's an example of a data frame in R.
- It's a lot like other tables we've worked with throughout this program.
- There's column names and rows and cells with data.
- The columns contain one variable, and the rows have a set of values that match each column.
- We use data frames for a lot of the same reasons as tables too.
- They help summarize data and put it into a format that's easy to read and use.
- There's some things to know about data frames before working with them.
- We'll learn more about data frames throughout this program, but this is a great starting point.
- First, columns should be named.
- Using empty column names can create problems with your results later on.
- Let's think back to our example.
- Each of the columns are named based on the variable they represent.
- There's carat, cut, color, clarity, depth.
- All of these columns represent data about the diamonds.
- Next, it's important to know that the data stored in your data frame can be many different types, like numeric, factor, or character.
- Often data frames contain dates, time stamps and logical vectors.
- Finally, each column should contain the same number of data items, even if some of those data items are missing.
- Data frames are foundational.
- Now let's talk about tibbles.
- In the tidyverse, tibbles are like streamlined data frames.
- They make working with data easier, but they're a little different from standard data frames.
- First, tibbles never change the data types of the inputs.
- They won't change your strings to factors or anything else.
- You can make more changes to base data frames, but tibbles are easier to use.
- This saves time because you won't have to do as much cleaning or changing data types in tibbles.
- Tibbles also never change the names of your variables, and they never create row names.
- Finally, tibbles make printing in R easier.
- They won't accidentally overload your console because they're automatically set to pull up only the first 10 rows and as many columns as fit on screen.
- Super useful when you're working with large sets of data.
- Data frames and tibbles are the building blocks for analysis in R so having set standards for how they're built and dealt with is pretty important.
- If we all have the same understanding of what a data frame is, we can communicate more effectively.
- It's like we're all speaking the same language.
- It's also just a lot more practical.
- We need to be able to do things like define columns and review code easily in R.
- These characteristics make it easier to share your data and reproduce your analysis.
- Consistent data structures like data frames make it easier to operate on an entire dataset.
- Tidy data refers to the principles that make data structures meaningful and easy to understand.
- It's a way of standardizing the organization of data within R.
- These standards are pretty straightforward.
- Variables are organized into columns.
- Observations are organized into rows and each value must have its own cell.
- Now that you know a little more about data frames, let's start using them.
- Coming up, I'll teach you how to create data frames, add data to them and expand them.
- Bye for now.
Hey, welcome back.
- Before we can start cleaning and organizing our data or even check it for bias, we need to get our data into a usable format.
- This is where data frames come in.
- You might remember we talked a little bit about data frames before.
- In this video, we'll learn more about what data frames are and how you can use them.
- Let's get started.
- First, let's talk about what a data frame is.
- A data frame is a : Added to Selection.

## Questions & Notes

- Data frame: A collection of columns
  - Columns should be named
  - data stored can be many different types, like numberic, factor, or character
  - each column should contain the same number of data intems
- Tibbles: (in the tidyverse) tibbles are like streamlined data frames, they make working with data easier
  - Differences from standard data frames:
    - Never change the data types of the inputs
    - Never change the names of variables
    - Never create row names
    - Make printing easier

- Tidy data (R): a way of standardizing the organization of data within R
- Tidy data standards
  - variables are organized into columns
  - observations area organized into rows
  - each value must have its own cell

### Question 1: Fill in the blank: A data frame is a collection of _____

- [x] columns
- [ ] cells
- [ ] tibbles
- [ ] data

> Correct: A data frame is a collection of columns. It is similar to a table in spreadsheets or SQL.

### Question 2: Which of the following are standards of tidy data? Select all that apply.

- [ ] Columns are named
- [x] Variables are organized into columns
- [x] Observations are organized into rows
- [x] Each value has its own cell

> Correct: Variables are organized into columns, observations are organized into rows, and each value must have its own cell.

## **Key Points:**

- Data frames in R are akin to spreadsheets or SQL tables, consisting of columns and rows.
- They are used to summarize and organize data for easy readability and analysis.
- Columns in data frames should be named appropriately to avoid potential issues.
- Data within data frames can be of various types, including numeric, factor, character, dates, time stamps, and logical vectors.
- Tibbles, found in the tidyverse, are enhanced versions of data frames that maintain input data types, variable names, and do not create row names.
- Tibbles also have better printing capabilities, displaying only the first 10 rows and fitting as many columns as possible on screen to avoid overloading the console.
- Consistent use of data frames and tibbles facilitates effective communication, sharing of data, and reproducibility of analyses.
- Tidy data principles involve:
  - organizing variables into columns
  - observations into rows, and
  - ensuring each value has its own cell, thus standardizing data organization within R.
