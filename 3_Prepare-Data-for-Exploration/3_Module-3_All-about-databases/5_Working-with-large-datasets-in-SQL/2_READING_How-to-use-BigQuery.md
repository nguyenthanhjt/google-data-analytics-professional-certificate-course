# Using BigQuery

[BigQuery](https://cloud.google.com/bigquery/docs) is a data warehouse on Google Cloud that data analysts can use to query, filter large datasets, aggregate results, and perform complex operations.

An upcoming activity is performed in BigQuery. This reading provides instructions to create your own BigQuery account, select public datasets, and upload CSV files. At the end of this reading, you can confirm your access to the BigQuery console before you move on to the activity,

**Note**: Additional getting started resources for a few other SQL database platforms are also provided at the end of this reading if you choose to work with them instead of BigQuery.

## Types of BigQuery accounts

There are two different types of accounts: sandbox and free trial. A sandbox account allows you to practice queries and explore public datasets for free, but has additional [restrictions](https://cloud.google.com/bigquery/docs/sandbox#limits) on top of the [standard quotas and limits](https://cloud.google.com/bigquery/quotas). If you prefer to use BigQuery with the standard limits, you can set up a free trial account instead. More details:

- A free sandbox account doesn’t ask for a method of payment. It does, however, limit you to 12 projects. It also doesn't allow you to insert new records to a database or update the field values of existing records. These data manipulation language (DML) operations aren't supported in the sandbox.
- A free trial account requires a method of payment to establish a billable account, but offers full functionality during the trial period.

With either type of account, you can upgrade to a paid account at any time and retain all of your existing projects. If you set up a free trial account but choose not to upgrade to a paid account when your trial period ends, you can still set up a free sandbox account at that time. However, projects from your trial account won't transfer to your sandbox account. It would be like starting from scratch again.

Set up a free sandbox account for use in this program
Follow these [step-by-step instructions](https://cursive.io/shared/2da0e63f3-9de7-476f-997b-93fff70d7cb6) or watch the video, [Setting up BigQuery, including sandbox and billing options](https://www.coursera.org/learn/data-preparation/lecture/YCkys/setting-up-bigquery-including-sandbox-and-billing-options).

For more detailed information about using the sandbox, start with the documentation, [Using the BigQuery sandbox](https://cloud.google.com/bigquery/docs/sandbox?hl=en_US).

After you set up your account, you will see the project name you created for the account in the banner and **SANDBOX** at the top of your BigQuery console.

## Set up a free trial account instead (if you prefer)

If you prefer not to have the sandbox limitations in BigQuery, you can set up a free trial account for use in this program.

- Follow these [step-by-step instructions](https://cursive.io/shared/2e98bf922-42d6-48c2-998f-6057389d0ccb) or watch the video, [Setting up BigQuery, including sandbox and billing options](https://cursive.io/shared/2e98bf922-42d6-48c2-998f-6057389d0ccb). The free trial offers $300 in credit over the next 90 days. You won’t get anywhere near that spending limit if you just use the BigQuery console to practice SQL queries. After you spend the $300 credit (or after 90 days) your free trial will expire and you will need to personally select to upgrade to a paid account to keep using Google Cloud Platform services, including BigQuery. Your method of payment will never be automatically charged after your free trial ends. If you select to upgrade your account, you will begin to be billed for charges. 
- After you set up your account, you will see My First Project in the banner and the status of your account above the banner – your credit balance and the number of days remaining in your trial period.

## How to get to the BigQuery console

In your browser, go to [console.cloud.google.com/bigquery](console.cloud.google.com/bigquery).

Note: Going to [console.cloud.google.com](https://console.cloud.google.com/) in your browser takes you to the main dashboard for the Google Cloud Platform. To navigate to BigQuery from the dashboard, do the following:

Click the Navigation menu icon (Hamburger icon) in the banner.

Scroll down to the BIG DATA section.

Click BigQuery and select SQL workspace.

Watch the [How to use BigQuery](https://www.coursera.org/learn/data-preparation/lecture/YWn81/how-to-use-bigquery) video for an introduction to each part of the BigQuery SQL workspace.

## (Optional) Explore a BigQuery public dataset

You will be exploring a public dataset in an upcoming activity, so you can perform these steps later if you prefer.

Refer to these [step-by-step instructions](https://cursive.io/shared/242bde9a6-5415-4ce0-bbae-7e875d14d927).

## (Optional) Upload a CSV file to BigQuery

These steps are provided so you can work with a dataset on your own at this time. You will upload CSV files to BigQuery later in the program.

Refer to these [step-by-step instructions](https://cursive.io/shared/2dea0d610-ef6b-4ba8-8e44-d40dfeb0454b).

## Getting started with other databases (if not using BigQuery)

It is easier to follow along with the course activities if you use BigQuery, but if you are connecting to and practicing SQL queries on other database platforms instead of BigQuery, here are similar getting started resources:

- [Getting started with MySQL](https://dev.mysql.com/doc/mysql-getting-started/en/): This is a guide to setting up and using MySQL.
- [Getting started with Microsoft SQL Server](https://docs.microsoft.com/en-us/sql/relational-databases/tutorial-getting-started-with-the-database-engine?view=sql-server-ver15): This is a tutorial to get started using SQL Server.
- [Getting started with PostgreSQL](https://www.postgresql.org/docs/10/tutorial-start.html): This is a tutorial to get started using PostgreSQL.
- [Getting started with SQLite](https://www.sqlite.org/quickstart.html): This is a quick start guide for using SQLite.
