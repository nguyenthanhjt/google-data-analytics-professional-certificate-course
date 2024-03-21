# Quiz: Course 7 Module 3 challenge

## 1. **Question 1**: A data analyst creates a data frame with data that has more than 50,000 observations in it. When they print their data frame, it slows down their console. To avoid this, they decide to switch to a tibble. Why would a tibble be more useful in this situation?

- [ ] Tibbles will automatically create row names to make the data easier to read
- [ ] Tibbles only include a limited number of data items
- [x] Tibbles won’t overload the console because they automatically only print the first 10 rows of data and as many variables as will fit on the screen
- [ ] Tibbles will automatically change the names of variables to make them shorter and easier to read

## 2. **Question 2**: A data analyst is examining a new dataset for the first time. They load the dataset into a data frame to learn more about it. What function(s) will allow them to review the names of all of the columns in the data frame? Select all that apply

- [x] str()
- [x] colnames()
- [x] head()
- [ ] library()

## 3. **Question 3**: You are working with the ToothGrowth dataset. You want to use the glimpse() function to get a quick summary of the dataset. Write the code chunk that will give you this summary

   ```R
   glimpse(ToothGrowth)
   ```

   How many variables does the ToothGrowth dataset contain?

- [x] 3
- [ ] 5
- [ ] 4
- [ ] 2

## 4. **Question 4**: You have a data frame named employees with a column named Last_NAME. What will the name of the employees column be in the results of the function rename_with(employees, tolower)?

- [ ] lAST_nAME
- [ ] last_nAME
- [x] last_name
- [ ] Last_NAME

## 5. **Question 5**: A data analyst is working with the penguins data. They write the following code

   ```R
   penguins %>%
   ```

   The variable species includes three penguin species: Adelie, Chinstrap, and Gentoo. What code chunk does the analyst add to create a data frame that only includes the Gentoo species?

- [x] filter(species == “Gentoo”)
- [ ] filter(species == “Adelie”)
- [ ] filter(species <- “Gentoo”)
- [ ] filter(Gentoo == species)

## 6. **Question 6**: You are working with the penguins dataset. You want to use the summarize() and min() functions to find the minimum value for the variable bill_depth_mm. At this point, the following code has already been written into the script

   ```R
   penguins %>% 
     drop_na() %>% 
     group_by(species) %>%
   ```

   Add the code chunk that lets you find the minimum value for the variable bill_depth_mm.

   1 point

   ```R
   summarize(min_bill_depth = min(bill_depth_mm))
   ```

   What is the minimum bill depth in mm for the Chinstrap species?

- [ ] 13.1
- [ ] 12.4
- [ ] 15.5
- [x] 16.4

## 7. **Question 7**: A data analyst is working with a data frame called zoo_records. They want to create a new column named is_large_animal that signifies if an animal has a weight of more than 199 kilograms. What code chunk lets the analyst create the is_large_animal column?

- [x] zoo_records %>% mutate(is_large_animal = weight > 199)
- [ ] zoo_records %>% mutate(weight > 199 = is_large_animal)
- [ ] zoo_records %>% mutate(weight > 199 <- is_large_animal)
- [ ] zoo_records %>% mutate(is_large_animal == weight > 199)

## 8. **Question 8**: A data analyst is working with a data frame named customers. It has separate columns for area code (area_code) and phone number (phone_num). The analyst wants to combine the two columns into a single column called phone_number, with the area code and phone number separated by a hyphen. What code chunk lets the analyst create the phone_number column?

- [ ] unite(customers, “phone_number”, area_code, phone_num)
- [ ] unite(customers, area_code, phone_num, sep=”-”)
- [ ] unite(customers, “phone_number”, area_code, sep=”-”)
- [x] unite(customers, “phone_number”, area_code, phone_num, sep=”-”)

## 9. **Question 9**: A data analyst is using statistical measures to get a better understanding of their data. What function can they use to determine how strongly related are two of the variables?

- [ ] bias()
- [ ] mean()
- [x] cor()
- [ ] sd()

## 10. **Question 10*:   A data analyst wants to check the average difference between the actual and predicted values of a model. What single function can they use to calculate this statistic?

- [ ] cor()
- [x] bias()
- [ ] sd()
- [ ] mean()
