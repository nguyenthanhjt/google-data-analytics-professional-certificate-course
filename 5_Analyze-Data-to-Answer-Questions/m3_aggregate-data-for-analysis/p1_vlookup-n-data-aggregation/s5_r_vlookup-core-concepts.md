# `VLOOKUP` core concepts

Spreadsheet functions can be used to quickly find information and perform calculations using specific values. `VLOOKUP`, or Vertical Lookup, is one such function that vertically searches for a certain value in a column to return a corresponding piece of information. In this reading, you’ll examine the intricacies of this extremely useful function so you understand how it works when you use it to analyze data.

## `VLOOKUP` functionality

`VLOOKUP` searches for a search term, called a `search_key`, in one column of a spreadsheet. When the `search_key` is found, the function returns the data from another column of the row from which it  was located. `VLOOKUP` returns only the value that corresponds to the first item it matches. So, if there are multiple matching values, the spreadsheet will return only data about the first one.

## `VLOOKUP` use cases

Here are two common reasons why you might use `VLOOKUP`:

Populating data in a spreadsheet. Perhaps a store manager is tracking incoming shipments before a busy holiday. They could use `VLOOKUP` to look up product ID codes in a product spreadsheet and retrieve the corresponding product information from another spreadsheet. This would help the manager know how many stock clerks they need to schedule to work when the shipments arrive.

Merging data from one spreadsheet with data in another. If a teacher keeps one spreadsheet for student grades and another for attendance, they could use `VLOOKUP` to combine the spreadsheets. That way, they could search for a particular student in the attendance sheet, and `VLOOKUP` would pull the corresponding attendance record into the grades spreadsheet.

## `VLOOKUP` syntax

`VLOOKUP` is available in both Microsoft Excel and Google Sheets. Here, you’ll explore its syntax in Google Sheets. Refer to the resources at the end of this reading for more information about `VLOOKUP` in Microsoft Excel.

`VLOOKUP`’s syntax is:

```text
VLOOKUP`(`search_key`, range, index, is_sorted)
```

The following sections explain each of the four parts of the syntax.

`search_key`: This is the value the function will search for. It can be a number, text string, or cell reference.

`range`: This is the range of cells over which the function will search and return information. The first column in the range is searched. When the search key is found, the index from that row is returned.

For example, if you search for the `search_key` in column B and return the data from column D, the range would need to include columns B through D, such as the range B2:D10. If you specified a range of A2:D10, the function would search for the search term in column A.

The `search_key` must be to the left of the information you want the function to return. This may require you to move columns around before you use `VLOOKUP`. For example, if you plan to search for the `search_key` column D, but the information you want the function to return is in column A, you must rearrange your columns before using `VLOOKUP`.

`index`: This is the position of the column that contains the data to be returned. The first column in the range is column number 1, and each column is numbered sequentially to the right.

For example, if the range is B2:D10 and you want to return a value from column D, the index number would be 3. If the index is not between 1 and the number of columns in range, the error message`#VALUE!` will be returned.

`is_sorted`: This indicates whether to return an approximate or exact match. For example, if you’re searching for Google, then google would not count as a match.

- To return an exact match, set `is_sorted` to `FALSE`. This is recommended.
- To return an approximate match, set `is_sorted` to `TRUE`. The nearest match (less than or equal to the `search_key`) is returned. To use this option to obtain accurate results, you must sort your data in ascending order. But, you could still find a value.
- If neither `TRUE` nor `FALSE` are selected, the function will default to `TRUE`.

## The #N/A error

`#N/A` indicates that a matching value can't be returned because no matches were found.

## Key takeaways

Use `VLOOKUP` to search for a value in a column and return a corresponding piece of information. It’s a very useful tool for data professionals, as it enables them to combine data from multiple sources and find information quickly. Keep in mind that the column that matches the `search_key` in a `VLOOKUP` formula should be on the left side of the data. The range must include both the column being searched and the column that contains the information being returned. TRUE means an approximate match, and FALSE means an exact match on the `search_key`. 

## `VLOOKUP` resources for Microsoft Excel

`VLOOKUP` may slightly differ in Microsoft Excel, but the overall concepts can still be generally applied. Refer to the following resources if you’re working with Excel:

- [How to use `VLOOKUP` in Excel](https://support.microsoft.com/en-us/office/vlookup-function-0bbc8083-26fe-4963-8ab8-93a18ad188a1): This tutorial includes a video to help you get a general understanding of how the `VLOOKUP` function works in Excel, as well as practical examples to look through.
- [`VLOOKUP` in Excel tutorial](https://www.youtube.com/watch?v=d3BYVQ6xIE4): Follow along in this video lesson and learn how to write a `VLOOKUP` formula in Excel and master time-saving useful tips and tricks.
- [23 things you should know about `VLOOKUP` in Excel](https://exceljet.net/things-you-should-know-about-vlookup): Explore this list of `VLOOKUP` facts, common challenges and their solutions.
- [How to use Excel's `VLOOKUP` function](https://edu.gcfglobal.org/en/excel-tips/how-to-use-excels-vlookup-function/1/): This article shares a specific example about applying `VLOOKUP` in your searches.
- [`VLOOKUP` in Excel vs Google Sheets](https://infoinspired.com/sheets-vs-excel-formula/vlookup-formula-in-excel-and-google-sheets/): This guide offers a `VLOOKUP` comparison of Excel and Google Sheets.
