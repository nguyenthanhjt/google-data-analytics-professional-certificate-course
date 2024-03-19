# Quiz: Course 7 - Module 2 challenge

## Question 1: Which of the following are examples of variable names that can be used in R?

- [ ] value(2)
- [ ] value%2
- [ ] value-2
- [x] **value_2**

## Question 2: You want to create a vector with the values 12, 23, 51, in that exact order. After specifying the variable, what R code chunk lets you create the vector? 

- [x] **c(12, 23, 51)**
- [ ] c(51, 23, 12)
- [ ] v(12, 23, 51)
- [ ] v(51, 23, 12)

## Question 3: A data analyst finds the code mdy(10211020) in an R script. What is the year of the date that is created?

- [ ] 1021
- [ ] 2120
- [x] **1020**
- [ ] 1102

## Question 4: A data analyst wants to store a vector in a variable. What type of operator would they use to do this?

- [ ] Relational
- [ ] Arithmetic
- [ ] Logical
- [x] **Assignment**

## Question 5: A data analyst is deciding on naming conventions for an analysis that they are beginning in R. Which of the following rules are widely accepted stylistic conventions that the analyst should use when naming variables? Select all that apply

- [x] Use all lowercase letters in variable names.
- [ ] Use single letters like “x” to name all variables.
- [ ] Begin all variable names with an underscore.
- [x] **Use an underscore to separate words within a variable name.**

## Question 6: What type of packages are automatically installed and loaded to use in R studio when you start your first programming session?

- [ ] CRAN packages
- [ ] Recommended packages
- [x] **Base packages**
- [ ] Community packages

## Question 7: A data analyst needs a system of packages that use a common design philosophy for data manipulation, exploration, and visualization. What set of packages fulfills their need?

- [ ] Recommended
- [x] **tidyverse**
- [ ] Base
- [ ] CRAN

## Question 8: A data analyst wants to take a data frame named people and filter the data where age is 10, arranged by height, and grouped by gender. Which code snippet would perform those operations in the specified order?

- [ ] group_by( arrange( filter( people, age == 10 ), height ), gender )

- [ ] people %>% ## not correct

   filter(age == 10) +

   arrange(height) +

   group_by(gender)

- [x] filter( arrange( group_by( people, gender ), height ) , age == 10 )

- [ ] people %>%

   group_by(gender) %>%

   arrange(height) %>%

   filter(age == 10)

## Question 9: A data analyst wants to create the date February 27th, 2027 using the lubridate functions. Which of the following are examples of code that would create this value? Select all that apply

- [x] ymd("2027-02-27")
- [x] mdy(02272027)
- [ ] mdy("2027-02-27")
- [ ] dmy(02272027)
