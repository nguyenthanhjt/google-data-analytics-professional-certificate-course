# Course 5 - Module 1 challenge

## Question 1: A data analyst at a retail company sorts customer data in a spreadsheet. They sort all data by ranking in the Purchase Amount column, keeping together all data across rows. What spreadsheet tool are they using?

- `Sort Sheet`
- Sort Together
- Sort Rank
- Sort Document

## Question 2:Fill in the blank: To filter for all students in the Sophomore table who live in Fairfield County, a data professional uses the _____ clause in SQL

- LIMIT
- `WHERE`
- FILTER
- EXCEPT

## Question 3:A junior data analyst performs several calculations on a dataset. What phase of analysis is the analyst in?

- `Transform data`
- Format and adjust data
- Organize data
- Get input from others

## Question 4:Which of the following statements accurately describe sorting and filtering? Select all that apply

- Filtering enables data professionals to view the data that has bugs or errors.
- `Sorting enables data analysts to rank data based on a specific metric.`
- `Filtering is effective at reducing the amount of data that is displayed.`
- Sorting can be performed with SQL, but not in spreadsheets.
- `Data professionals sort data to make it easier to understand, analyze, and visualize.`
- `Filtering involves showing data that meets a specified criteria while hiding the rest.`
- `Sorting can be used to group similar data together by a classification.`

## Question 5:Fill in the blank: During an analysis project, _____ might involve creating new columns in order to prepare the dataset for analysis

- transforming data
- `formatting and adjusting data`
- organizing data
- getting input from others

## Question 5.1: Fill in the blank: During an analysis project, _____ might involve merging or splitting datasets in order to prepare them for analysis

- `formatting and adjusting data`
- organizing data
- getting input from others
- transforming data

## Question 6:Which query will return a list of all construction businesses that have made more than $8 million, in order from the largest number of employees to the fewest?

    ```sql
    SELECT *
    FROM 'Company_data'
    WHERE Business = 'Construction'
    WHERE Revenue < 8000000
    ORDER BY number_of_employees DESC
    ```

    ```sql
    SELECT *
    FROM 'Company_data'
    WHERE Business = 'Construction', Revenue < 8000000
    ORDER BY number_of_employees ASC
    ```

    ```sql
    SELECT *
    FROM 'Company_data'
    WHERE Business = 'Construction'
    AND Revenue > 8000000
    ORDER BY number_of_employees ASC
    ```

    ```sql
    SELECT *
    FROM 'Company_data'
    WHERE Business = 'Construction'
    AND Revenue > 8000000
    ORDER BY number_of_employees DESC
    -- correct
    ```

## Question 7:A data professional at a manufacturing company is tasked with identifying which machines are most likely to need repairs. In the analyze phase of the data analysis process, what activities might this involve? Select all that apply

- `Format the data to filter for machines that need the most maintenance`
- `Organize a dataset by machine type and performance levels`
- `Get input from colleagues on the data team`
- Prepare a report for the stakeholders

## Question 7.1: A data professional in customer service is tasked with identifying customers who are at risk for taking their business to a competitor. In the analyze phase of the data analysis process, what activities might this involve? Select all that apply

- `Format the data to filter for low customer satisfaction scores`
- `Organize a dataset by customer and purchase history`
- Prepare a report for the stakeholders
- `Request input from other customer service data professionals`

## Question 8:Which function sorts a spreadsheet range between cells C1 and D70 in ascending order by the first column, Column C?

- =SORT(C1:D70, 1, FALSE)
- =SORT(C1:D70, A, TRUE)
- =SORT(C1:D70, A, FALSE)
- `=SORT(C1:D70, 1, TRUE)`
