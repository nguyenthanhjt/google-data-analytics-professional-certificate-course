# Spreadsheets versus SQL

Video transcript

- Hey there.
- So far we've learned about both spreadsheets and SQL.
- While there's lots of differences between spreadsheets and SQL, you'll find some similarities too.
- Let's check out what spreadsheets and SQL have in common and how they're different.
- Spreadsheets and SQL actually have a lot in common.
- Specifically, there's tools you can use in both spreadsheets and SQL to achieve similar results.
- We've already learned about some tools for cleaning data in spreadsheets, which means you already know some tools that you can use in SQL.
- For example, you can still perform arithmetic, use formulas and join data when you're using SQL, so we'll build on the skills we've learned in spreadsheets and use them to do even more complex work in SQL.
- Here's an example of what I mean by more complex work.
- If we were working with health data for a hospital, we'd need to be able to access and process a lot of data.
- We might need demographic data, like patients' names, birthdays, and addresses, information about their insurance or past visits, public health data or even user generated data to add to their patient records.
- All of this data is being stored in different places, maybe even in different formats, and each location might have millions of rows and hundreds of related tables.
- This is way too much data to input manually, even for just one hospital.
- That's where SQL comes in handy.
- Instead of having to look at each individual data source and record it in our spreadsheet, we can use SQL to pull all this information from different locations in our database.
- Now, let's say we want to find something specific in all this data, like how many patients wit h a certain diagnosis came in today.
- In a spreadsheet we can use the COUNTIF function to find that out, or we can combine the COUNT and WHERE queries in SQL to find out how many rows match our search criteria.
- This will give us similar results, but works with a much larger and more complex set of data.
- Next, let's talk about how spreadsheets and SQL are different.
- First, it's important to understand that spreadsheets and SQL are different things.
- Spreadsheets are generated with a program like Excel or Google Sheets.
- These programs are designed to execute certain built-in functions.
- SQL on the other hand is a language that can be used to interact with database programs, like Oracle MySQL or Microsoft SQL Server.
- The differences between the two are mostly in how they're used.
- If a data analyst was given data in the form of a spreadsheet they'll probably do their data cleaning and analysis within that spreadsheet, but if they're working with a large data set with more than a million rows or multiple files within a database, it's easier, faster and more repeatable to use SQL.
- SQL can access and use a lot more data because it can pull information from different sources in the database automatically, unlike spreadsheets which only have access to the data you input.
- This also means that data is stored in multiple places.
- A data analyst might use spreadsheets stored locally on their hard drive or their personal cloud when they're working alone, but if they're on a larger team with multiple analysts who need to access and use data stored across a database, SQL might be a more useful tool.
- Because of these differences, spreadsheets and SQL are used for different things.
- As you already know, spreadsheets are good for smaller data sets and when you're working independently.
- Plus, spreadsheets have built-in functionalities, like spell check that can be really handy.
- SQL is great for working with larger data sets, even trillions of rows of data.
- Because SQL has been the standard language for communicating with databases for so long, it can be adapted and used for multiple database programs.
- SQL also records changes in queries, which makes it easy to track changes across your team if you're working collaboratively.
- Next, we'll learn more queries and functions in SQL that will give you some new tools to work with.
- You might even learn how to use spreadsheet tools in brand new ways.
- See you next time.

## Question

A team of analysts is working on a data analytics project. How could data in a SQL database be more useful to the team than data in spreadsheets? Select all that apply.

- `They can track changes to SQL queries across the team.`
- They can use SQL to make working with smaller datasets easier.
- `They can use SQL to interact with the database program.`
- `They can use SQL to pull information from the database at the same time.`

> Data stored in a SQL database is useful to a project with multiple team members because they can access the data at the same time, use SQL to interact with the database program, and track changes to SQL queries across the team.

## Keypoints

|Spreadsheets|SQL|
|------------|---|
|Generated with a program|A language used to interact with data programs|
|Access to the data you input|Can pull information from different sources in the database|
|Stored locally|Stored across a database|
|Small datasets|Larger datasets|
|Working independently|Tracks changes across team|

- Commonalities between Spreadsheets and SQL:
  - Both spreadsheets and SQL share similarities in tools and functionalities.
  - Skills learned in spreadsheets, such as arithmetic, formulas, and data joining, can be extended to more complex tasks in SQL.
- Example of Complex Work in SQL:
  - In scenarios like managing health data for a hospital, SQL proves valuable.
  - SQL allows for the retrieval of diverse data (demographics, insurance, past visits, public health data) stored in various locations and formats within a database.
- Benefits of SQL in Handling Large and Complex Data:
  - When dealing with extensive data sources and millions of rows, SQL outperforms manual spreadsheet data input.
  - SQL facilitates the extraction and processing of information from different locations in a database efficiently.
- Comparison of Data Retrieval in Spreadsheets and SQL:
  - While spreadsheets use functions like COUNTIF, SQL employs queries like COUNT and WHERE for similar results.
  - SQL operates with larger and more complex datasets, making it more suitable for such tasks.
- Differences between Spreadsheets and SQL:
  - Spreadsheets are generated with programs like Excel or Google Sheets, executing built-in functions.
  - SQL is a language interacting with database programs (e.g., Oracle, MySQL, Microsoft SQL Server).
  - Spreadsheets are effective for smaller datasets and individual work, while SQL excels with larger datasets, offering faster and more repeatable processes.
- Accessing and Storing Data:
  - SQL can access and utilize a more extensive range of data as it can pull information from various sources in a database automatically.
  - Spreadsheets, on the other hand, only have access to manually input data.
- Use Cases and Specialties:
  - Spreadsheets are suitable for smaller datasets and independent work, offering built-in functionalities like spell check.
  - SQL is great for larger datasets, even handling trillions of rows, and is adaptable across multiple database programs.
  - SQL records changes in queries, facilitating collaborative work by tracking changes across teams.
- Future Learning:
  - The section hints at upcoming learning about additional queries and functions in SQL, expanding the analyst's toolkit.
