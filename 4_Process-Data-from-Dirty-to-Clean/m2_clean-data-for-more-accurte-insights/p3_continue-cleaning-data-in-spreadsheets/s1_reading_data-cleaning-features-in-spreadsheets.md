# Step-by-Step guide: Data-cleaning features in spreadsheets

This reading outlines the steps the instructor performs in the next video, section 2 [Data-cleaning features in spreadsheets](./s2_video_data-cleaning-features-in-spreadsheets.md). In the video, the instructor explains how to use menu options in spreadsheets to fix errors.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video.

## What you’ll need

If you’d like to follow along with the examples in this video, choose a spreadsheet tool. Google Sheets or Excel are recommended.

To access the spreadsheet the instructor uses in this video, click the link to the template to create a copy of the dataset. If you don’t have a Google account, download the data directly from the attachments below.

- Link to logistics data: [International Logistics Association Memberships - Data for Cleaning](https://docs.google.com/spreadsheets/d/1jmxXS6ZJEMtaoli5__qApb9LE_nXkU2ysf5c8N1tiQA/template/preview)
- Link to cosmetics data: [Cosmetics Inc. - Data for Cleaning](https://docs.google.com/spreadsheets/d/12U9Y4IVAGwml7XWBBgC4j9l0cCjqIZlqJc9vu3jr6Ig/template/preview?resourcekey=0-ds9iuh8tsuB7PwGd2dHMDA#gid=0)

OR attachments:

- [international-logistics-association-memberships_data-for-cleaning.xlsx](./resources/international-logistics-association-memberships-data.xlsx)
- [cosmetics-inc_ata-for-cleaning.xlsx](./resources/cosmetics-inc_data.xlsx)

## Example 1: Use conditional formatting to highlight blank cells

Conditional formatting is a spreadsheet tool that changes how cells appear when values meet specific conditions.

1. Open the spreadsheet [International Logistics Association Memberships - Data for Cleaning](https://docs.google.com/spreadsheets/d/1jmxXS6ZJEMtaoli5__qApb9LE_nXkU2ysf5c8N1tiQA/template/preview).

2. Select the range of cells to which you’ll apply conditional formatting. In this example, you’ll select columns **A** through **L**, except for columns **F** and **H**. To select all columns except for F and H:
   a. Select cell **A** to highlight column **A**.
   b. Hold down the **SHIFT** key and at the same time use your mouse to select cell **E**. This will highlight all the columns between **A** and **E**.
   c. To select the remainder of the columns, hold down the CONTROL (Windows) or COMMAND (Mac) key while you select cells G, I, J, K, and L.
   d. Columns **A** through **L** in your spreadsheet should be highlighted except Column **F** and Column **H**.
   e. From the menu, select Format, then Conditional formatting. The columns you’ve selected should turn a light shade of green, and a new Conditional format rules tool will appear. Additionally, the Apply to range field should indicate the cells you’ve selected.
   f. Next, apply a condition to these cells to change the cell color if the cell is empty. In the Format cells if drop-down, select Cell is empty.
   g. Select the Formatting style field. Select a bright color from the drop-down to make the blank cells stand out.
   h. Select Done.

## Example 2: Remove duplicates

Remove duplicates is a spreadsheet tool that automatically searches for and eliminates duplicate entries from a spreadsheet. This is faster and easier than searching the data by scrolling through it.

- Create a copy of your dataset by right clicking the **Association ABC membership** tab and selecting **Duplicate**. This is a good practice, as it protects against accidentally deleting important data. Continue working in the new sheet, **Copy of Association ABC memberships**.
- In the menu, select **Data**, then **Data cleanup**, then **Remove duplicates**.
- Check the box next to **Data has header row**.
- Check the box next to **Select All** to inspect the entire spreadsheet.
- Select **Remove duplicates**.

## Example 3: Format dates consistently

Format dates to make all of the data in your spreadsheet consistent. This makes items easier to find and manipulate.

- Select column **J** (Membership valid through), which contains dates.
- From the menu, select **Format**, then **Number**, then **Date**.

## Example 4: Use split to separate data into columns

The split menu option is helpful when you have more than one piece of data in a cell and you want to separate those pieces of data into different cells.

- Select column **L** (Certification).
- In the menu, select **Data**, then **Split text to columns**.
- The delimiter (for example, a comma) will be automatically detected.
- If needed, specify the separator manually in the dropdown that appears in your spreadsheet.

## Example 5: Use split to fix numbers stored as text

`SPLIT` is a spreadsheet function that divides text around a specified character and puts each fragment into a new, separate cell.

- Open the spreadsheet [Cosmetics Inc. - Data for Cleaning](https://docs.google.com/spreadsheets/d/12U9Y4IVAGwml7XWBBgC4j9l0cCjqIZlqJc9vu3jr6Ig/template/preview?resourcekey=0-ds9iuh8tsuB7PwGd2dHMDA#gid=0).
- Notice that cell **F12** contains an error.
- Select column **E** (Total).
- In the menu select **Data**, then select **Split text to columns**.
- This removes the quotation marks from cell **E12**, so the spreadsheet recognizes the data in the cell as a number, resolving the error in cell **F12**.
