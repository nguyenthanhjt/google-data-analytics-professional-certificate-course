# *Course challenge*

## 1 Scenario 1, question 1-5

You’ve just started a new job as a data analyst. You’re working for a midsized pharmacy chain with 38 stores in the American Southwest. Your supervisor shares a new data analysis project with you.She explains that the pharmacy is considering discontinuing a bubble bath product called Splashtastic. Your supervisor wants you to analyze sales data and determine what percentage of each store’s total daily sales come from that product. Then, you’ll present your findings to leadership.You know that it's important to follow each step of the data analysis process: ask, prepare, process, analyze, share, and act. So, you begin by defining the problem and making sure you fully understand stakeholder expectations.One of the questions you ask is where to find the dataset you’ll be working with. Your supervisor explains that the company database has all the information you need. Next, you continue to the prepare step. You access the database and write a query to retrieve data about Splashtastic. You notice that there are only 38 rows of data, representing the company’s 38 stores. In addition, your dataset contains five columns: Store Number, Average Daily Customers, Average Daily Splashtastic Sales (Units), Average Daily Splashtastic Sales (Dollars), and Average Total Daily Sales (All Products).

1. You know that spreadsheets work well for processing and analyzing a small dataset, like the one you’re using. To get the data from the database into a spreadsheet, what should you do?

- Download the data as a .CSV, then import it into a spreadsheet.
- Copy and paste the data into a spreadsheet.
- Use Tableau to convert the data into a spreadsheet.
- Email a copy of the dataset to your company email address.

2. Scenario 1 continued

You’ve downloaded the data from your company database and imported it into a spreadsheet. IMPORTANT: To answer questions using this dataset for the scenario, click the link below and select the “Use Template” button

Now, it’s time to process the data. As you know, this step involves finding and eliminating errors and inaccuracies that can get in the way of your results. While cleaning the data, you notice that information about Splashtastic is missing in one of the rows. You are unsure of how to proceed, so the best course of action is to ask your supervisor for guidance.

- True
- False

`True`. The best course of action when you notice missing information or uncertainties in the data is to ask your supervisor for guidance. It's important to clarify any issues or uncertainties to ensure that the data analysis process is accurate and reliable.

3. Scenario 1 continued

Once you’ve found the missing information, you analyze your dataset. During analysis, you create a new column F. At the top of the column, you add the attribute Average Percentage of Total Sales - Splashtastic.

Fill in the blank: An attribute is a characteristic or _____ of data used to label a column.

- `Quality`
- Observation
- Collection
- Number

4. Scenario 1 continued

Next, you determine the average total daily sales over the past 12 months at all stores. The entire range of cells that contain these sales are E2:E39. The correct syntax is =AVERAGE(E2:E39).

- True
- False

True. The syntax `=AVERAGE(E2:E39)` is correct for determining the average total daily sales over the past 12 months at all stores in the range of cells E2:E39.

5. Scenario 1 continued

You’ve reached the share phase of the data analysis process. What can you do in this phase to share the Splashtastic sales insights you've discovered?

- Revisit the analyze phase.
- Establish a repository for the data.
- Present your findings to stakeholders.
- Present your findings to customers.

In the share phase of the data analysis process, you can `Present your findings to stakeholders` to share the Splashtastic sales insights you've discovered.

## Scenario 2, questions 6-10

You’ve been working for the nonprofit National Dental Society (NDS) as a junior data analyst for about two months. The mission of the NDS is to help its members advance the oral health of their patients. NDS members include dentists, hygienists, and dental office support staff.

The NDS is passionate about patient health. Part of this involves automatically scheduling follow-up appointments after crown replacement, emergency dental surgery, and extraction procedures. NDS believes the follow-up is an important step to ensure patient recovery and minimize infection.

Unfortunately, many patients don’t show up for these appointments, so the NDS wants to create a campaign to help its members learn how to encourage their patients to take follow-up appointments seriously. If successful, this will help the NDS achieve its mission of advancing the oral health of all patients.
Your supervisor has just sent you an email saying that you’re doing very well on the team, and he wants to give you some additional responsibility. He describes the issue of many missed follow-up appointments. You are tasked with analyzing data about this problem and presenting your findings using data visualizations.

An NDS member with three dental offices in Colorado offers to share its data on missed appointments. So, your supervisor uses a database query to access the dataset from the dental group. The query instructs the database to retrieve all patient information from the member’s three dental offices, located in zip code 81137.
The table is dental_data_table, and the column name is zip_code. You have written the following query, but received an error when it ran. What is the clause that will correct this query?

```sql
SELECT *
FROM dental_data_table
WHERE dental_data_table = 81137
```

- WHERE zip_code =81137
- WHERE zip_code =81137
- WHER=81137
- WHERE_zip_code =81137

7. Scenario 2 continued

The dataset your supervisor retrieved and imported into a spreadsheet includes a list of patients, their demographic information, dental procedure types, and whether they attended their follow-up appointment. To use the dataset for this scenario, click the link below and select “Use Template.”

The patient demographic information includes data such as age, gender, and home address. You review the demographic data, paying particular attention to geography. 
What geographic aspect of the data may negatively impact fairness?

- The patients all live in the same country.
- `The patients all live in the same zip code.`
- The patients all live in the same city.
- The patients all live in houses.

The geographic aspect of the data that may negatively impact fairness is:

The patients all live in the same zip code.
Having all patients in the same zip code could introduce bias and limit the generalizability of findings, as it may not represent a diverse range of geographic locations and demographics.

8. Scenario 2 continued

As you’re reviewing the dataset, you notice that there are a disproportionate number of senior citizens. So, you investigate further and find out that this zip code represents a rural community in Colorado with about 800 residents. In addition, there’s a large assisted-living facility in the area. Nearly 300 of the residents in the 81137 zip code live in the facility.

You recognize that’s a sizable number, so you want to find out if age has an effect on a patient’s likelihood to attend a follow-up dental appointment. You analyze the data, and your analysis reveals that older people tend to miss follow-ups more than younger people.

So, you do some research online and discover that people over the age 60 are 50% more likely to miss dentist appointments. Sometimes this is because they’re on a fixed income. Also, many senior citizens lack transportation to get to and from appointments.

With this new knowledge, you write an email to your supervisor expressing your concerns about the dataset. He agrees with your concerns, but he’s also impressed with what you’ve learned and thinks your findings could be very important to the project. He asks you to change the business task. Now, the NDS campaign will be about educating dental offices on the challenges faced by senior citizens and finding ways to help them access quality dental care.

Fill in the blank: Changing the business task involves _____ a new question or problem to be solved.

- `defining`
- recording
- sharing
- analyzing

Changing the business task involves defining a new question or problem to be solved.

9. Scenario 2 continued

You continue with your analysis. In the end, your findings support what you discovered during your online research: As people get older, they’re less likely to attend follow-up dental visits.

But you’re not done yet. You know that data should be combined with human insights in order to lead to true data-driven decision-making. So, your next step is to share this information with people who are familiar with the problem professionally. They’ll help verify the results of your data analysis.

The people who are familiar with a problem professionally and help verify the results of data analysis include customers and competitors.

- True
- `False`

The statement is false because the people who are familiar with a problem professionally and help verify the results of data analysis are typically experts, colleagues, or stakeholders in the field related to the analysis. They may include subject matter experts, researchers, domain specialists, or even end-users of the data. Customers and competitors, while important in business contexts, are not typically the individuals who validate and verify the results of data analysis. Instead, they may benefit from the insights generated through data analysis.

10. Scenario 2 continued

The subject-matter experts are impressed by your analysis. The team agrees to move to the next step: data visualization. You know it’s important that stakeholders at NDS can quickly and easily understand that older people are less likely to attend important follow-up dental appointments than younger people. This will help them create an effective campaign for members.

It’s time to create your presentation to stakeholders. It will include a data visualization that demonstrates the lifetime trend of people being less likely to attend follow-up appointments as they get older.  

For this, a pie chart will be most effective.

- True
- `False`

A pie chart is not the most effective choice for demonstrating a lifetime trend of people being less likely to attend follow-up appointments as they get older. Pie charts are typically used to display parts of a whole and are best suited for illustrating the composition of a single data set at a specific point in time. In this case, a line chart or a bar chart would be more appropriate for showing trends over time, such as the relationship between age and attendance of follow-up appointments. These types of charts allow for the clear representation of data trends and patterns across different age groups.
