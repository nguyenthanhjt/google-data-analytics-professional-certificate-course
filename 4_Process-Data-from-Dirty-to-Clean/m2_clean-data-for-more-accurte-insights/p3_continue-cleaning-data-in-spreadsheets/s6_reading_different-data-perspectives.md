# Step-by-Step: Different data perspectives

This reading outlines the steps the instructor performs in the next video, [Different data perspectives](./s7_video_different-data-perspectives.md)
. The video teaches you different methods data analysts use to view data differently and how looking at different views leads to more efficient and effective data cleaning.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video

## What you’ll need

If you’d like to follow along with the examples in this video, choose a spreadsheet tool. Google Sheets or Excel are recommended.

To access the spreadsheet the instructor uses in this video, click the link to the template to create a copy of the dataset. If you don’t have a Google account, download the data directly from the attachments below.

Link to template: [Cosmetics, Inc](https://docs.google.com/spreadsheets/d/1J8wiEi7R9Jt3kNOjV1Bp-w1Zw1GvIbXgd78EeoXT9Mg/template/preview).

OR file [cosmetics-inc_data-for-pivot-table-and-`VLOOKUP`.xlsx](./resources/cosmetics-inc_data-for-pivot-table-and-`VLOOKUP`.xlsx)

## Example 1: Pivot tables

A pivot table is a data summarization tool. It can be used in data processing and in data cleaning, for which pivot tables offer a quick, clutter-free view of your data. Pivot tables help sort, reorganize, group, count, total, or average data in a dataset.

1. In the Cosmetics Inc. spreadsheet, select the data you need to include. In this case, select the entire spreadsheet by dragging from the top-left cell to the bottom-right cell that contains data.

2. Select **Insert**, then **Pivot Table**. Choose **New sheet** and **Create**. Google Sheets creates a new sheet where you can define the pivot table.

3. To add specific data to your pivot table, refer to the **Pivot table editor** on the right side of the window. For example, in the video, the instructor says they want to view only the most profitable products—the ones for which Cosmetics, Inc. has at least $10,000 in orders.
   - a. In the **Pivot table editor** panel, next to **Rows**, select **Add**.
   - b. From the columns list, select **Total**.
   - c. Below **Rows**, from the **Order** dropdown list, select **Descending** to put the most profitable items at the top.
   - d. To add another row with the product codes, next to **Rows**, select **Add**.
   - e. From the column list, select **Products**.
   - f. Notice that the top two most ordered products are **15143Exfo** and **3279Masc**. The rest of the orders total less than $10,000.

## Example 2: ``VLOOKUP``

`VLOOKUP` is a spreadsheet function that vertically searches for a certain value in a column to return a corresponding piece of information. It's rare for all of the data an analyst will need to be in the same place. Usually, you'll have to search across multiple sheets or even different databases. `VLOOKUP` helps bring the information together.

1. In the Cosmetics Inc. spreadsheet on the **Sheet 1** tab, select a cell in the first empty column adjacent to the top row of your data, such as H2.
2. In the selected cell, enter `=VLOOKUP(A2, 'Sheet 2'!A1:B31, 2, false)`
   - a. **Note**: This references information in another sheet. Make sure you have **Sheet 2** in your workbook.
   - b. This formula will take the value in cell **A2** of **Sheet 1** and check for that value in **Sheet 2** among the cells from **A1:B31** in the 2nd column (which corresponds with the 2 in the formula). Because the formula includes **“false,**” it will search only for an exact match. It will then output the value of column B in Sheet 2 as the result.
3. Press **Enter** to input the formula. The result is LashX Mascara.
4. Next, **select the cell** and **drag** the fill handle in the lower-right corner down to populate the other cells in the sheet with the formula.
5. To identify the products mentioned, select **Edit > Find and Replace**. In the Find text box, enter the product codes, then press **Enter**.

## Example 3: Plotting

The plotting tool allows analysts to quickly create a graph, chart, table, or other visual from data. Plotting is useful for identifying skewed data or outliers.

1. In Sheet 1 of the Cosmetics, Inc. spreadsheet, select column B, which contains the prices.
2. Select Insert > Chart.
   - a. By default, Google Sheets creates a bar chart.
   - b. Drag the chart to the side so you can view the data in the sheet.
3. Check for obvious outliers and fix them in the spreadsheet. For example, you might notice that an item in the middle of the chart has an extremely low price of $0.73. The decimal point is in the wrong place. In cell B15, correct this price to $7.30, and notice that Google Sheets automatically updates the chart.
