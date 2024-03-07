# Video : Link multiple datasets in Tableau

Video transcript

- Hi and welcome back.
- In this video, we're going to use Tableau to link multiple datasets.
- This lets analysts compare all datasets in the same visualization, visualize comparisons and combinations of data, and share more complex projects.
- You can put this video on one side of the screen and follow along in another window.
- You might notice your screen is slightly different from the video.
- That's okay.
- Tableau updates its interface from time to time, but the general steps will stay the same.
- Feel free to pause this video as you work in your own Tableau workspace before continuing to the next step.
- To begin, we're going to need to download the four datasets we'll use for this activity, click the link to create a copy of the datasets and download them.
- If you don't have a Google account, download the datasets directly from the attachments.
- Now imagine this scenario.
- You're working as a data analyst for a policy research institute.
- For your current project, you need to create a visualization that shows the CO_2 emissions per capita for each country from 2000-2011.
- You'll also provide information about each country's population, GDP, and energy use.
- Let's get started.
- First, log into Tableau Public.
- If you haven't created an account, refer to the earlier reading, logging into Tableau Public.
- Go to the circle, then choose "My profile." From there, select "Create a Viz." This will open the Tableau Public interface.
- The connect to data window will pop up.
- From here, you can go to the Files tab and upload the CO_2 dataset.
- Now, go to the data source tab.
- Then the connections column.
- From here, choose the plus icon to add another dataset.
- First, add energy, then add GDP total and total population.
- Now we'll have four datasets loaded into Tableau.
- You can proceed to linking them with JOINs Tableau has already added energy into the multiple connections area.
- We can remove it by dragging it back to the connections column.
- Now let's create JOINs as a reminder, inner and outer joins are types of relationships that can be used to combine data based on common columns of information.
- To set up our first JOIN, we'll select CO_2 under connections.
- Beneath that in the sheet section, click and drag CO_2 data cleaned to the multiple connection section.
- Then double click the box created by the dataset.
- This opens a physical table and lets us create JOINs To set the first JOIN, select the energy dataset under connections and drag the energy sheet beneath it to the right side of the CO_2 data cleaned box.
- A pop-up window for a JOIN will appear.
- It will automatically populate with year from CO_2 data cleaned and Year 1 from energy.
- If not, put year on the left side of the chart and Year 1 on the right side.
- Then choose "Add" from JOIN clause under year.
- Select "Country Name" from the down on the left side and "Country" on the right side.
- After that, use the X to close the drop-down menu, we need to fix something in our dataset.
- Year and Year 1 have a number sign above them.
- We can click those number signs and select date instead, to change the data type for each column.
Play video starting at :4:4 and follow transcript4:04
Now, join the other datasets, choose "GDP Total" under Connections.
- Then under sheets, drag the GDP total sheet into the white space underneath the energy box.
- The pop-up window should already be populated with Year 1 under data source and year GDP total under GDP total.
- Before adding any additional joins, the data type for year GDP total needs to be changed.
- We'll make its data type date just like we did with the other year columns.
- Now continue setting the join.
- Choose the Venn diagram between Energy and GDP total, then add new JOIN clause under Year 1.
- A drop-down menu will appear.
- Under CO_2 data cleaned, select "Country name".
- Then the empty field under GDP total across from country name.
- Set the right side of the JOIN to country one.
- Then close the join pop-up.
- We'll repeat this process for total population, the last dataset we downloaded.
- When we drag the sheet to create the JOIN, the window should already be populated with year under data source and year total population under total population.
- Change year total population to the date data type to match the other year columns.
- Then select the "Venn diagram" to edit the JOIN and click "Add new JOIN clause" under year.
- Under CO_2 Data Cleaned, choose "Country name" then on the right side of the row, country total population.
- Close the pop-up.
- If you haven't yet, be sure to update your data by clicking on the "Update Now" button.
- Nice.
- You've joined four different sources of data.
- Check out your new dataset.
- While your dataset CO_2 went from 1960-2011, your other datasets went from 2000-2015.
- The intersection, the years they have in common only includes 2000-2011.
- This is the time span that we need.
- However, there are some changes we still need to make.
- Some of the data types need to be converted.
- Similar to when you change your year columns to date types, you'll need to change the energy use and current GDP columns.
- Above the energy use column is an ABC icon.
- This means is a string type.
- Select it to open a drop-down and change it to number decimal.
- Current GDP is also a string type but needs to be a whole number instead.
- Choose the ABC icon to change it to number whole.
- Now we get to make our visualization.
- To begin, choose the Sheet 1 tab, you'll notice a column on the left side of the screen.
- Under CO_2 Data Cleaned, drag country name to the detail square.
- Drag CO_2 per capita to the color square.
- Then choose the square and edit colors.
- Select the palette dropdown and change it from automatic to red-green diverging.
- Check the boxes for stepped color and reversed because green is generally viewed as a good thing when it comes to CO_2 emissions, you want the colors to move toward red as emissions worsen.
- Click the "Show Advanced" dropdown.
- Then the start and end boxes.
- Put zero into the start column and 62 at the end column.
- Then close the window.
- Drag year from under CO_2 data cleaned into the filters area.
- Choose years, next, all, and then okay.
- In the filters box, right-click on "Year," "Year," select "Show Filter." The filter will appear on the right side of the screen.
- On the far right side of the screen, choose the arrow to the right of year , select "Single value." Now the areas will be colored only for the values of each year.
- Select any year between 2000-2011 to view that year's CO_2 emissions.
- Make sure to save your progress by clicking published as icon or hovering over the file tab and selecting "Save." If you are asked to create an extract, return to the data source tab and click "Create Extract," then click "Save" again.
- Congratulations.
- You've linked your data and made a comprehensive dataset in Tableau.
- The more visualizations you make, the more you'll be able to share complex analyses and insights.
Hi and welcome back.
- In this video, we're going to use Tableau to link multiple datasets.
- This lets analysts compare all : Added to Selection.
- Press [⌘ + S] to save as a note

## Questions & Notes

### Scenario

Create a visualization that shows the CO2 emissions per capita for each country from 2000-2011

### Important note

This is a companion tutorial. After you follow along with the instructor, you can practice again with the hands-on activity that comes next.

(Optional) If you prefer, you may skip this video tutorial and move on to the activity now. Link to activity: [Hands-On Activity: Practice linking data in Tableau](./s2_pq_activity_link-multiple-datasets-in-tableau.md).

To follow along with the instructor in Tableau Public, click the links to the spreadsheet templates below and select "Use Template."

Links to datasets: [CO2](https://docs.google.com/spreadsheets/d/1NBV7WYvOX-WbB6f7JLm0jaaf5E-L9Me5fKVFgBkNJKo/template/preview), [Energy](https://docs.google.com/spreadsheets/d/1OZQu4Sd6TaZMRyvECZNK9rjKPnl41ToS_ZWg3xwRnCE/template/preview), [Population](https://docs.google.com/spreadsheets/d/1wNQzkMZQGL9I0j7PYW1qdt9UoBYv94Yswn1ry8YBFC8/template/preview), and [GDP](https://docs.google.com/spreadsheets/d/17YOeJcActweV5vJc1JjJIyMcy89Qm5AFIP1X26ymMSM/template/preview#gid=1769006840)

OR if you don't have a Google account, you can download the spreadsheets directly from the attachments below:

- [CO2-Dataset.xlsx](./resources/CO2-Dataset.xlsx)
- [Energy-Dataset.xlsx](./resources/Energy-Dataset.xlsx)
- [GDP-Dataset.xlsx](./resources/GDP-Dataset.xlsx)
- [Population-Dataset.xlsx](./resources/Population-Dataset.xlsx)

## **Key Points:**

1. **Linking Multiple Datasets in Tableau:**
   - Linking multiple datasets in Tableau allows analysts to compare, visualize, and share complex projects with combined data.

2. **Downloading Datasets:**
   - Download the four datasets (CO2, Energy, GDP, Population) from the provided links or directly from the attachments.

3. **Scenario:**
   - Imagine working as a data analyst for a policy research institute.
   - The goal is to create a visualization showing CO2 emissions per capita for each country from 2000-2011, along with information on population, GDP, and energy use.

4. **Tableau Public:**
   - Log into Tableau Public and go to the "My profile" > "Create a Viz" to open the Tableau Public interface.

5. **Connecting Datasets:**
   - Upload the CO2 dataset in the connect to data window.
   - Navigate to the data source tab and connections column.
   - Add other datasets (Energy, GDP, Population) by clicking the plus icon.

6. **Joining Datasets:**
   - Perform JOINs to link datasets based on common columns (e.g., year, country name).
   - Adjust data types and create relationships between datasets.

7. **Data Conversion:**
   - Convert data types where needed, ensuring consistency for effective visualization.

8. **Creating Visualization:**
   - Go to Sheet 1.
   - Drag relevant variables (e.g., country name, CO2 per capita, year) to different sections.
   - Customize visualization by editing colors, setting filters, and creating a meaningful layout.

9. **Saving and Updating Data:**
   - Save progress by clicking the publish icon or using the file tab.
   - If prompted, create an extract to save the linked data.

10. **Exploration:**
    - Explore the comprehensive dataset with linked information from multiple sources.

