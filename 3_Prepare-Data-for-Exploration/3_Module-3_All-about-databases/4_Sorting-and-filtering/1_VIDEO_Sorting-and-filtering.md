# Sorting and filtering

[VIDEO](./resources/1_VIDEO_Sorting-and-filtering.mp4) and [transcript](./resources/1_VIDEO_Sorting-and-filtering.txt)

- In the past few videos, you've learned about both internal and external data. Now I'll show you how to focus on only the data that's relevant to the problem you're trying to solve. This is useful if you're working with a very large complex spreadsheet, which data analysts encounter all the time. Having lots of data can make it difficult to quickly find and analyze the information you need. No two analytics projects are the same. Often data analysts process, view, and use data very differently, even if it comes from the exact same source. Here's an example. Check out this spreadsheet that shows a company's sales reps and where they work. Different data analysts might want different information from the spreadsheet, and that's where sorting and filtering comes in. Sorting and filtering the data in a spreadsheet helps us customize the way data is presented. They can also organize data so analysts can zoom in on the pieces that matter. Think of it like a magnifying glass for our data. Let's begin with sorting. Sorting involves arranging data into a meaningful order to make it easier to understand, analyze, and visualize. Data can be sorted in ascending or descending order, and alphabetically or numerically. Sorting can be done across all of a spreadsheet or just in a single column or table. You can also sort by multiple variables. For instance, if our data set contains both city and state fields, we can sort first by city and then by state.
- Anytime you're sorting data, it's always a good idea to freeze the header row first. To do this, we'll highlight the row. Then from the view menu, choose freeze and one row.
- This locks the row in place. Now when we scroll down the sheet, the header row stays visible so we know the category of each column.
- Looks good to me. Now let's sort the entire spreadsheet. We'll sort by city first. To do this, select the city column,
- then use the drop-down arrow to sort the sheet. Select A to Z.
- This will sort all the columns from A to Z by row, with the selected column being the primary sort criteria. The cities are now sorted alphabetically, and they're still grouped with the corresponding states, sales reps, and auto parts. The details across each row are automatically kept together when sorting a particular section, as you can see here. Multiple criteria sorting is another very useful data analysis tool. For instance, let's say we want to see a list of sales reps by the cities and states in which they work. First, we select the entire data set,
- then choose data and sort range.
- In the dialog box, make sure that "Data has header row" is highlighted.
- That way row A, city, states, sales rep, and auto parts won't be part of the sort.
- Then in the sort by drop-down menu, select state and the sort order A to Z. Now add another sort column. In the "then by" drop-down, select city and the sort order A to Z.
- Finally, select Sort.
- Now we can search the data to easily find a sales rep who works in a particular state and city. Sorting is useful when you want to look at everything in a spreadsheet in alphabetical or numerical order. But sometimes data analysts want to isolate a particular piece of information. To do this, they use a filter. Filtering means showing only the data that meets a specific criteria while hiding the rest. A filter simplifies a spreadsheet by only showing us the information we need. For example, we could add a filter to see only the sales reps who worked with a particular product. To do this, we first select Data and Create a filter. Choose the column with the data we need. In this case, Auto Parts. Filter buttons will appear in the corner of each column header. To filter our spreadsheet by auto part, click the button in the Auto Parts header. In this example, let's say we want to only see sales reps who worked with rims. Remove the check marks from the categories we don't want to see, which is everything except for rims.
- Then select okay.
- The filter temporarily hides anything that doesn't meet the condition. But note that, even though they aren't visible, they're still there. When it's time to view the entire area spreadsheet again, simply turn off the filter.
- Sorting and filtering are very important tools in the data analyst's toolbox. In the next video, you'll discover even more ways to narrow in on the exact information you need for any data analysis project.

## Question

- Would you like to follow along with the instructor using the same spreadsheet? To use the template for the spreadsheet, click the link below and select "Use Template."

Link to template: [Sales Rep Cities, States, and Parts](https://docs.google.com/spreadsheets/d/1rA5zeXih2y95tRzaApsSJPa7NpT5hlcgwRUfXoKuzLM/template/preview#gid=0)
OR If you don't have a Google account, you can download the spreadsheet directly from the attachment [Sales-Rep-Cities-States-and-Parts](./resources/Sales-Rep-Cities-States-and-Parts.xlsx):

- The menu option has slightly changed. Select Data and Sort range, and then choose Advanced range sorting options to view the dialog box shown.

## Keypoints

- Sorting:
  - Sorting arranges data in a meaningful order to make it easier to understand, analyze, and visualize.
  - It can be done in ascending or descending order, alphabetically or numerically.
  - Freezing the header row is essential when sorting to keep column labels visible while scrolling.
- Multiple Criteria Sorting:
  - Sorting can be done based on multiple variables, providing a more detailed and refined organization of data.
- Filtering:
  - Filtering shows only the data that meets specific criteria, hiding the rest.
  - Filters simplify a spreadsheet by displaying only the necessary information.
  - Filtering allows for isolating specific pieces of information based on set conditions.
- Applying Filters:
  - Filters can be applied to columns to show only data that meets certain criteria.
  - The filtered data is temporarily hidden, and the filter can be turned off to view the entire dataset.
