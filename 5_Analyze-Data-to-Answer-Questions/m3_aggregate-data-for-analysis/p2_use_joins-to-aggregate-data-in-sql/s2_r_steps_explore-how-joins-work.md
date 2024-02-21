# Step-by-Step: Explore how JOINs work

This reading provides you with the steps the instructor performs in the following video, [Explore how JOINs work](./s3_v_explore-how-joins-work.md). The video teaches you how to use JOIN in SQL to aggregate data in databases.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference tool if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video.

## What you’ll need

In order to follow along with the instructor, you will need the employee dataset uploaded into your project space. If you haven’t already uploaded this data, follow the instructions in the [Upload the employee dataset to BigQuery](./s1_r_upload-employee-dataset-to-bigquery.md) reading.

## Common JOINs

This video explores exactly how JOINs work. A JOIN is a SQL clause that is used to combine rows from two or more tables based on a related column. The instructor discusses the different types of JOINs in more detail in the video; here’s a quick reference you can review as you follow along:

- INNER JOIN: a function that returns records with matching values in both tables
- LEFT JOIN: a function that returns all the records from the left table (first mentioned) and only the matching records from the right table (second mentioned)
- RIGHT JOIN: a function that returns all records from the right table (second mentioned) and only the matching records from the left table (first mentioned).
- OUTER JOIN: a function that combines the RIGHT JOIN and LEFT JOIN to return all matching records in both tables.

## Example 1: INNER JOIN

In the video, the instructor uses BigQuery to join the employees and departments tables. The following steps take you through typing the query into the query window. If you prefer, you can copy and paste the following query into the query window instead.

In BigQuery, select the COMPOSE A NEW QUERY button. BigQuery opens a query window where you can enter your query. The instructor has already executed some queries so their starting line number may be different from yours. If you’ve just opened BigQuery, your line number will be 1. It’s okay if your line numbers aren’t the same as what’s in the video.

1. In line 1 of the query window, enter SELECT and then press Enter.
2. Press Tab and then in line 2 enter employees.name AS employee_name, then press Enter.
3. In line 3, enter employees.role AS employee_role, then press Enter.
4. In line 4, enter departments.name AS department_name, then press Enter.
5. In line 5, press Backspace to stop indenting, enter FROM, then press Enter.
6. In line 6, press Tab, then enter employee_data.employees. Press Enter.
7. In line 7, press Backspace to stop indenting, enter INNER JOIN, then press Enter.
8. In line 8, press Tab, enter employee_data.departments ON, then press Enter.
9. In line 9, enter employees.deparment_id = departments.department_id.
10. Run the query by selecting the Run button.

```sql
SELECT
 employees.name AS employee_name,
 employees.role AS employee_role,
 departments.name AS department_name
FROM
 employee_data.employees
INNER JOIN
 employee_data.departments ON
 employees.department_id = departments.department_id
```

## Example 2: LEFT JOIN

You start a new query in BigQuery either by deleting your previous query in the current query window or by opening a new query window. To open a new query window, select the + button.

A screenshot of the right pane in BigQuery with the Compose new query button highlighted
Now, add a new query that uses LEFT JOIN. If you prefer, you can copy and paste this query into the query window in BigQuery.

1. In line 1, enter SELECT and then press Enter.
2. In line 2, press Tab to indent the row, enter employees.name AS employee_name, then press Enter.
3. In line 3, enter employees.role AS employee_role, then press Enter.
4. In line 4, enter departments.name AS department_name, then press Enter.
5. In line 5, press Backspace to stop indenting, enter FROM, then press Enter.
6. In line 6, press Tab,  then enter employee_data.employees, then press Enter.
7. In line 7, press Backspace to stop indenting, enter LEFT JOIN, then press Enter.
8. In line 8, press Tab, enter employee_data.departments ON, then press Enter.
9. In line 9, enter employees.deparment_id = departments.department_id.
10. Run the query by selecting the Run button.

```sql
SELECT
 employees.name AS employee_name,
 employees.role AS employee_role,
 departments.name AS department_name
FROM
 employee_data.employees
LEFT JOIN
 employee_data.departments ON
 employees.department_id = departments.department_id
```

## Example 3: RIGHT JOIN

Use the following steps to write a RIGHT JOIN query. If you prefer, you can copy and paste the query below into the query window.

Delete the previous query or open a new query window.

1. In line 1, enter SELECT and then press Enter.
2. In line 2, press Tab to indent the row, enter employees.name AS employee_name, then press Enter.
3. In line 3, enter employees.role AS employee_role, then press Enter.
4. In line 4, enter departments.name AS department_name, then press Enter.
5. In line 5, press Backspace to stop indenting, enter FROM, then press Enter.
6. In line 6, press Tab,  then enter employee_data.employees, then press Enter.
7. In line 7, press Backspace to stop indenting, enter RIGHT JOIN, then press Enter.
8. In line 8, press Tab, enter employee_data.departments ON, then press Enter.
9. In line 9, enter employees.deparment_id = departments.department_id.
10. Run the query by selecting the Run button.

```sql
SELECT
 employees.name AS employee_name,
 employees.role AS employee_role,
 departments.name AS department_name
FROM
 employee_data.employees
RIGHT JOIN
 employee_data.departments ON
 employees.department_id = departments.department_id
```

## Example 4: OUTER JOIN

Use the following steps to write an OUTER JOIN query. If you prefer, you can copy and paste the query below into the query window.

1. Delete the previous query or open a new query window.
2. In line 1, enter SELECT and then press Enter.
3. In line 2, press Tab to indent the row, enter employees.name AS employee_name, then press Enter.
4. In line 3, enter employees.role AS employee_role, then press Enter.
5. In line 4, enter departments.name AS department_name, then press Enter.
6. In line 5, press Backspace to stop indenting, enter FROM, then press Enter.
7. In line 6, press Tab,  then enter employee_data.employees, then press Enter.
8. In line 7, press Backspace to stop indenting, enter FULL OUTER JOIN, then press Enter.
9. In line 8, press Tab, enter employee_data.departments ON, then press Enter.
10. In line 9, enter employees.deparment_id = departments.department_id.
11. Run the query by selecting the Run button.

```sql
SELECT
 employees.name AS employee_name,
 employees.role AS employee_role,
 departments.name AS department_name
FROM
 employee_data.employees
FULL OUTER JOIN
 employee_data.departments ON
 employees.department_id = departments.department_id
```
