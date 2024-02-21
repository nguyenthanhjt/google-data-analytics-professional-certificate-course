# Prepare for VLOOKUP

Video transcript

- Hi, again.
- In this video, we'll prep our data for VLOOKUP, a data aggregation tool.
- As you learned before, data aggregation is the process of gathering data from multiple sources in order to combine it into a single summarized collection.
- Data aggregation can give you all kinds of information about the data you are looking at.
- For example, in marketing, you can aggregate data from an ad campaign to see how it performed over time and for particular customers.
- Travel companies use data aggregation to figure out how much their competitors charge for a certain flight, hotel room, or rental car type.
- Then, they can make sure they price their own products as competitively as possible.
- One thing these businesses all have in common is that they can use VLOOKUP to help them achieve these goals.
- As a reminder, VLOOKUP stands for vertical lookup.
- Basically, it's a function that searches for a certain value in a column to return a corresponding piece of information.
- Earlier, we used VLOOKUP to take the value in one cell and search for a match in another.
- We were able to match a product code made up of numbers and letters that lived in one spreadsheet to the actual name of the product that lived in another.
- But before any of that can happen, we need to make sure our data is properly prepared.
- As you've heard many times, clean data is much more likely to give you accurate results.
- Let's start with the first common data-cleaning task: different data types.
- For example, a dataset might have dates formatted as numbers, or numbers represented as text strings instead of numeric values.
- When data is not in a consistent format or a format that the spreadsheet application recognizes, VLOOKUP won't know what to do with that data, and it will return an error.
- Earlier, you learned how to convert numbers to dates using the Format tool.
- Now, let's focus on converting text to numeric values.
- To do this, you could use the Format menu to select a type of number, but you could also use the VALUE function.
- VALUE is a function that converts a text string that represents a number to a numerical value.
- Here's an example.
- In this spreadsheet, the numbers in column A are currently text strings.
- We can confirm this by running a simple SUM function.
- The syntax is equals SUM, open parenthesis, and then the items you want to add together.
- Here, it's A2 to A4.
- The colon says we're including everything between these two references.
- Now you can add a closed parenthesis and press Enter, or you can click and drag on the cells you want inside the parentheses to save a little bit of time.
- The result is zero.
- That's because the function doesn't work on text strings.
- But if we apply the VALUE function, it automatically converts that text to a numeric value.
- To do that, we'll type equals VALUE, then an open parenthesis.
- Inside, we reference the cell whose value we want to convert, in this case A2.
- Now if we close the parentheses and press Enter, you'll notice that the 1, 2, 3 is numeric.
- If we drag it down the column, the 4, 5, 6 and 7, 8, 9 also become numeric.
- Now we can test it by running another SUM function.
- We'll type equals SUM and an open parenthesis, then B2, colon, and B4.
- B2, B3, and B4 are included in the sum.
- Close the parentheses and press Enter.
- Now it shows that the total is 1,368.
- The next common error comes from having extra spaces in your spreadsheet.
- As you've learned, when data is copied from one source to another, sometimes a few leading or trailing spaces tag along.
- These can cause problems when using VLOOKUP.
- We want to make sure to use TRIM during the data- cleaning process.
- TRIM automatically deletes any extra spaces added to the cell.
- Another typical mistake in VLOOKUP, which you can easily catch during data cleaning, are duplicates.
- If there are duplicate rows in the search, it will return only the first match it finds.
- As you learned before, Remove duplicates is a tool that automatically searches for and eliminates duplicate entries from a spreadsheet.
- Using Remove duplicates, as you saw in a video a little while ago, is a great way to get rid of duplicates and help make sure you find the right record during the lookup.
- It's always good to remember that clean data is the foundation that everything else is built on.
- VLOOKUP can be a very useful data-cleaning tool.
- In the next video, we'll keep exploring more ways you can use VLOOKUP.
- See you there.

## Notes

- VLOOKUP (Vertical Lookup): a function that searches for a certian value in a column to return a corresponding piece of information.
- VALUE: A function that converts a text string that represents a number to a numberical value.
- Remove duplicates: A tool that automatically searches for and eleminates duplicate entries from a spreadsheet.

## Question

Would you like to follow along with the instructor using the same spreadsheet? To use the spreadsheet template, click the link below and select "Use Template."

Link to template: [Converting numerical and text values](https://docs.google.com/spreadsheets/d/1EGwjKtU3594CPiOfHYIgYbPcEf1r-33MDVblUdDtglE/template/preview?resourcekey=0-VqjIc9-RS8nN7pkK0NVKLQ#gid=0)

OR If you don't have a Google account, you can download the spreadsheet directly from the attachment [converting-numerical-and-text-values_preparing-for-vlookup.xlsx](./resources/converting-numerical-and-text-values_preparing-for-vlookup.xlsx).

- A data analyst applies the VALUE function to a text string that represents a number, but is formatted as text. What does the VALUE function do to that text string?
  - It searches for text strings within the spreadsheet that match the value.
  - It filters any text strings in the spreadsheet that equal the value.
  - `It converts the text string to a numerical value`.
  - It changes the value of the text string to zero.

> The VALUE function converts the text string to a numerical value.

## Keypoints

- **Definition of Data Aggregation**: The video begins by reiterating that data aggregation involves gathering data from multiple sources to create a summarized collection. VLOOKUP is introduced as a tool for achieving this.
- **Examples of Data Aggregation**: Examples are given to illustrate how businesses, such as those in marketing and travel, use data aggregation. For instance, marketing companies can aggregate data from ad campaigns to analyze performance, and travel companies can use data aggregation to set competitive prices.
- **Introduction to VLOOKUP**: VLOOKUP, which stands for vertical lookup, is briefly explained. It is described as a function that searches for a specific value in a column and returns a corresponding piece of information.
- **Purpose of VLOOKUP**: VLOOKUP is highlighted as a tool that helps achieve business goals by looking up and retrieving relevant information from datasets.
- **Data Preparation for VLOOKUP**: The video emphasizes the importance of preparing data before using VLOOKUP. Clean data is stressed as more likely to yield accurate results.
- **Common Data-Cleaning Tasks**: The video covers common data-cleaning tasks, including handling different data types. It explains that inconsistent formats, such as dates formatted as numbers or numbers represented as text, can cause errors in VLOOKUP. The importance of converting text to numeric values for proper data processing is highlighted.
- **Use of VALUE Function**: The VALUE function is introduced as a tool for converting text strings representing numbers into numerical values. An example demonstrates how to use the VALUE function to convert text to numeric values in a spreadsheet.
- **Handling Extra Spaces**: The video discusses the issue of extra spaces in a spreadsheet, which can cause problems when using VLOOKUP. The TRIM function is introduced as a solution to automatically remove extra spaces during data cleaning.
- **Dealing with Duplicates**: Duplicate entries can lead to errors in VLOOKUP, and the video recommends using the "Remove duplicates" tool to automatically search for and eliminate duplicate entries from a spreadsheet.
- **Clean Data as a Foundation**: The video concludes by reinforcing the idea that clean data is the foundation for accurate results in data analytics. VLOOKUP is presented as a valuable data-cleaning tool.