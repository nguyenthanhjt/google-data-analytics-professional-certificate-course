# From one type to another

Video transcript

- Hey there! So far, we've learned about typecasting data with SQL as a way of converting data from one type to another in databases.
- Now I want to check out another way to format data types within spreadsheets.
- In this video, we'll talk more about why making sure your data is formatted properly is so important and how to format numbers and convert units of measurement in your spreadsheets.
- Let's get started.
- Sometimes, you need to convert data when you're working with spreadsheets.
- That might mean changing numbers into dates, strings, percentages, or even currency.
- It's important to double check that all of your data is in the right format for your analysis.
- Sometimes even after cleaning and processing data, it still might not be in the right format you need.
- Let's think back to the table with movie data from before.
- There were a lot of different data types that included numbers, such as dates, budgets, and text strings, like actors' names.
- These are distinct values, but the spreadsheet doesn't always automatically know that.
- Here's an example.
- Let's say you wanted to sort the movies in this spreadsheet by most recent.
- If the spreadsheet cast them as strings instead of dates, it might sort them alphabetically.
- Until you change the data type, you won't be able to sort them the way you want.
- It's also possible that your datasets contain inconsistent units of measurement that you'll need to convert.
- Like say, a table that includes both US dollars and English pounds.
- That's why it's important to check those data types again, so you don't run into any problems during the actual analysis.
- Think about the incorrectly cast dates in our movie table.
- If your boss needed a list of the 20 most recent movies, but your spreadsheet was organized alphabetically instead of by the most recent, you wouldn't be giving her the list of movies she needed.
- Incorrectly formatted data can lead to time-consuming mistakes in your analysis, and might end up affecting your stakeholders' decision-making.
- But taking the time early on to convert and format your data can help you avoid that.
- And now that you know why you'll need to convert data types while working in spreadsheets, let's find out how.
- First, let me show you a really useful menu for specifying data types in spreadsheets.
- Here's the movie data table we use before, but now the money columns aren't typed as currency.
- On the toolbar at the top of the sheet, you'll find a menu that can help you convert these numbers into specific data types.
- It gives you a lot of choices just from the drop-down menu, such as number, currency, date, percentage....
- And if you click to open the full menu, there's even more options, including one for a custom number format.
- We know that we want these columns to be in currency format, so let's do that.
- All I have to do is select this column and then hit the currency shortcut.
- And now it's all typed correctly.
- But it doesn't stop there.
- You can go even further and convert the unit of measurement you're using.
- For this example, let's check out a different table.
- Imagine that you're working with a weather channel to gather data about daily temperatures.
- You have a table with some data about daily observations on the temperature, wind speed, and precipitation in this area.
- Right now, the temperatures are in Fahrenheit, but for your analysis you need them to be in Celsius.
- No problem.
- All you need to do is use the CONVERT function to change the unit of measurement.
- We'll use this empty column here.
- Here's the first temperature in the table.
- We'll input the CONVERT function in our new column to change it to Celsius.
- Then we need to put what cell we want converted.
- And finally, we're going to convert.
- And presto! Now this cell has the right unit of measurement for your analysis.
- You can simply apply it to the rest of this column.
- Now this temperature data is all in Celsius, and your unit of measurement is consistent across the table.
- And here's another tip.
- When adding data to tables using a formula, go back and paste the data in as values afterwards.
- That way they're locked in.
- Otherwise the cell stays as a formula and could get confusing when you start working with the data.
- So let's do that now.
- We'll copy the values and then right click in a new column.
- There's an option for "Paste special." And there's an option to "Paste values only." And now we have the static values in this column.
- Making sure your data is in the right format before you start analysis is so important.
- Do this, and your analysis will return the kinds of answers you're really searching for.
- And now you know some ways to typecast numbers and convert units of measurement in spreadsheets.
- You can feel confident your data is formatted the right way.
- Next up, we'll talk more about adjusting your data for analysis and data validation.
- See you soon.

## Notes

- Incorrectly formatted data can:
  - Lead to mistakes
  - Take time to fix
  - Affect stakeholder's decision-making

## Question

To convert the temperature in cell B2 in a Google spreadsheet from degrees Celsius to degrees Fahrenheit, what is the correct syntax for the CONVERT function?

- =CONVERT(B2, "F", "C")
- =CONVERT(B2, "Fahrenheit", "Celsius")
- =CONVERT(B2, "C", "F")
- =CONVERT(B2, "Celsius", "Fahrenheit")

> In Google Sheets, to convert the temperature in cell B2 from degrees Celsius to degrees Fahrenheit, the correct syntax for the CONVERT function is =CONVERT(B2, "C", "F").

## Keypoints

- Importance of Data Formatting:
  - Data often needs to be converted in spreadsheets, such as changing numbers into dates, strings, percentages, or currency.
  - Incorrectly formatted data can lead to sorting and analysis errors, impacting decision-making.
- Addressing Data Type Challenges:
  - Example: Sorting movies by the most recent date might be problematic if dates are cast as strings instead of actual dates.
  - Inconsistent units of measurement, like mixing US dollars and English pounds, can create challenges.
- Menu for Specifying Data Types:
  - Spreadsheets offer a useful menu for specifying data types.
  - The toolbar at the top provides options like number, currency, date, percentage, and custom number formats.
  - Demonstrates converting columns into currency format using the toolbar.
- CONVERT Function for Unit Conversion:
  - Illustrates using the CONVERT function to change the unit of measurement.
  - Example: Converting temperatures from Fahrenheit to Celsius in a weather data table.
  - Emphasizes the importance of consistency in unit measurement across the table.
- Paste Values to Lock Data:
  - Advises pasting data as values after using formulas to avoid confusion.
  - Demonstrates copying values, right-clicking in a new column, selecting "Paste special," and choosing "Paste values only."
- Importance of Proper Data Format:
  - Incorrectly formatted data can lead to mistakes, consume time for fixes, and impact stakeholder decision-making.
  - Ensuring data is in the right format before analysis is crucial for accurate results.
