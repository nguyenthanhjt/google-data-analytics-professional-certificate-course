# Video: Transforming data

Video transcript

- Welcome back.
- So far, we've started cleaning and now working with data in R.
- Now, let's talk about how to transform data.
- Sometimes you need to be able to break up a variable across multiple columns or combine existing columns, or even add new values to your data frame.
- Coming up, we'll use the separate, unite and mutate functions to transform our data in R.
- Luckily, the packages already downloaded into our library have some tools we can use to do just that.
- Let's open RStudio Cloud and check them out.
- To start, we'll create a data frame from scratch.
- For this example, we'll create a standard data frame, so that we can test out other functions.
- But you could also make a tribble here since we're manually inputting the data.
- You'll learn more about tribbles in a reading.
- For our dataset, we are going to copy and paste some data to create our own data frame.
- If you want to use the same data to follow along, check out the earlier reading.
- Our data contains employee information, including names and job titles.
- You can just copy it in.
- We can then name the data frame employee, indicate the column names as id, name and job title, and print the whole data frame.
- Right now, the first and last names are combined into one column.
- We can use the separate function to split these into separate columns.
- We'll start with separate, and then the data frame we want to work with and the column we'd like to separate.
- Then we'll add what we'd like to split the name column into.
- We'll just name these new columns, first name and last name.
- And finally, we'll tell R to separate the name column at the first blank space.
- When we run this, it will build us new columns for the first and last names.
- The separate function has a partner, unite.
- The unite function allows us to merge columns together.
- Basically, it does the opposite of separate.
- Let's say we're working with the version of this data frame with two name columns, and we want to combine them.
- We'll copy in this data as well.
- Our unite statement's a lot like our separate.
- We'll start with unite and indicate the data frame we're referring to.
- Then, we'll name the column we're combining first name and last name in.
- And then we'll say which columns we're combining.
- No quotation marks needed here.
- And finally, we can include a space that separates them.
- And when we run that, those two columns are combined.
- In addition to separating and merging columns, we can also create new variables in our data frame using the mutate function.
- We worked with mutate a little bit before to clean and organize our data.
- But mutate can also be used to add columns with calculations.
- Let's go back to our penguin dataset.
- Right now, the body mass column is measured in grams.
- Maybe we want to add a column with kilograms.
- To do that, we'll use mutate to perform the conversion and add a new column.
- And it will return a tibble with our new column.
- You can make calculations on multiple new variables by adding a comma.
- Let's add a column converting the flipper length too.
- Now, we've learned how to transform existing data in our tables and how to create new variables.
- Separate, unite and mutate are some basic functions that we'll keep building on, and you might discover new ways to use them while you're practicing too.
- Coming up, we'll talk more about summarizing data frames and how to address bias.
- I'll see you soon

## Question & Notes

- `separate(dataset, column-name, into=c('new-col-1','new-col-2',..), sep = 'separator-character')`: split data in a column into some others columns
- `unit()`: allow to merge/combine columns together
- `mutate()`:

**Note**: if you are following along within your Posit (R Studio) project, the following code was pasted into the script editor:

Copy + paste the syntax of the following concatenated list function that defines the three variables: first_name, last_name, and job_title:

```r
first_name <- c("John", "Rob", "Rachel", "Christy", "Johnson", "Candace", "Carlson", "Pansy", "Darius", "Claudia")

last_name <- c("Mendes", "Stewart", "Abrahamson", "Hickman", "Harper", "Miller", "Landy", "Jordan", "Berry", "Garcia")

job_title <- c("Professional", "Programmer", "Management", "Clerical", "Developer", "Programmer", "Management", "Clerical", "Developer", "Programmer")

employee <- data.frame(id, first_name, last_name, job_title)

print(employee)
```

The employee variable is defined as a data frame with the following parameters: id, first_name, last_name, and job_title.

Once this code is pasted into your editor, run the code, and continue with the video.

```r
# full code




id <- c(1:10)

id

name <-
  c(
    "John Mendes",
    "Rob Stewart",
    "Rachel Abrahamson",
    "Christy Hickman",
    "Johnson Harper",
    "Candace Miller",
    "Carlson Landy",
    "Pansy Jordan",
    "Darius Berry",
    "Claudia Garcia"
  )

job_title <-
  c(
    "Professional",
    "Programmer",
    "Management",
    "Clerical",
    "Developer",
    "Programmer",
    "Management",
    "Clerical",
    "Developer",
    "Programmer"
  )

employee <- data.frame(id, name, job_title)

View(employee)

print(employee)

# separated a column into 2 ones
separated <-
  separate(employee,
           name,
           into = c('first_name', 'last_name'),
           sep = ' ')
print(separated)

##

first_name <-
  c(
    "John",
    "Rob",
    "Rachel",
    "Christy",
    "Johnson",
    "Candace",
    "Carlson",
    "Pansy",
    "Darius",
    "Claudia"
  )

last_name <-
  c(
    "Mendes",
    "Stewart",
    "Abrahamson",
    "Hickman",
    "Harper",
    "Miller",
    "Landy",
    "Jordan",
    "Berry",
    "Garcia"
  )

job_title <-
  c(
    "Professional",
    "Programmer",
    "Management",
    "Clerical",
    "Developer",
    "Programmer",
    "Management",
    "Clerical",
    "Developer",
    "Programmer"
  )

employee <- data.frame(id, first_name, last_name, job_title)

print(employee)

## combibe/ merge columns
unite(employee, 'name', first_name, last_name, sep = ' ')

## mutate() to add new column
library("palmerpenguins")
View(penguins)

penguins %>%
  mutate(body_mass_kg = body_mass_g / 1000,
         flipper_length_m = flipper_length_mm / 1000) %>% 
  select(species, body_mass_kg, flipper_length_m)
```
