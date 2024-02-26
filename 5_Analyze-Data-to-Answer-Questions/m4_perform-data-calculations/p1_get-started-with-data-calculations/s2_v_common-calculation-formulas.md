# Video - Common calculation formulas

Video transcript

- Hey there.
- You probably do a lot of calculations in your daily life.
- Maybe it's figuring out how much to tip someone or balancing your budget.
- You might do some of these calculations in your head or with paper and pencil or the calculator on your phone.
- You might even have shortcuts to use to make the calculations easier.
- You'll perform a lot of calculations as a data analyst too.
- But they'll involve more numbers in a wider range of calculations.
- That's where you'll put your data analyst tools to work.
- We'll show you how you could use formulas in a spreadsheet to complete some of the most basic calculations.
- Formulas are one of the many shortcuts that data analysts use.
- But rest assured, even though they're shortcuts, they'll still calculate with complete accuracy.
- We've covered a lot of these calculations earlier in the program.
- But if you skip that part and want a refresher, we'll review them here.
- These calculations will also be more advanced than the ones we've covered so far.
- But they'll also be closer to what you might use on the job.
- We'll be using Google Sheets in this video, but you can also use Excel.
- The steps might look a little different in Excel, but the outcomes will be the same.
- Let's try out some calculations with sales data from a discount store chain.
- We'll look at data for one of the stores in the chain.
- Our objective: use the existing sales data to find any trends.
- This is a great way to see a lot of the ways formulas can be useful in your analysis.
- We'll start by finding annual sales over the years 2011-2020.
- The data is already organized in columns by month and in rows by year.
- But we don't have the total sales for each year yet.
- We can use a sum function to help us figure that out.
- We'll add the sales from 2011 first.
- We'll add a heading for the annual sales column, then we can type our sum function and a formula.
- All formulas begin with an equal sign.
- We'll type that first, followed by sum and then an open parenthesis.
- After the open parenthesis, we need to tell the formula which cells are being added.
- In this case, we need data from the whole row which begins in cell B2.
- B2 is a cell reference we'll use.
- Instead of typing each cell one by one, we can put them in the formula quickly by selecting cell B2 and dragging the fill handle across the row to the last cell with sales data, M2.
- Now we'll complete the formula by closing the parentheses and pressing Enter.
- Just like that, we've calculated the total sales for 2011.
- Here's another shortcut we worked with in an earlier video.
- The fill handle is the tiny box in the corner of each sale.
- You can use it for lots of things like selecting multiple cells for a formula or continuing a pattern across several cells, the fill handle definitely qualifies as a shortcut.
- We can use the formula we created to calculate the total sales for the other years in the dataset.
- All we have to do is drag the fill handle down the other cells in the annual sales column and we'll have total sales data for the rest of the years in the dataset.
- Let's say, we also need to find the growth in annual sales from year to year.
- This would be a good time to think through the problem before we try to solve it.
- Do we have the data we need to solve this? Not yet.
- Thinking backwards like this helps us plan out the steps to move forward.
- The first step we'll need to do is calculate the total sales per year.
- Then we'll measure the rate of change between years.
- We'll start by labeling a new column.
- In this case, we won't need to use a function or parentheses, since we're only using data from two cells.
- We can just use the name of those cells, we'll type an equals sign and then click in "Cell N3", which automatically populates that sale in the formula.
- Next, we'll add a minus sign to the formula because we're subtracting to find the difference between two consecutive years.
- Clicking in "Cell N2" gives us the total from 2011, which we can then subtract from the total from 2012.
- Then we hit Enter and get our sales growth from 2011-2012.
- We're definitely getting some useful data here.
- Let's keep going.
- We can also use our sales growth to find the growth rate between the two years.
- We'll show this as a percentage.
- We'll head our column with the percent sign and growth.
- To do this, we'll divide the total in cell O3 by the annual sales from 2011 in cell N2.
- A slash is a symbol that a formula recognizes as division, so we'll place that between the two cell references and presto, there's the growth rate.
- Growth rates are usually shown as percentages, which can be easier than a decimal to read and understand.
- Let's change this number to a percentage.
- Time for another shortcut.
- All we have to do is click the percent style button and our growth rate will become a percentage.
- We can select the cells for both the total growth and the growth rate to populate the rest of the two columns.
- We have some negative numbers, but that just means that there was negative growth from one year to the next.
- We've got just a few more things to calculate for our stakeholders.
- Next step is finding the average sales.
- We want to compare sales between months to learn if there's a trend.
- We'll add this in a row instead of a column.
- This will line up our averages under each month.
- To find our averages, will calculate the total and then divide that total by the number of values added to get it.
- We can do this by using the average function.
- Between our parentheses will select the cells that contain the sales data for January, B2 through B11.
- We'll duplicate that formula across the row through December to look for trends.
- Right away, we know that summer months and December have the highest average sales.
- Since our stakeholders will want to understand our findings quickly and easily, we'll add a little visualization to the data with conditional formatting.
- You'll learn more about data visualizations like conditional formatting soon.
- But here's a sneak peek.
- Conditional Formatting is a spreadsheet tool that changes how cells appear when values meet specific conditions.
- Let's apply conditional formatting to the cells with the average sales by month.
- We'll use a color scale to show the range of averages.
- Well, the lowest monthly average remaining as white and we'll apply shades of green to the rest of the values.
- The brighter the green, the higher the average.
- Now, when we share our analysis with our stakeholders, they will be able to tell right away which months have the highest average sales.
- Just a couple more steps to complete our analysis.
- Now we need to find the minimum and maximum for average monthly sales.
- With the dataset this small, it might be easy to find the minimum and maximum values without a formula, but it's still good practice to use one.
- Not to mention, using a formula helps prevent human error, will again rely on formulas with Functions to do these calculations, we'll start with the lowest monthly average.
- Our function here is MIN, followed by the cells with the average month B12 through M12.
- After we press Enter, the lowest monthly average is calculated.
- We can repeat the same steps to find the highest monthly average,
- in this formula will use the same data, but we'll replace MIN with MAX for maximum.
- For this store location, sales are strongest in December and weakest in January.
- We could share these findings with stakeholders if they've met our objectives.
- If they haven't, we might need to continue with our analysis.
- Either way, I hope you've learned how spreadsheet formulas can be valuable tools when doing calculations.
- Coming up, we'll check out more formulas.
- See you soon.

## Questions and notes

Would you like to follow along with the instructor using the same spreadsheet?

To use the template for this spreadsheet, click the link below and select “Use Template.”

Link to template: [Discount Variety Store-433, Monthly Sales](https://docs.google.com/spreadsheets/d/1lwz8hk7fBRMMgOG-Kk34JnBWSh2yEQ5aN8iJ--pb54Q/template/preview)

OR If you don't have a Google account, you can download the spreadsheet from the attachment [discount-variety-store-433-monthly-sales.xlsx](./resources/discount-variety-store-433-monthly-sales.xlsx)

### Question 1: You are calculating the sum of a range of cells from A2 through F2. What is the correct syntax for this calculation?

- `=SUM(A2:F2)`
- =SUM(A2+F2)
- =SUM(A2,F2)
- =SUM(A2*F2)

> To calculate the sum of a range of cells from A2 through F2, the correct syntax is =SUM(A2:F2). Formulas begin with an equals sign. A2:F2 are the cell references to be summed. And the colon between the two cell references indicates that it is a range of cells.

### Question 2: You are analyzing the results of retail sales calculations. You click in cell H10 and find the following formula: =H9/G9. What operation is taking place in this cell?

- Addition
- Subtraction
- Multiplication
- Division

> In the formula =H9/G9, the operation is division. The operator for division is a slash (/).

## Key points from the video

1. **Introduction to Calculations:**
   - Daily life involves various calculations, and as a data analyst, calculations become more extensive and diverse.
   - Formulas in spreadsheets are presented as powerful tools for data analysts, providing shortcuts for accurate calculations.

2. **Spreadsheet Tools and Formulas:**
   - Overview of using formulas in a spreadsheet for basic and advanced calculations.
   - Emphasis on the accuracy of calculations even with the use of shortcuts.

3. **Software Compatibility:**
   - Usage of Google Sheets is demonstrated, with acknowledgment that similar outcomes can be achieved in Excel.

4. **Practical Example - Sales Data Analysis:**
   - Objective: Analyzing sales data for a discount store chain to identify trends over the years 2011-2020.
   - Demonstration of calculating annual sales using the SUM function and the fill handle for efficiency.

5. **Calculating Sales Growth and Growth Rate:**
   - Introduction of a new column for sales growth.
   - Calculation of growth rate between consecutive years, presented as a percentage.
   - Usage of shortcuts for converting numbers to percentages.

6. **Average Monthly Sales:**
   - Calculation of average monthly sales to compare trends between months.
   - Utilization of the AVERAGE function and the fill handle for efficiency.

7. **Conditional Formatting for Data Visualization:**
   - Introduction of conditional formatting as a tool for data visualization.
   - Application of conditional formatting to represent the range of average monthly sales using a color scale.

8. **Minimum and Maximum Monthly Averages:**
   - Use of the MIN and MAX functions to find the lowest and highest monthly averages, respectively.
   - Emphasis on using formulas to prevent human error and ensure accuracy.

9. **Conclusion:**
   - Reinforcement of the value of spreadsheet formulas in data analysis.
   - Teaser for upcoming videos covering more formulas.
