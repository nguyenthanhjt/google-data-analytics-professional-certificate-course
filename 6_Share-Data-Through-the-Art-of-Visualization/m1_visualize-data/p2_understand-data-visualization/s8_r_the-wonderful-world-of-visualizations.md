# The Wonderful World of Visualizations

As a data analyst, you will often be tasked with relaying information and data that your audience might not readily understand. Presenting your data visually is an effective way to communicate complex information and engage your stakeholders. One question to ask yourself is: “what is the best way to tell the story within my data?” This reading includes several options for you to choose from (although there are many more).

## Line Chart

A **line chart** is used to track changes over short and long periods of time. When smaller changes exist, line charts are better to use than bar graphs. Line charts can also be used to compare changes over the same period of time for more than one group.

**Example:**

```plaintext
Year | Graduation Rate
-----|----------------
2008 | 87%
2009 | 89%
2010 | 92%
2011 | 92%
2012 | 96%
```

From this table, you are able to present your data in a line chart like this:

![Line graph depicting an increase of high school graduation rates from 87% in 2008 to 96% in 2012](./resources/img-10.png)

**Example (Gender Comparison):** Maybe your data is more specific than above. For example, let’s say you are tasked with presenting the difference of graduation rates between male and female students. Then your chart would resemble something like this:

![Line graph depicting an increase in high school graduation for male and female students over the years from 2008 to 2012](./resources/img-11.png)

## Column Chart

**Column charts** use size to contrast and compare two or more values, using height or lengths to represent the specific values.

**Example:**

```plaintext
Month    | Vehicles Sold
---------|---------------
August   | 2,800
September| 3,700
October  | 3,750
November | 4,300
December | 4,600
```

Visually, it would resemble something like this:

![Bar graph of 2020 of increasing monthly car sales from August to December](./resources/img-12.png)

**Example (Competing Car Brands):**

What would this column chart entail if we wanted to add the sales data for a competing car brand?

![Double bar graph of monthly car sales for Car A and Car B increasing from August to December](./resources/img-13.png)

## Heatmap

Similar to bar charts, **heatmaps** also use color to compare categories in a data set. They are mainly used to show relationships between two variables and use a system of color-coding to represent different values.

**Example:**
![Heatmap of varying climates for different cities around the world between June to January ranging from hot to cold](./resources/img-14.png)

## Pie Chart

The pie chart is a circular graph that is divided into segments representing proportions corresponding to the quantity it represents, especially when dealing with parts of a whole.

**Example:**

```plaintext
Movie Category | Preference
---------------|-----------
Comedy         | 41%
Drama          | 11%
Sci-fi         | 3%
Romance        | 17%
Action         | 28%
```

Visually, it would resemble something like this:

![Pie chart of five movie categories and percentage of audience preference](./resources/img-15.png)

## Scatterplot

**Scatterplots** show relationships between different variables. Scatterplots are typically used for two variables for a set of data, although additional variables can be displayed.

**Example:** For example, you might want to show data of the relationship between temperature changes and ice cream sales. It would resemble something like this:

![Scatterplot showing the rising sales of ice cream as the temperature rises, rising to 500 around 100 degrees Fahrenheit](./resources/img-16.png)

As you may notice, the higher the temperature got, the more demand there was for ice cream—so the scatterplot is great for showing the relationship between the two variables.

## Distribution Graph (Histogram)

A **distribution graph** displays the spread of various outcomes in a dataset.

**Example:** Let’s apply this to real data. To account for its supplies, a brand new coffee shop owner wants to measure how many cups of coffee their customers consume, and they want to know if that information is dependent on the days and times of the week. That distribution graph would resemble something like this:
![Histogram showing cups of coffee purchased across all 7 days of the week, largest consumed midweek on Wednesday around 100](./resources/img-17.png)

From this distribution graph, you may notice that the amount of coffee sales steadily increases from the beginning of the week, reaching the highest point mid-week, and then decreases towards the end of the week.

If outcomes are categorized on the x-axis by distinct numeric values (or ranges of numeric values), the distribution becomes a **histogram**. If data is collected from a customer rewards program, they could categorize how many customers consume between one and ten cups of coffee per week. The histogram would have ten columns representing the number of cups, and the height of the columns would indicate the number of customers drinking that many cups of coffee per week.

Reviewing each of these visual examples, where do you notice that they fit in relation to your type of data? One way to answer this is by evaluating patterns in data. Meaningful patterns can take many forms, such as:

- **Change**: This is a trend or instance of observations that become different over time. A great way to measure change in data is through a line or column chart.
- **Clustering**: A collection of data points with similar or different values. This is best represented through a distribution graph.
- **Relativity**: These are observations considered in relation or in proportion to something else. You have probably seen examples of relativity data in a pie chart.
- **Ranking**: This is a position in a scale of achievement or status. Data that requires ranking is best represented by a column chart.
- **Correlation**: This shows a mutual relationship or connection between two or more things. A scatterplot is an excellent way to represent this type of data pattern.

## Studying Your Data

Data analysts are tasked with collecting and interpreting data as well as displaying data in a meaningful and digestible way. Determining how to visualize your data will require studying your data’s patterns and converting it using visual cues. Feel free to practice your own charts and data in spreadsheets. Simply input your data in the spreadsheet, highlight it, then insert any chart type and view how your data can be visualized based on what you choose.