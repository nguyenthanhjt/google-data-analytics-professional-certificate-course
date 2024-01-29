# Step-by-step: Use the SORT function in spreadsheets

This reading outlines the steps the instructor performs in the next video, [Use the SORT function im spreadsheets](https://www.coursera.org/learn/analyze-data/lecture/K6WB8/the-sort-function). In this video, the instructor demonstrates how you can use the `SORT` function to arrange data into a meaningful order to make it easier to understand, analyze, and visualize.  

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video.

## What you’ll need

If you’d like to follow along with the examples in this video, choose a spreadsheet tool. Google Sheets or Excel are recommended.

To access the spreadsheet the instructor uses in this video, click the link to the template to create a copy of the dataset. If you don’t have a Google account, download the data directly from the attachments below.

Link to dataset: [Party plan spreadsheet](https://docs.google.com/spreadsheets/d/1L1Z6b3X9WCpwzisHcxvjC5-Qett-BOMo9yg8Cz36NME/template/preview)

OR [party-plan-spreadsheet.xlsx](./resources/party-plan-spreadsheet.xlsx)

## Example 1: Sort guests by table

Use a spreadsheet function to sort guests by the table to which they’re assigned.

1. Open the [Party plan spreadsheet](https://docs.google.com/spreadsheets/d/1L1Z6b3X9WCpwzisHcxvjC5-Qett-BOMo9yg8Cz36NME/template/preview).
2. Select cell G1 and enter the equal sign `=`.
3. Enter `SORT` followed by an open parenthesis ( to begin the `SORT` function.
4. Enter the first cell from the Guest column of the spreadsheet, **A2**, followed by a colon [:], then enter the last cell from the Sent Invitation column, **D6**, followed by a comma. **A2:D6** is the range of cells over which this function will sort.
5. Enter **2** followed by a comma to specify the column by which to sort the data. Note that the function doesn't recognize letters, so use the column’s number. Column A corresponds to 1, B corresponds to 2, and so on.
6. Enter `TRUE` followed by a close parenthesis ). `TRUE` means the function will return results in ascending order, so the tables will be listed starting with table one. **Note**: To return results in descending order, enter `FALSE`.

7. Press **Enter** (Windows) or Return (Mac).

The party guests are now sorted by the table to which they’re assigned.  

## Example 2: Customized sort order

When you sort data in a spreadsheet using multiple conditions with a customized sort order, data is sorted  based on the order in which the conditions are applied to the data. To sort party guests by whether or not they've been sent an invitation and to list the guests alphabetically:

1. Highlight all the data in the party plan spreadsheet: cells **A1 to D6**.
2. In the menu, select **Data > Sort range > Advanced range sorting options**. This opens the Sort range from A1 to D6 dialog box.
3. Check the **Data has a header row** checkbox to make sure column titles aren’t included in the sorted data.  
4. From the **Sort by** drop-down list, select **Sent Invitation**.
5. Select the **A to Z** radio button to make sure the No responses are listed first and the Yes responses are listed second.
6. Select **Add another sort column** to add the additional sorting condition.
7. From the **Sort by** drop-down list, select **Guest Names** to list guests alphabetically.
8. Select the **A to Z** radio button.
9. Select `SORT`.  

This returns your customized sort order, which lists the No invitations and those guests alphabetically, followed by the Yes invitations and those guests alphabetically.
