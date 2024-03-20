# Practice Quiz: Test your knowledge on cleaning data

## **Question 1**: Data analysts are cleaning their data in R. They want to be sure that their column names are unique and consistent to avoid any errors in their analysis. What R function can they use to do this automatically?

- [ ] clean_names()
- [ ] select()
- [x] rename_with()
- [ ] rename()

> Correct: The clean_names() function will automatically make sure that column names are unique and consistent.

## **Question 2**: You are working with the penguins dataset. You want to use the `arrange()` function to sort the data for the column bill_length_mm in ascending order. You write the following code

   ```r
   penguins %>%
   ```

   Add a single code chunk to sort the column bill_length_mm in ascending order. Note: DO NOT write the above code `penguins %>%` into your answer as it has already been pre-written into the code chunk.

   What is the shortest bill length in mm?

- [ ] 33.1
- [x] 32.1
- [ ] 33.5
- [ ] 34.0

> Correct: You add the code chunk arrange(bill_length_mm) to sort the column bill_length_mm in ascending order. The correct code is penguins %>% arrange(bill_length_mm). Inside the parentheses of the arrange() function is the name of the variable you want to sort. The code returns a tibble that displays the data for bill_length_mm from shortest to longest. The shortest bill length is 32.1mm.

## **Question 3**: Data analysts are working with customer information from their company’s sales data. The first and last names are in separate columns, but they want to create one column with both names instead. Which of the following functions can they use?

- [ ] select()
- [x] separate()
- [ ] unite()
- [ ] arrange()

> Correct: The unite() function can be used to combine columns.
