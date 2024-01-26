# Verification of data cleaning

Video transcript

- Hey there. In this video, we'll continue building on the verification process. As a quick reminder, the goal is to ensure that our data-cleaning work was done properly and the results can be counted on. You want your data to be verified so you know it's 100 percent ready to go. It's like car companies running tons of tests to make sure a car is safe before it hits the road. You learned that the first step in verification is returning to your original, unclean dataset and comparing it to what you have now. This is an opportunity to search for common problems. After that, you clean up the problems manually. For example, by eliminating extra spaces or removing an unwanted quotation mark. But there's also some great tools for fixing common errors automatically, such as TRIM and remove duplicates. Earlier, you learned that TRIM is a function that removes leading, trailing, and repeated spaces and data. Remove duplicates is a tool that automatically searches for and eliminates duplicate entries from a spreadsheet. Now sometimes you had an error that shows up repeatedly, and it can't be resolved with a quick manual edit or a tool that fixes the problem automatically. In these cases, it's helpful to create a pivot table. A pivot table is a data summarization tool that is used in data processing. Pivot tables sort, reorganize, group, count, total or average data stored in a database. We'll practice that now using the spreadsheet from a party supply store. Let's say this company was interested in learning which of its four suppliers is most cost-effective. An analyst pulled this data on the products the business sells, how many were purchased, which supplier provides them, the cost of the products, and the ultimate revenue. The data has been cleaned. But during verification, we noticed that one of the suppliers' names was keyed in incorrectly.
- We could just correct the word as "plus," but this might not solve the problem because we don't know if this was a one-time occurrence or if the problem's repeated throughout the spreadsheet. There are two ways to answer that question. The first is using Find and replace. Find and replace is a tool that looks for a specified search term in a spreadsheet and allows you to replace it with something else. We'll choose Edit. Then Find and replace. We're trying to find P-L-O-S, the misspelling of "plus" in the supplier's name. In some cases you might not want to replace the data. You just want to find something. No problem. Just type the search term, leave the rest of the options as default and click "Done." But right now we do want to replace it with P-L-U-S. We'll type that in here. Then click "Replace all" and "Done."
- There we go. Our misspelling has been corrected. That was of course the goal. But for now let's undo our Find and replace so we can practice another way to determine if errors are repeated throughout a dataset, like with the pivot table. We'll begin by selecting the data we want to use. Choose column C. Select "Data." Then "Pivot Table." Choose "New Sheet" and "Create."
- We know this company has four suppliers. If we count the suppliers and the number doesn't equal four, we know there's a problem. First, add a row for suppliers.
- Next, we'll add a value for our suppliers and summarize by COUNTA. COUNTA counts the total number of values within a specified range. Here we're counting the number of times a supplier's name appears in column C. Note that there's also function called COUNT, which only counts the numerical values within a specified range. If we use it here, the result would be zero. Not what we have in mind. But in other special applications, COUNT would give us information we want for our current example. As you continue learning more about formulas and functions, you'll discover more interesting options. If you want to keep learning, search online for spreadsheet formulas and functions. There's a lot of great information out there. Our pivot table has counted the number of misspellings, and it clearly shows that the error occurs just once. Otherwise our four suppliers are accurately accounted for in our data. Now we can correct the spelling, and we verify that the rest of the supplier data is clean. This is also useful practice when querying a database. If you're working in SQL, you can address misspellings using a CASE statement. The CASE statement goes through one or more conditions and returns a value as soon as a condition is met. Let's discuss how this works in real life using our customer_name table. Check out how our customer, Tony Magnolia, shows up as Tony and Tnoy. Tony's name was misspelled. Let's say we want a list of our customer IDs and the customer's first names so we can write personalized notes thanking each customer for their purchase. We don't want Tony's note to be addressed incorrectly to "Tnoy." Here's where we can use: the CASE statement. We'll start our query with the basic SQL structure. SELECT, FROM, and WHERE. We know that data comes from the customer_name table in the customer_data dataset, so we can add customer underscore data dot customer underscore name after FROM. Next, we tell SQL what data to pull in the SELECT clause. We want customer_id and first_name. We can go ahead and add customer underscore ID after SELECT. But for our customer's first names, we know that Tony was misspelled, so we'll correct that using CASE. We'll add CASE and then WHEN and type first underscore name equal "Tnoy." Next we'll use the THEN command and type "Tony," followed by the ELSE command. Here we will type first underscore name, followed by End As and then we'll type cleaned underscore name. Finally, we're not filtering our data, so we can eliminate the WHERE clause. As I mentioned, a CASE statement can cover multiple cases. If we wanted to search for a few more misspelled names, our statement would look similar to the original, with some additional names like this.
- There you go. Now that you've learned how you can use spreadsheets and SQL to fix errors automatically, we'll explore how to keep track of our changes next.

## Question

Would you like to follow along with the instructor using the same spreadsheet? To use the spreadsheet template, click the link below and select "Use Template."

Link to template: [Jeff’s Party Planet - Data for Cleaning](https://docs.google.com/spreadsheets/d/1RaDdSEp2V6D09FE6LOFkiJGv9CMT83GIV_U9YnY2rvI/template/preview?resourcekey=0-IU2-k90CX0mrt0ebwrvwDw#gid=0)

OR file [jeffs-party-planet_data-for-cleaning.xlsx](./resrouces/jeffs-party-planet_data-for-cleaning.xlsx)

> The menu option has slightly changed. To insert a pivot table select `Insert` and `Pivot Table`.
>  
> **Note**: This section of the video does not use the Jeff's Party Planet dataset you downloaded earlier. The example that the instructor uses is not from a public dataset and is just intended to demonstrate how a CASE statement works.

## Key Points from Section 4: Verification of Data Cleaning

- This section focuses on the verification process of cleaned data, emphasizing the importance of ensuring data accuracy before analysis. Key points include:

- Objective of Verification:
  - Verification ensures that data cleaning was executed correctly, and the results are trustworthy.
  - Similar to car companies running tests to ensure a car's safety before it hits the road, data should undergo verification before being used for decision-making.
- Manual and Automatic Cleaning:
  - Manual cleanups involve revisiting the original unclean dataset, identifying common problems, and making manual edits.
  - Automatic tools like TRIM and remove duplicates are effective for fixing common errors automatically.
- Pivot Tables for Verification:
  - Pivot tables are powerful tools for data summarization in data processing.
  - They help sort, reorganize, group, count, total, or average data stored in a database.
  - Demonstrated with an example of a party supply store interested in finding the most cost-effective supplier.
- Using Find and Replace:
  - Find and Replace is a tool for looking for a specified search term in a spreadsheet and replacing it.
  - Demonstrated by correcting a misspelled supplier's name ("Plos" to "Plus") using Find and Replace.
- Pivot Table Example:
  - Pivot tables help identify repeated errors in a dataset.
  - Creating a pivot table to count the occurrences of supplier names and identify any anomalies.
- SQL CASE Statement:
  - In SQL, a CASE statement is used to handle conditions and return values based on those conditions.
  - Example: Correcting misspelled names in a customer_name table using a CASE statement in a SELECT query.
- Keeping Track of Changes:
  - Verification helps in identifying and correcting errors, ensuring the reliability of the data.
  - The next step is explored, focusing on how to keep track of changes made during the cleaning process.