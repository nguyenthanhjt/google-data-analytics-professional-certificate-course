# Video: Cleaning up with the basics

Video transcript

- Hi again.
- Now that we've got a little more experience with the data frames, we can start doing some interesting things like clean, standardize, manipulate, and visualize data.
- We'll go through some common tasks that you'll perform as a data analyst.
- But we're just scratching the surface of what you might want to do in R.
- We'll start with the basics and learn how to clean up our columns.
- There will be a reading with a handy list you can refer to afterwards too.
- Let's install the Here, Skimr and Janitor packages now.
- We'll go ahead and open our console.
- First, we'll add the Here package.
- This package makes referencing files easier.
- To install it, we'll just write install.packages.
- Then in the parentheses, we'll put Here and RStudio will install it.
- After we install it, we'll also need to load it using library.
- Next, we'll install Skimr and Janitor.
- As a quick reminder, these packages simplify data cleaning tasks.
- They're both really useful and do slightly different things.
- The Skimr package makes summarizing data really easy and let's you skim through it more quickly.
- We'll install it now.
- The Janitor package has functions for cleaning data.
- After it's done installing, we'll still need to load it.
- Finally, we want to make sure the dplyr package is loaded since we are going to be using some of its features.
- There, now we've got all the packages we need for basic data cleaning.
- Now, let's load some data in.
- Later, when you're practicing with your own data, you can use read to grab a file.
- For example, if you had a CSV you wanted to load, you could write, read underscore CSV, and input the file name in the parentheses.
- This is where the Here package comes in handy.
- Be sure to install and load the Here package before trying to save CSV files.
- For now, we'll load a really fun package to practice with, the palmer penguin package.
- This is a dataset we've used before, but just as a quick reminder, the palmer penguin data has lots of information about three penguin species in the Palmer Archipelago, including size measurements, clutch sizes, and blood isotope ratios.
- Who doesn't love penguins? First, we'll install the package.
- We'll type install.packages and input palmerpenguins.
- Then remember to load it by using the library function.
- Now that we've got this data loaded into our library, we can try some cleaning functions on our columns.
- There's a few different functions that we can use to get summaries of our data frame.
- Skim without charts, glimpse, head, and select.
- The skim without charts function gives us a pretty comprehensive summary of a dataset.
- Let's try it out.
- When we run this, we get a lot of info back.
- First, it gives us a summary with the name of the dataset and the number of rows and columns.
- It also gives us the column types and a summary of the different data types contained in the data frame.
- Or we could use Glimpse to get a really quick idea of what's in this dataset.
- When we run this command, it'll show us a summary of the data.
- There's 344 rows and eight columns.
- We have species, island, measurements for bills, which are basically beaks and flippers, the penguins' body mass in grams, the sex, and finally, the year the data was recorded.
- We can also use Head to get a preview of the column names and the first few rows of this data set.
- Having the column names summarized like this will make it easier to clean them up.
- We can use select to specify certain columns or to exclude columns we don't need right now.
- Let's say we only need to check the species column.
- We can input penguins, then a pipe to indicate we'll add another command, and our select.
- We'll jump back into an R script because it will be easier to see.
- Now we have just the species column, or maybe we want everything except the species column.
- We'll put minus species instead of species, and now we have every column but species.
- The select statement is useful for pulling just a subset of variables from a large dataset.
- This lets you focus on specific groups of variables.
- There's a lot of other select functions that build on this that we'll cover later on.
- Now that we know our column names, we've got a better idea of what we might want to change.
- The rename function makes it easy to change column names.
- Starting with the penguin data, we'll type rename and change the name of our island column to island underscore new.
- Now, looking at our column names, we can see the column name has changed.
- Or let's say we want to change our columns so that they're spelled and formatted correctly.
- In spreadsheet programs, as long as our column names are meaningful, they're fine.
- But since we have to type the column names over and over in R, we need them to be consistent.
- Similar to the rename function, the rename_with() function can change column names to be more consistent.
- For example, maybe we want all of our column names to be in uppercase.
- We can use the rename_with() function to do that.
- This will automatically make our column names uppercase.
- But since variable names are usually lowercase, we'll use the "To lower" option to change it back.
- The clean names function in the Janitor package will automatically make sure that the column names are unique and consistent.
- Let's try the clean names function on our penguins data.
- This ensures that there's only characters, numbers, and underscores in the names.
- Now you know some functions for cleaning columns in your datasets.
- Try practicing them on your own with the palmer penguins data.
- Once you're comfortable with these functions, we'll learn even more about data cleaning in R.
- See you soon.
Hi again.
- Now that we've got a little more experience with the data frames, we can start doing some interesting things like clean, standardize, manipulate, and visualize data.
- We'll go through some common tasks that you'll perform as a data analyst.
- But we're just scratching the surface of what you might want to do in R.
- We'll start with the: Added to Selection.

## Questions & Notes

### Question 1: Which of the following functions returns a summary of the data frame, including the number of columns and rows? Select all that apply

- [x] glimpse()
- [ ] clean_names()
- [x] skim_without_charts()
- [ ] rename()

> Correct: The skim_without_charts() and glimpse() functions both return a summary of the data frame, including the number of columns and rows.

### Question 2: The rename_with() function can be used to reformat column names to be upper or lower case.

- [x] True
- [ ] False

> orrect: The rename_with() function can be used to reformat column names to be upper or lower case.

## Keypoints

1. **Introduction to Packages:** The video begins by highlighting the importance of packages like Skimr, Janitor, and dplyr for data cleaning tasks.

2. **Package Installation and Loading:** The instructor demonstrates how to install and load necessary packages using commands like `install.packages()` and `library()`.

3. **Loading Data:** The palmerpenguins package is introduced as a dataset for practice, and the process of loading it into R is shown.

4. **Data Summary:** Functions like `skim_without_charts()`, `glimpse()`, and `head()` are used to gain insights into the dataset's structure and content.

5. **Column Selection:** The `select()` function is utilized to choose specific columns for analysis, allowing for focused examination of relevant data.

6. **Column Renaming:** Methods for renaming columns using `rename()` and `rename_with()` are demonstrated to ensure consistency and clarity in column names.

7. **Column Cleaning:** The `clean_names()` function from the Janitor package is introduced to ensure uniformity and uniqueness in column names, simplifying further data processing.

Overall, this section provides a foundational understanding of basic data cleaning techniques in R, setting the stage for more advanced data manipulation tasks in subsequent modules.
