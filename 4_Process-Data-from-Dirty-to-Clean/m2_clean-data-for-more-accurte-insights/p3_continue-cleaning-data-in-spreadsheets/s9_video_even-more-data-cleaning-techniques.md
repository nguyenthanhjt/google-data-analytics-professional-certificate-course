# VIDEO: Even more data-cleaning techniques

VIDEO Trancript

- Hello.
- So far you've learned about a lot of different tools and functions that analysts use to clean up data for analysis.
- Now we'll take a step back and talk about some of the really big picture aspects of clean data.
- Knowing how to fix specific problems, either manually with spreadsheet tools, or with functions, is extremely valuable.
- But it's also important to think about how your data has moved between systems and how it's evolved along it's journey to your data analysis project.
- To do this, data analysts use something called data mapping.
- Data mapping is the process of matching fields from one database to another.
- This is very important to the success of data migration, data integration, and lots of other data management activities.
- As you learned earlier, different systems store data in different ways.
- For example, the state field in one spreadsheet might show Maryland spelled out.
- But another spreadsheet might store it as MD.
Data mapping helps us note these kinds of differences so we know when data is moved and combined it will be compatible.
- As a quick reminder, compatibility describes how well two or more data sets are able to work together.
- The first step to data mapping is identifying what data needs to be moved.
- This includes the tables and the fields within them.
- We also need to define the desired format for the data once it reaches its destination.
- To figure out how this works let's go back to the merger between our two logistics associations.
Starting with the first data field, we'll identified that we need to move both sets of member IDs.
- To define the desired format, we'll choose whether to use numbers like this spreadsheet, or email addresses like the other spreadsheet.
- Next comes mapping the data.
- Depending on the schema and number of primary and foreign keys in a data source, data mapping can be simple or very complex.
- As a reminder, a schema is a way of describing how something is organized.
- A primary key references a column in which each value is unique and a foreign key is a field within a table that is a primary key in another table.
- For more challenging projects there's all kinds of data mapping software programs you can use.
- These data mapping tools will analyze field by field how to move data from one place to another then they automatically clean, match, inspect, and validate the data.
- They also create consistent naming conventions, ensuring compatibility when the data is transferred from one source to another.
- When selecting a software program to map your data, you want to be sure that it supports the file types you're working with, such as Excel, SQL, Tableau, and others.
- Later on, you'll learn more about selecting the right tool for a particular task.
- For now, let's practice mapping data manually.
- First, we need to determine the content of each section to make sure the data ends up in the right place.
- For example, the data on when memberships expire would be consolidated into a single column.
- This step makes sure that each piece of information ends up in the most appropriate place in the merged data source.
- Now, you might remember that some of the data was inconsistent between the two organizations, like the fact that one uses a separate column for suite apartment or unit number but the other doesn't.
This brings us to the next step, transforming the data into a consistent format.
- This is a great time to use concatenate.
- As you learned before, concatenate is a function that joins together two or more text strings, which is what we did earlier with our cosmetics company example.
- We'll insert a new column and then type equals concatenate, then the two text strings we want to make one.Drag that through the entire column.
- Now we have the consistency in the new merged association lists of member addresses.
- Now that everything's compatible, it's time to transfer the data to its destination.
- There's a lot of different ways to move data from one place to another, including querying, import wizards, and even simple drag and drop.
- Here's our merged spreadsheet.
It looks good, but we still want to make sure everything was transferred properly.
- We'll go into the testing phase of data mapping.
- For this, you inspect a sample piece of data to confirm that it's clean and properly formatted.
It's also a smart practice to do spot checks on things such as the number of nulls.
- For the test, you can use a lot of the data cleaning tools we discussed previously, such as data validation, conditional formatting, COUNTIF, sorting, and filtering.
- Finally, once you've determined that the data is clean and compatible, you can start using it for analysis.
- Data mapping is so important because even one mistake when merging data can ripple throughout an organization, causing the same error to appear again and again.
- This leads to poor results.
- On the other hand, data mapping can save the day by giving you a clear road map you can follow to make sure your data arrives safely at it's destination.
- That's why you learn how to do it.

## Questions

### Question 1

**Pro Tip**: Use CONCATENATE to help you format the data as it is merged.

Coming up, if you enter `=CONCATENATE(D2, E2)` as demonstrated by the instructor, the results will appear like this: **25 Dyas RdSte. 101**

You could manually clean the data later to add a space between Rd and Ste., but why not let CONCATENATE do the work for you?

Because `CONCATENATE` merges strings, you can enter an additional string to insert a space between Rd and Ste.

Enter `=CONCATENATE(D2, " ", E2)` instead and you will have an address that is formatted like this: **25 Dyas Rd Ste. 101**.

Much better!

### Question 2

In the next visualization, the merger conducted by the instructor was the combination of data from the '*Global Logistics Association*' spreadsheet that was added to the target '*International Logistics Association memberships*' spreadsheet starting at **row 73**. The final result of this combination is the data contained within the third '*Logistics Association Merger*' spreadsheet.

If you're following along with the video, you can get a feel for data validation by spot-checking the data in the Logistics Association Merger spreadsheet.

**Was all the data merged?**

One way to spot check is *manually combining the rows* from the first two datasets and comparing the results to the total number of rows in the third merger spreadsheet. Do all the rows in your resulting merger match the number of rows of data in the Logistics Association Merger spreadsheet?

**Was membership data migrated correctly?**

Randomly select a few members in the International Logistics Association spreadsheet and compare their data in the Logistics Association Merger spreadsheet. Do the same for a few members in the Global Logistics Association spreadsheet.

**Are the data formats in the merged spreadsheet consistent?**

Check the data formats for each column of the Logistics Association Merger spreadsheet.

Did you discover that the dates in the **Membership valid through** column are inconsistently formatted? Some dates have the format of 2/17/2021 and others have the format of Tuesday, November 9, 2021.

To fix this inconsistency, select the entire column (Column J), select **Format** from the main menu, select **Number**, and then choose the date format you would like all cells in the column to have.

## Keypoints

- Data mapping is crucial for understanding how data moves between systems and ensuring compatibility.
- Identify what data needs to be moved and define the desired format.
- Transform data into a consistent format using tools like CONCATENATE.
- Testing and validation ensure clean and properly formatted data for analysis.