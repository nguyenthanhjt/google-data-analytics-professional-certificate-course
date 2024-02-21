# Upload the employee dataset to BigQuery

This reading outlines the steps you need to perform before watching the video and following along in the step-by-step guide, [Explore how JOINs work](./s3_v_explore-how-joins-work.md).

## What you will need

Download the two .csv files from the attachments below:

[departments-table_understanding-joins.csv](./resouces/departments-table_understanding-joins.csv)

[employees-table_understanding-joins.csv](./resouces/employees-table_understanding-joins.csv)

Then, log in to your BigQuery account and follow along with this reading to upload the employee data provided as two new tables.

## Prepare for the next video

### Create a new dataset

1. Open your BigQuery console and select the project to which you’ll upload data. For the purpose of this reading, the example project is named **dac5bigquery**. Your project will have a different name.

2. From the **Explorer** pane, select the **Actions** icon (the three vertical dots) next to your project name. Then select **Create dataset**.

3. In the **Create dataset** window, enter **employee_data** for the **Dataset ID**.

4. Make sure the **Location type** is set to **Multi-region** with **US(multiple regions in the United States)** selected.

5. Leave the **Advanced** options set to their default settings.

6. Select **CREATE DATASET** to add the dataset to your project. It will now appear under your project in the Explorer pane. If you don’t see the new dataset listed, select the arrow next to your project in the **Explorer** pane to expand its contents.

7. In the Explorer pane, select the employee_data dataset you just created. The Dataset info window opens in the Details pane.

### Create the employees table

Create a table for the employees within your employee_data dataset. To do this:

1. Select **+ CREATE TABLE** from the options in the Details pane. Under Source:

    From the dropdown in the field Create table from, select Upload.

    From the Select file field, select BROWSE. Then, find and select the [Employees Table - Understanding JOINS](https://d3c33hcgiwev3.cloudfront.net/TMwinKTQQ2aYTZGdcL0Fog_84586bd2265a4888af22e8060747c8e1_Employees-Table---Understanding-JOINS.csv?Expires=1700006400&Signature=XeqsCQhRu8D7cS7Ew8kaS3ySfbc2aYOuk~bTZZ8eBdF07KQtiMu4sAgRB4V1xboPLvCry4H61bXFNjqBT1PmbKFo8dgzPbmOUsS0msC6Fca6c-gj95HVM1PJq5pRctkQiC8OaBKml3T9KRs0lctwoqeJI-HKUo5e7hs2dF-q~EA_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A) .csv File you downloaded previously.

    The file format should be automatically detected after selecting the Employee Table .csv file. If it’s not, select CSV from the File format drop-down.

2. Under Destination:

   - Enter **employees** in the **Table** field.
   - **Project**, **Dataset**, and **Table type** will be automatically filled. You do not need to update these fields.  

3. Under **Schema**, select the **Auto detect** checkbox.

4. Select **CREATE TABLE**. The employees table will be nested under **employee_data** in the **Explorer** pane.

### Create a departments  table

Next, create a table for the departments within the employee_data dataset. To do this:

1. Select the employee_data dataset from the Explorer panel.

2. Select + CREATE TABLE from the options located in the main editor window.

3. Under Source:

    From the dropdown in the field Create table from, select Upload from the list of options.

    From the Select file field, select BROWSE. Find and select the [Departments Table - Understanding JOINS](https://d3c33hcgiwev3.cloudfront.net/9vVSOuERRjusAUScVM-rOw_d98f88a17db84f198dee412210c13ae1_Departments-Table---Understanding-JOINS.csv?Expires=1700006400&Signature=BTJ2YLesayzmJfmfNXNbbpPk1iw5Gtn-S5VuVwvjSBrHHVcx43MzcGPWP6skOxWPQZATx2JVKw2x0aR9HKbxe80VLIK9enqXKETlIOcPYpxjDw52KFdA-Ugi4gpqegDFSl8E1bqumIk-tPxDwRe9SKnBDAeTxXGgroVc~ssKB88_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A).csv File you downloaded previously.

4. The file format may be automatically detected after selecting the Departments Table .csv file. If it’s not, select CSV from the File format drop-down.

5. Under the Destination section:

   - Enter **departments** in the Table field.
   - **Project**, **Dataset**, and **Table type** will be automatically filled out so you do not need to update these fields.

6. Under **Schema**, select the **Auto detect** checkbox.

7. Select **CREATE TABLE** in the Create Table window. The departments table will appear under the employee_data dataset listed within your project.

### Verify the data

Make sure that you’ve uploaded the tables correctly by previewing the tables you just created.

1. From the **Explorer** pane, select the **employees** table.

2. Select the **Preview** tab to verify that you have the following data:
3. Select the departments table.
4. Select the Preview tab to verify that you have the following data:

When your data previews match these instructions, you are ready to follow along with the step-by-step guide and video on [Explore how JOINs work](./s3_v_explore-how-joins-work.md).
