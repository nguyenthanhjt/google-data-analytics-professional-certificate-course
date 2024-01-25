# Discussion Prompt: Debug SQL code

You’ve been learning how to use SQL to query databases and clean your data. When using a programming language, it’s common to make coding errors. For example, if you use improper syntax, the database won’t know what you’re trying to communicate. Everyone makes coding errors, from experienced programmers to new learners. So it’s helpful to know some strategies for resolving errors.

Think about some of the errors you have encountered when working with SQL. Then, explain why you chose these errors. Next, write down your top three tips for resolving them. Feel free to find more information online before you start writing. [Stack Overflow](https://stackoverflow.com/)
 is a great place to start, or you can search online to find other helpful resources.

Please submit two or more paragraphs (150-200 words) in your written response. Then, go to the [discussion forum](https://www.coursera.org/learn/process-data/discussions) to read what other learners have written, and choose at least two posts to comment on and discuss.

## My Response

When working with SQL, encountering coding errors is a common part of the learning process. One error I frequently encountered was related to syntax issues. In SQL, a misplaced comma or a missing parenthesis can lead to syntax errors, making it challenging for the database to interpret the query correctly. Often, these errors resulted from oversight or typos during query composition.

Another type of error I encountered was related to ambiguous column references, especially when working with multiple tables. If a column is present in more than one table included in the query, specifying which table the column belongs to is crucial. Failure to do so can lead to errors like "ambiguous column name," as the database cannot determine the exact source of the column.

To address these issues, my top three tips for resolving SQL errors are as follows:

Thoroughly Review Syntax: Before executing a query, carefully review the syntax to ensure all keywords, commas, and parentheses are correctly placed. Utilize online resources like Stack Overflow or the official documentation to identify and correct syntax errors.

Specify Column Sources: When working with multiple tables, explicitly specify the source table of each column in the SELECT, FROM, and WHERE clauses. This helps eliminate ambiguity and ensures the database accurately interprets the query.

Use Error Messages Wisely: Pay attention to error messages provided by the database management system. These messages often offer insights into the nature of the error and guide you toward the specific part of the query that needs correction.

