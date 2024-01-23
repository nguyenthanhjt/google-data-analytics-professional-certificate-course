# READING: Step-by-Step: Even more data-cleaning techniques

This reading outlines the steps the instructor performs in the next video,[Even more data-cleaning techniques](./s9_video_even-more-data-cleaning-techniques.md)
. This video teaches you different methods data analysts use in data mapping. Data mapping is the process of matching fields from one database to another. It’s critical to the success of data migration, data integration, and many other data-management activities. This video contains one activity for you to practice.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skill demonstrated in the video.

## What you’ll need

If you’d like to follow along with the example in this video, choose a spreadsheet tool, such as Google Sheets or Excel.

To access the spreadsheet the instructor uses in this video, click the link to the template to create a copy of the dataset. If you don’t have a Google account, download the data directly from the attachments below.

Link to templates:

- [International Logistics Association memberships](https://docs.google.com/spreadsheets/d/1ST8zMU2NCVgWCfwOge-8iWJguZ-NwW8C8s5p3kfC2K0/template/preview)
- [Global Logistics Association](https://docs.google.com/spreadsheets/d/186Yx3S-ejZr1cJunsal2tUV9J1abixhBUDjXbUtQT7I/template/preview)
- [Logistics Association Merger](https://docs.google.com/spreadsheets/d/1rWFRcunKBh2t6zy5zxOxcBrDyokyJZL9OJnZ5XH5tFw/template/preview)

Downloads:

- [logistics-association-merger.xlsx](resources/logistics-association-merger.xlsx)
- [global-logistics-association.xlsx](resources/global-logistics-association.xlsx)
- [international-logistics-association-memberships.xlsx](resources/international-logistics-association-memberships.xlsx)

## Example: `CONCATENATE`

`CONCATENATE` is a function that joins together two or more text strings. In the video, you’ll learn how to use `CONCATENATE` to clean data after two datasets have been combined.

- Open the dataset spreadsheet titled **Global Logistics Association**. When prompted, select **USE TEMPLATE**.
- **Insert** a new column to the right of column **E**. Label it **New Address** in cell **F1**.
- In the second row of the new column (cell **F2**), enter `=CONCATENATE (D2,E2)` and press Enter.
  - You will notice that some results need a space between the street address and the unit or suite number, such as: 25 Dyas RdSte. 101.
  - You could manually clean the data later to add a space between Rd and Ste., but `CONCATENATE` can actually do it for you. 
  - The `CONCATENATE` formula can help you format the data as it is merged by entering an additional string to insert a space between Rd and Ste.
  - Enter `=CONCATENATE(D2, " ", E2)` and you will have an address that is formatted like this: 25 Dyas Rd Ste. 101. Much better!
- Ensure the new data in the cell accurately reflects the merging of the two previous columns.
- Select cell F2 and drag down to apply the formula to all rows in the column.

## Keypoints

**Objective**: Learn how to use the CONCATENATE function for cleaning data after combining two datasets, with a focus on formatting addresses.

- Example - `CONCATENATE`:
  - Open the [Global Logistics Association](./resources/global-logistics-association.xlsx) dataset. If prompted, select **USE TEMPLATE**.
  - Insert a new column to the right of column E and label it New Address in cell **F1**.
  - In cell **F2**, enter the formula `=CONCATENATE(D2, E2)` and press Enter.
    - Observe that some results need a space between the street address and the unit or suite number (e.g., 25 Dyas RdSte. 101).
  - To add a space between Rd and Ste., use the `CONCATENATE` formula with an additional string. Enter `=CONCATENATE(D2, " ", E2)` in cell F2.
    - Now, the address should be formatted like this: **25 Dyas Rd Ste. 101**.
  - Confirm that the new data accurately reflects the merging of the two previous columns.
  - Select cell **F2** and drag down to apply the formula to all rows in the column.
