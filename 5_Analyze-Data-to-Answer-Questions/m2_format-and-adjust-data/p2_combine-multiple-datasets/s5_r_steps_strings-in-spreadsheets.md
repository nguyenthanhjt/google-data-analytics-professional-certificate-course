# Step-by-Step: Strings in spreadsheets

This reading outlines the steps the instructor performs in the next video, [Strings in spreadsheets](./s6_v_string-in-spreadsheets.md). In this video, the instructor demonstrates the `LEN`, `LEFT`, `RIGHT`, and `FIND` functions and discusses how you can use them to better understand your data.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference tool if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video.

## What you’ll need

If you’d like to access the spreadsheet the instructor uses in this video, click the link to the dataset to create a copy. If you don’t have a Google account, you may download the data directly from the attachments below. Note that this is a larger database so it may take a moment or two to load.

Link to the Citi Bike dataset: [Citi Bike Trip Data]([./resources/](https://docs.google.com/spreadsheets/d/1ZetYs2n7csR1pI92hOuMfV_RXmxbOh1UOOxx1KdDv0E/template/preview?usp=sharing&resourcekey=0-qpI7g9md35n648x5jgNwaQ)).

OR [citi-bike-trip-data.xlsx](./resources/citi-bike-trip-data.xlsx)

Note: If the directions in the video do not work for the version of Excel you have, visit the free online training center [Microsoft Excel for Windows Training](https://support.microsoft.com/en-us/office/excel-video-training-9bc05390-e94c-46af-a5b3-d7c22f6990bb), and search for these functions to learn how to use them in Excel.

## Example 1: The `LEN` function

The `LEN` function calculates a string’s length. Use this formula to check the length of the datetime strings in column C.

1. Open the [Citi Bike Trip Data]([./resources/](https://docs.google.com/spreadsheets/d/1ZetYs2n7csR1pI92hOuMfV_RXmxbOh1UOOxx1KdDv0E/template/preview?usp=sharing&resourcekey=0-qpI7g9md35n648x5jgNwaQ)). spreadsheet.
2. In cell **B2**, enter the equals sign [=] to begin the function.
3. Enter `LEN`, followed by an open parenthesis [(].
4. Select cell **C2**. Then add a close parenthesis [)].
5. Press **Enter**. The result, 19, indicates the string in cell **C2** is 19 characters.

## Example 2: The `FIND` function

The `FIND` function locates specific characters and substrings in a string. All of the start-time (column C) and stop-time (column D) strings in the spreadsheet have a space between the date and the time. Use the FI`ND function to determine where in the string this space is located.  

1. Select cell **B3** and enter the equals sign[=].
2. Enter `FIND` followed by an open parenthesis [(].
3. Enter quotation mark, then space, then close quotation mark [" "] to specify that you want to find a space.
4. Select cell **C3** and add a close parenthesis [)].
5. Press **Enter** to run the formula. This function returns 11, indicating that the space is the 11th character in the string.  

**Note**: `FIND` is case sensitive, so always make sure you input the substring correctly.

## Example 3: The `RIGHT` function

Use the `RIGHT` function to select a specific number of characters on the right side of a cell. Here, you want to return the substring that represents time, which is contained within the eight characters to the right of the space.

1. Reopen the spreadsheet so you are working with an unaltered version of the document [Citi Bike Trip Data]([./resources/](https://docs.google.com/spreadsheets/d/1ZetYs2n7csR1pI92hOuMfV_RXmxbOh1UOOxx1KdDv0E/template/preview?usp=sharing&resourcekey=0-qpI7g9md35n648x5jgNwaQ)) spreadsheet.
2. In cell **B2**, enter the equals sign [=].
3. Enter `RIGHT` followed by an open parenthesis [(].
4. Select cell **C2** then enter a comma [,].
5. Enter **8** to specify that you want the function to return the eight rightmost characters in the string.
6. Add a close parenthesis [)] to complete the formula.
7. Press **Enter** to run the formula. The time stamp from the start-time data string has now been isolated in cell **B2**.
8. Double-click the fill handle in cell **B2** to fill the rest of the column.
9. Enter **Time** in cell **B1** to add a column header.

## Example 4: The `LEFT` function

Use the `LEFT` function to select a specific number of characters on the left side of a cell. Here, you want to return the date substring, which is the 10 characters to the left of the space. These characters represent the start date.

1. Right-click cell **B**.
2. Select **Insert 1 column left** to create a new column **B** for the date substring.
3. Enter **Date** in cell **B1** to add a column header.
4. Enter the equals sign [=] in cell **B2**.
5. Enter **LEFT** followed by an open parenthesis [(].
6. Select cell **D2** then enter a comma [,]. **Note**: You added a column, so the start time column is now column D.
7. **Add a comma** [,] after **D2** in the formula.
8. Enter **10**, to indicate that you want to return the first 10 characters in the date string.
9. Add a close parenthesis [)] to complete the formula. **Note**: The instructor enters 11, which will return the date substring and the space.
10. Press **Enter**. The date from the start-time data string has now been isolated in the new cell **B2**.
11. Double-click the fill handle in cell **B2** to fill the rest of the column.
