# Ungraded Plugin: Start validating

Ensuring data integrity
Multiple choice exercise

Validating data
Ivan is a data analyst working on an annual sales report for a popular ice cream chain. Answer the questions Ivan faces as he validates data for his report.

## 1. Ice cream club members get free ice cream for their birthday. After running a query to see how many members got their free ice cream last year, Ivan noticed some null values.

The head of marketing explained to Ivan that members can visit as many locations as they want on their birthday. Ivan realized this meant the field should not be defined as a yes/no binary. Instead, it is better represented as a numeric value, up to the actual number of locations visited.

> Validating a data type means checking that the data matches the data type defined for the field.

## 2. To track all sales, Ivan assigned a primary key to every item on the menu from 1 to 60. After running a query to find the most popular menu items, he wondered why he couldn’t find any beverage sales.

After reviewing the table, he realized he forgot to assign values to the five beverages on the menu, so he added those to the menu table, bringing the range to 1 to 65.

> Validating a data range means checking that the data falls within an acceptable range of values defined for the field.

## 3. Ivan ran a query to discover the top neighborhoods where ice cream club members live.

After running the query, he noticed that several zip code results contained letters—but in his country, zip codes can only contain numeric values.

> Validating data constraints means checking that data meets certain conditions or criteria, such as type of characters.

## 4.Ivan wanted to measure how long ice cream pint inventory sits in company freezers. He ran a query to pull pint production dates and shipping dates. Next, he noticed that some production dates came after their shipping date. This told Ivan there must be an error in the data.

> Validating data consistency means checking that the data makes sense in the context of other related data.

## 5.After working with an advertising agency, the ice cream shop received five different jingle options to use in their new commercial. Ivan stored these files in his database as MP3 files.

When he ran a query for the jingles, he got null values. He went back into the database to see why the MP3 files wouldn’t show up.

> Validating data structure means checking that the data follows or conforms to a set structure, such as MP3 files or HTML code.

## 6.After clearly defining that zip code values must have only numeric values, Ivan ran his query again to find out where club members live. But he noticed some results had six or more values.

Zip codes in his country should only have five numeric digits. So he went back to verify that the endings of strings are better defined within the table.

> Code validation means checking that the application code systematically performs any of the previously mentioned validations during user data input.