# Video - Pivot tables continued

Video transcript

- Welcome back.
- In the last video, we created a pivot table of movie data and revenue calculations to help our manager think through new movie ideas.
- We used our pivot table to make some initial observations about annual revenue.
- We also discovered that the average revenue for 2015 was lower than other years even though more movies were released that year.
- We hypothesized that this was because more movies that earn less than $10 million in revenue were released in 2015.
- To test this theory, we created a copy of our original pivot table.
- Now we are going to apply filters in calculated fields to explore the data more.
- Let's get started.
- You all remember that the filter option lets us view only the values we need.
- We'll select a cell in our copied pivot table and add a filter to the box office revenue column.
- The filter will then be applied to the entire table.
- When we open the status menu, we can choose to filter the data to show specific values.
- But in our case, we want to filter by condition so we can figure out how many movies in each year earn less than $10 million.
- The condition we'll use in our filter is less than and our value will be $10 million which is why we renamed these columns earlier.
- We'll type our number in a dollar and cents format so the condition matches the data in our pivot table.
- This might not be necessary, but it prevents potential errors from happening.
- Now we know that 20 movies released in 2015 made less than $10 million.
- This seems like a high number compared to the other years.
- But keep in mind, there were more movies from our data set released in 2015.
- Before we move on, let's use a calculated field to verify our average because it was copied from another pivot table before we filtered it.
- That way we can check that it's correct.
- We'll create a customized column called a calculated field using our values menu.
- A calculated field is a new field within a pivot table that carries out certain calculations based on the values of other fields.
- You can do this in Excel too using field settings and the create formula menu.
- For the formula in our calculated field, we'll use the sum function and divide the sum of the box office revenue data from our original table by the count of the same data.
- Because we applied our filter to this pivot table earlier, this formula will only return the average revenue of movies under $10 million.
- That worked.
- We were able to check the accuracy of some of our data before analyzing it.
- Always a good thing.
- But it's still difficult to tell how much of an impact these lower earning movies had on the average revenue.
- Let's run a quick formula to find the percentage of movies for each year that earned less than $10 million.
- This will make it easier to compare from year to year.
- Instead of a calculated field, we'll add this as a formula in a new column, that way we can pull data from both of our pivot tables.
- We'll put a header for our table in cell G10 and name it percent of total movies.
- Then we'll add our formula to the next cell in the column.
- Divide the number of movies in the copy table by the number of movies in the original table.
- Then we'll use the fill handle in the cell with a formula and drag it to apply the formula to the rest of the years.
- Finally, we'll format these numbers as percentages.
- Now our analysis shows that 16 percent of the movies released in 2015 earned less than $10 million of revenue.
- The other years are all close to 10 percent.
- This is one possible explanation for why the average revenue is comparatively low in 2015.
- In real life, we'd most likely need to take our analysis even further depending on our goals.
- But for now, we're all set.
- You've learned how you can use pivot tables to perform data calculations.
- It will take practice, but pivot tables are worth it because they do more than calculate.
- They organize and filter data too.
- Together we've covered functions, formulas, and pivot tables.
- All great tools to use in analysis.
- With practice and experience, it will feel like you've used them forever.
- Just take your time getting to know how they work.
- Keep exploring these videos and the readings.
- Great work.

## Questions and Notes

### Notes

- Calculated field: a new field with a pivot table that carries out certain calculations based on on the values of other fields
  - `=SUM('Box Office Revenue ($)')/count('Box Office Revenue ($)')`

### Questions 1: A calculated field within a pivot table is used to carry out calculations based on what?

- The syntax of the available formulas
- The filtered values
- `The values of other fields`
- The function in the calculated field

> A calculated field within a pivot table is used to carry out calculations based on the values of other fields. The calculated field is added as an additional row or column in a pivot table.
