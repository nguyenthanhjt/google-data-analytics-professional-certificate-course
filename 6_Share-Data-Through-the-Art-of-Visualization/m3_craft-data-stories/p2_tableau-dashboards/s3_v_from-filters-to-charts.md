# Video: From fileter to charts

Video transcript

- So far, we've focused a lot on understanding our audience.
- Whether you're trying to engage people with data storytelling or creating dashboards designed for a certain person or group, understanding your audience is key.
- As you've learned, you can make dashboards that are tailored to meet different stakeholder requirements.
- To do this, it's important to think about who will be looking at the data and what they need from it.
- In this video, we'll continue exploring how to create compelling visuals to tell an interesting and persuasive data story.
- One great tool for doing this is a filter.
- You've learned about filters and spreadsheets and queries, but as a refresher, filtering means showing only the data that meets a specific criteria while hiding the rest.
- Filtering works the same way with dashboards—you can apply different filters for different users based on their needs.
- Tableau lets you limit the data you see based on the criteria you specify.
- Maybe you want to filter data and the data set to show only the last six months, or maybe you want to see information from one particular customer.
- You can even limit the number of rows or columns in a view.
- To explore these options, let's return to our world happiness example.
- Say your stakeholders were interested in only a few of the topics that affect overall happiness.
- Filtering for just gross domestic product, family, generosity, freedom, trust, and health, and then creating individual scatterplots for each would make this possible.
- You can also use filters to highlight or hide individual data points.
- For instance, if you have a scatterplot with outliers, you may want to explore what your plot would look like without them.
- However, note that this is just an example to show you how filters work; it's not okay to drop a data point just because it's an outlier.
- Outliers could be important observations, sometimes even the most interesting ones, so be sure to put on your data detective hat and investigate that outlier before deciding to remove it from your dashboard.
- Here's how to do it.
- To filter data points from the view, we can choose a single data point or click and drag in the view to select several points.
- Let's choose just one.
- Then on the tool tip that appears, we'll select "exclude" to hide it or we could have chosen to do it the other way by keeping only selected data points.
- Here's another example.
- If your data is in a table, you can filter entire rows or columns from your view.
- To do this, we'll select the rows we want in the view.
- Then, on the tool tip that appears, we'll choose to keep only those countries.
- Again, we could have also selected the data points we wanted to exclude and picked that option instead.
- Or if you like, we can even prefilter a Tableau dashboard.
- This means that your stakeholders don't have to filter the data themselves.
- Basically, by doing the filtering for them, you can save them time and effort and direct them to the important data you want them to focus on.
- Personally, I think the best thing about filters is they let you zero in on what's important.
- Sometimes I'm working with a huge data set, and I want to concentrate only on a specific area, so I'll add a filter to limit the data displayed on my dashboard.
- This cuts the clutter and gives me a simple, clear visual.
- I use filters a lot when working with data about advertising campaign performance.
- Filters help me isolate specific tactics, such a search or YouTube ads, to see which ones are working best and which ones could be improved.
- By limiting and customizing the information I'm looking at, it's much easier for me to see the story behind the numbers.
- And as I'm sure you've noticed, I love a good data story.
- As a data analyst, you'll often be relying on spreadsheets to create quick visualizations of your data to tell your story.
- Let's practice building a chart in a spreadsheet.
- To follow along, use the spreadsheet link in the previous reading, also included in the video.
- We'll be using Google Sheets, so this might look a little different in other spreadsheet platforms, like Excel.
- We'll begin by filtering just the data on how many customers purchase basic plus or premium software packages.
- To start, select the column for the software package and insert a chart.
- The spreadsheet suggests what it thinks is the best type of chart for our data, but we can choose any type of chart you'd like.
- Spreadsheet charts also let you assign different styles, access titles, a legend, and many other options.
- Feel free to explore the different functionality later on.
- We'll also cover this more in a reading.
- There's lots of different options to choose from.
- Let's say we also have data on which countries our customers are from and their overall satisfaction score for the software they purchased.
- First, highlight columns A and B, then click on "insert" and then "chart" again under "chart type." You want to select the first map option.
- Voila! Now we have a map that summarizes a customer survey scores by country.
- We can also customize this chart by clicking "customize" in the top right corner.
- Let's say we wanted to change our colors from red and green to a gradient so it's more accessible.
- We can do that by clicking "geo" and then change the min color to the lightest shade of blue, the mid color to the middle shade of blue, and the max color to the darkest shade of blue to show the spectrum of scores from low to high.
- Now we have a map chart that shows where respondents are most satisfied with their software in dark blue and least satisfied with their software in light blue.
- And this will be easier for anyone in our audience with color vision deficiencies to understand.
- Tableau and spreadsheets are common tools for creating data visualizations.
- By using their built-in functionalities like filters and charts, you can zero in on what information is most important and create compelling visuals for your audience.
- And now that we've explored some ways to create visuals, it's time to start preparing our data narrative.
- Coming up, we're going to talk more about telling stories with data and organizing presentations.
- I'll see you soon.

## Questions & Notes

If you would like to follow along with the video, click the link below and select “Use Template.”

Link to template: [Customer Service Survey Responses](https://docs.google.com/spreadsheets/d/1DWIKPvtci3Gq6Qbz15SjjY6l4wbc_4I-CpVaFDPneDA/template/preview?resourcekey=0-OOpDEJqur_5qsHXNIt2Bqg)

OR [customer-service-survey-responses.xlsx](./resources/c6-m3-p2-s2-s3_customer-service-survey-responses.xlsx)

If you don't have a Google account, you can download the spreadsheet from the attachment below.

To continue following along with the video, click the Country of Response tab (the second tab) in your copy of the spreadsheet.

### Notes

- **Filtering**: showing only the data that meets a specific criteria while hiding the rest

### Question 1: Filters in Tableau can be used for which of the following tasks? Select all that apply

- [x] To highlight a data point
- [x] To limit information
- [x] To customize information
- [ ] To organize data into a meaningful order

> Filters in Tableau can be used to limit information, customize information, or highlight a data point.

### Key Points

1. **Audience Understanding:**
   - Tailoring dashboards to meet different stakeholder requirements requires understanding the audience.
   - Data storytelling and dashboard creation involve considering who will be looking at the data and their specific needs.

2. **Importance of Filters:**
   - Filters are powerful tools for creating compelling visuals and telling persuasive data stories.
   - Filtering involves showing only data that meets specific criteria while hiding the rest.
   - Different filters can be applied for various users based on their needs.

3. **Filter Applications:**
   - Filters in Tableau can be used for tasks such as highlighting a data point, limiting information, and customizing information.
   - Filtering allows focusing on specific areas of interest, simplifying visuals, and enhancing the clarity of data stories.

4. **Filtering Examples:**
   - In the example of world happiness, filters could be applied to show data related to specific factors like gross domestic product, family, generosity, freedom, trust, and health.
   - Filtering can be applied to individual data points, excluding outliers, or to entire rows or columns in a table.

5. **Pre-filtering Dashboards:**
   - Prefiltering a Tableau dashboard involves setting up filters in advance, saving stakeholders time and effort in filtering data themselves.
   - Filters enable a clear focus on essential data points, cutting through clutter in large datasets.

6. **Filtering in Spreadsheet Platforms:**
   - Filters are also essential in spreadsheet platforms like Google Sheets.
   - Building charts in spreadsheets involves selecting and filtering specific data columns to create visualizations.

7. **Customizing Charts in Spreadsheets:**
   - Spreadsheet charts offer customization options such as assigning different styles, adding titles, legends, and more.
   - The ability to customize charts helps in creating visually appealing and informative visualizations.

8. **Data Visualization Tools:**
   - Tableau and spreadsheets are common tools for creating data visualizations.
   - Built-in functionalities like filters and charts in these tools help in zeroing in on crucial information and crafting compelling visuals.
