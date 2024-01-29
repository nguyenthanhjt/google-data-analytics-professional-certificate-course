# Sort and filter in Sheets and Excel

In this reading, you’ll examine the sorting and filtering options in Google Sheets and Microsoft Excel. Both offer basic sorting and filtering from set menu options. But if you need more advanced sorting and filtering capabilities, you can use their respective `SORT` and `FILTER` functions.

![Image of lightbulb, money icon, person icon, and an analog clock traveling into an open box Sort and filter in Sheets](./resources/img-1.png)

## Sort and filter in Sheets

Sorting in Google Sheets helps you quickly spot trends in numbers and text. For example, as the vice president of sales at a candy company, you want to improve chocolate sales in lower-performing regions—your company makes delicious chocolate and you know sales can improve. As a first step, you examine this by calculating gross (total) revenue of chocolate by sales region. In this case, you could sort the gross revenue column in **descending** (Z to A) order to find the top performing regions at the top, or sort the gross revenue column in **ascending** (A to Z) order to find the lowest performing regions at the top. Then, you can look at patterns in the best and worst regions to explore how to increase sales in the lower-performing regions.

If you want to learn more about the set menu options for sorting and filtering, start with these resources:

- [Sort and filter data](https://www.youtube.com/watch?v=VcRBHXBMKBU) (Google Help Center): instructions to sort data in alphabetical or numerical order and create filter views
- [Sort data by selecting a range of data in a column](https://www.youtube.com/watch?v=VcRBHXBMKBU): video of steps to achieve the task
- [Sort a range of data using sort criteria for multiple columns](https://blog.sheetgo.com/google-sheets-formulas/sort-formula-google-sheets/): technical tip instructions by SheetGo company to sort data across multiple columns

In addition to the standard menu options, the `SORT` function allows you to do more advanced sorting. Use this function to create custom sorting rules. You can sort the rows of a given range of data by the values in one or more columns. And you can set the sort criteria for each column. Refer to the [SORT function](https://support.google.com/docs/answer/3093150?hl=en) page for the syntax.

Like the `SORT` function, use the [FILTER function](https://support.google.com/docs/answer/3093197?hl=en) to filter by any matching criteria you like. This creates a custom filter.

As you’ve learned, you can filter data and then sort the filtered results. Using the `FILTER` and `SORT` functions together in a range of cells can programmatically and automatically achieve these results for you.

## Sort and filter in Excel

You can also sort in ascending (A to Z) and descending (Z to A) order in Microsoft Excel. Excel offers `Smallest to Largest` and `Largest to Smallest` sorting options when you’re working with numbers.

Similar to the `SORT` function in Google Sheets, Excel includes custom sort capabilities that are available from the menu. After you select the data range, click the **Sort & Filter** button to select the criteria for sorting. You can even sort by the data in rows instead of by the data in columns if you select **Sort left to right** under **Options**. (**Sort top to bottom** is the default setting to sort the data in columns.)

If you want to learn more about sorting and filtering in Excel, start with these resources:

- [Sort data in a range or table](https://support.microsoft.com/en-us/office/sort-data-in-a-range-or-table-62d0b95d-2a90-4610-a6ae-2e545c4a4654) (Microsoft Support): instructions to perform sorting in a variety of use cases
- [Excel training: sort and filter data](https://support.microsoft.com/en-us/office/video-sort-data-in-a-range-or-table-ffb9fcb0-b9cb-48bf-a15c-8bec9fd3a472#ID0EAABAAA=Transcript) (Microsoft Support): sorting and filtering videos with transcripts
- [Excel: sorting data](https://www.youtube.com/watch?v=Ep5q1cUhQas): video of how to use the **Sort & Filter** and Data menu options for sorting

Excel also has [SORT](https://support.microsoft.com/en-us/office/sort-function-22f63bd0-ccc8-492f-953d-c20e8e44b86c), [SORTBY](https://support.microsoft.com/en-us/office/sortby-function-cd2d7a62-1b93-435c-b561-d6a35134f28f), and [FILTER](https://support.microsoft.com/en-us/office/filter-function-f4f7cb66-82eb-4767-8f7c-4877ad80c759) functions. Explore how you can use these functions to automatically sort and filter your data in spreadsheets without having to select any menu options at all.

## Sort and filter manually with menus and buttons

Both Sheets and Excel feature menu options designed to let you sort and filter without using functions. For example, after selecting the data you’d like to sort in Google Sheets, you can choose **Data > Sort sheet** or **Data > Sort range** to sort that data. To filter the data, select all the columns and rows and choose **Data > Create a filter**. In Excel, you can use the Sort & filter button to bring up a user-friendly interface that guides you through sorting or filtering.

Finally, when using menus or buttons, here are a couple of best practices:

- Back up or make a copy of your data before making major changes.
- When filtering data, keep in mind that other users may also be accessing the spreadsheet. For example: Filters in Google Sheets can affect all viewers, so you should use filter views for personal filtering.

## Key takeaways

As you’ve learned, you can sort and filter data in Google Sheets and Excel with functions or by using menus and buttons. Sorting data is the process of arranging data into a meaningful order to make it easier to understand, analyze, and visualize. This can help you identify trends in the data. Filtering is the process of showing only the data that meets a specified criteria while hiding the rest. Once you’ve filtered data, you can sort it to find trends within those criteria. Menus and buttons offer the ability to do basic sort and filter functions, but you’ll need to use a function for custom sorting and filtering. 
