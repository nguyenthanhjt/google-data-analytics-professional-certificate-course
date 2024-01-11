# *Course 3 challenge*

> This is a timed quiz:Are you sure you are ready to start the quiz? You will be given 50 minutes to complete it. Once you reach the time limit, you will use one attempt.

## Scenario 1, questions 1-5

You’ve been working at a data analytics consulting company for the past six months. Your team helps restaurants use their data to better understand customer preferences and identify opportunities to become more profitable.

To do this, your team analyzes customer feedback to improve restaurant performance. You use data to help restaurants make better staffing decisions and drive customer loyalty. Your analysis can even track the number of times a customer requests a new dish or ingredient in order to revise restaurant menus.

Currently, you’re working with a vegetarian sandwich restaurant called Garden. The owner wants to make food deliveries more efficient and profitable. To accomplish this goal, your team will use delivery data to better understand when orders leave Garden, when they get to the customer, and overall customer satisfaction with the orders.

Before project kickoff, you attend a discovery session with the vice president of customer experience at Garden. He shares information to help your team better understand the business and project objectives. As a follow-up, he sends you an email with datasets.

Click below to read the email:

- The C3 Scenario 1 - Client Email.pdf

    ```pdf
    From: Carlos Soto <carlos_soto@gardenelizabethtownrestaurants.com>
    Date: Fri, 3/27/2021 3:14 PM
    Subject: Discovery session
    To: You <You@gmail.com>
    Team:
    Thank you for the productive discovery session earlier today!
    As discussed, attached are a few data sources that our team collected as we work on
    improving our delivery business. This data includes:
    ● Customer satisfaction survey results
    ● Data on how long each delivery takes compared to distance from Garden
    In addition, you’ll find a file that contains pictures of sandwich deliveries over a period of 30
    days. (We had a campaign that asked customers to photograph their orders, then share them
    on social media. We hope to use these pictures to evaluate quality control and ensure our
    sandwiches arrive in great condition.)
    Please let me know if you need anything else. Otherwise, we look forward to regrouping in a
    few weeks to understand how best to use this information to inform our plan.
    Thanks,
    Carlos
    Carlos Soto
    Vice President of Customer Experience
    Garden Restaurant Group
    Elizabethtown, KY
    ```

- The [Course-3-Final-Challenge-Data-Sets---Delivery-times_distance-1-.csv](./resources/Course-3-Final-Challenge-Data-Sets---Delivery-times_distance-1-.csv)

    ```csv
    Delivery,Driver,Time,Distance from Garden (in miles),Duration of delivery (minutes)
    1,Charles,1:54 PM,1.6,22
    2,Fatima,1:35 PM,12,39
    3,Beatriz,11:01 AM,6.1,38
    4,Eric,11:32 AM,4.4,26
    5,Charles,11:05 AM,6.3,39
    6,Beatriz,1:18 PM,4.9,27
    7,Eric,4:08 PM,0.9,24
    8,Diya,5:34 PM,2.9,28
    9,Fatima,11:43 AM,1.1,30
    10,Diya,9:14 PM,15,29
    11,Charles,1:44 PM,0.8,22
    12,Charles,1:32 PM,4.5,30
    14,Beatriz,8:27 PM,1.8,30
    15,Ali,1:05 PM,0.6,20
    16,Fatima,9:34 PM,1.8,36
    17,Charles,5:39 PM,7.5,21
    18,Diya,5:24 PM,5.3,47
    19,Fatima,2:32 PM,2.5,25
    20,Ali,11:20 AM,2.6,48
    21,Beatriz,1:45 PM,8.4,26
    22,Gabriel,12:09 PM,7.2,49
    23,Ali,1:09 PM,1.5,27
    24,Diya,6:10 PM,0.9,23
    25,Diya,2:17 PM,6.6,28
    26,Ali,7:16 PM,5.6,24
    27,Fatima,1:11 PM,5.2,29
    28,Ali,3:18 PM,13.9,25
    29,Fatima,1:31 PM,5.5,30
    30,Beatriz,11:54 AM,0.7,21
    31,Charles,1:35 PM,8.7,31
    32,Eric,5:42 PM,4.9,42
    33,Fatima,7:43 PM,15,52
    34,Gabriel,4:05 PM,3.6,43
    35,Charles,1:08 PM,5.1,53
    36,Gabriel,5:40 PM,10.3,50
    37,Fatima,1:10 PM,7.1,54
    38,Eric,2:09 PM,6.8,51
    39,Fatima,7:31 PM,4.6,66
    40,Fatima,1:52 PM,8.1,52
    41,Gabriel,9:37 PM,2.4,56
    42,Fatima,6:00 PM,2.1,53
    43,Ali,8:07 PM,7.5,53
    44,Ali,8:22 PM,5,62
    45,Charles,2:18 PM,2.7,54
    46,Charles,3:44 PM,14.6,55
    47,Gabriel,11:16 AM,1.1,26
    48,Fatima,3:58 PM,9.6,56
    49,Charles,8:24 PM,1.9,27
    50,Fatima,5:45 PM,3.4,57
    51,Diya,9:58 PM,4.9,28
    ```

- [Course-3-Final-Challenge-Data-Sets---Customer-survey-data-1-.csv](./resources/Course-3-Final-Challenge-Data-Sets---Customer-survey-data-1-.csv)

    ```csv
    Customer,How satisfied were you with your overall delivery experience at Garden?                    1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,How satisfied were you with the quality of the food at Garden?                             1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,How satisfied were you with the speed of delivery at Gardent?                                1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,Was your order accurate?                                 Please respond yes or no.
    1,5,3,4,Yes
    2,3,4,3,Yes
    3,4,5,2,Yes
    4,5,3,4,Yes
    5,2,5,1,Yes
    6,5,2,5,Yes
    7,1,4,3,Yes
    8,3,3,2,No
    9,5,1,3,Yes
    10,3,5,3,No
    11,5,3,4,Yes
    12,2,2,5,Yes
    13,4,5,3,No
    14,3,4,2,Yes
    15,1,5,1,Yes
    16,5,4,5,Yes
    17,2,2,4,Yes
    18,4,5,4,No
    19,5,1,5,Yes
    20,2,4,4,Yes
    21,5,5,1,Yes
    22,3,3,3,No
    23,1,5,5,Yes
    24,5,4,4,Yes
    25,3,3,2,Yes
    26,2,3,4,Yes
    27,2,2,3,No
    28,4,5,4,Yes
    29,4,1,2,Yes
    30,3,4,5,Yes
    31,5,5,4,Yes
    32,3,3,4,No
    33,1,2,5,Yes
    34,5,5,1,Yes
    35,5,1,2,Yes
    36,2,3,3,Yes
    37,1,5,4,Yes
    38,5,4,3,Yes
    39,2,2,4,No
    40,3,3,2,Yes
    ```

- Reviewing the data enables you to describe how you will use it to achieve your client’s goals. First, you notice that all of the data was collected by Garden employees using their own resources. What type of data does this describe?
  - Third-party data
  - Nominal data
  - `First-party data`
  - Qualitative data

>This describes first-party data, which is collected by an individual or group using their own resources.

- Reviewing the data enables you to describe how you will use it to achieve your client’s goals. First, you notice that all of the data is first-party data, which means that it was collected from outside sources.
  - True
  - `False`

## Question 2: Scenario 1 continued

Next, you review the customer satisfaction survey data. To use the template for the customer satisfaction survey data, click the link below and select “Use Template.”

Link to template: [Customer Satisfaction Survey data](https://docs.google.com/spreadsheets/d/1TIDFXT6FWkINcorBRBfHm4IIq2t_Fk_64A2FZmzZcFQ/template/preview?resourcekey=0-9fNDl5cafZVNOegbveShCA)

OR If you don’t have a Google account, download the CSV file directly from the attachment [customer-survey-data.csv](./resources/customer-survey-data.csv).

- The Customer Satisfaction Survey Data:

```csv
Customer,How satisfied were you with your overall delivery experience at Garden?                    1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,How satisfied were you with the quality of the food at Garden?                             1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,How satisfied were you with the speed of delivery at Gardent?                                1-5 where 1 = extremely dissatisfied and 5 = extremely satisfied,Was your order accurate?                                 Please respond yes or no.
1,5,3,4,Yes
2,3,4,3,Yes
3,4,5,2,Yes
4,5,3,4,Yes
5,2,5,1,Yes
6,5,2,5,Yes
7,1,4,3,Yes
8,3,3,2,No
9,5,1,3,Yes
10,3,5,3,No
11,5,3,4,Yes
12,2,2,5,Yes
13,4,5,3,No
14,3,4,2,Yes
15,1,5,1,Yes
16,5,4,5,Yes
17,2,2,4,Yes
18,4,5,4,No
19,5,1,5,Yes
20,2,4,4,Yes
21,5,5,1,Yes
22,3,3,3,No
23,1,5,5,Yes
24,5,4,4,Yes
25,3,3,2,Yes
26,2,3,4,Yes
27,2,2,3,No
28,4,5,4,Yes
29,4,1,2,Yes
30,3,4,5,Yes
31,5,5,4,Yes
32,3,3,4,No
33,1,2,5,Yes
34,5,5,1,Yes
35,5,1,2,Yes
36,2,3,3,Yes
37,1,5,4,Yes
38,5,4,3,Yes
39,2,2,4,No
40,3,3,2,Yes
```

The question in column E asks, “Was your order accurate? Please respond yes or no.” What kind of data is this?

- `Boolean data`
- Clean data
- Second-party data
- Ordinal data

> This is Boolean data, which has only two possible values, such as yes or no. 

## Question 3:Scenario 1 continued

Now, you review the data on delivery times and the distance of customers from the restaurant.
To use the template for the dataset, click the link below and select “Use Template.”

Link to template: [Delivery Times/Distance](https://docs.google.com/spreadsheets/d/19-8x0-P6TAppfx-GDZGoH-PHp0WtNyCM8QjVKqkGvac/template/preview?resourcekey=0-0qv0-O9ED0KVvM_pLxGK3A)

OR If you don’t have a Google account, download the CSV file directly from the attachment [delivery-times_distance.csv](./resources/delivery-times_distance.csv).

```csv
Delivery,Driver,Time,Distance from Garden (in miles),Duration of delivery (minutes)
1,Charles,1:54 PM,1.6,22
2,Fatima,1:35 PM,12,39
3,Beatriz,11:01 AM,6.1,38
4,Eric,11:32 AM,4.4,26
5,Charles,11:05 AM,6.3,39
6,Beatriz,1:18 PM,4.9,27
7,Eric,4:08 PM,0.9,24
8,Diya,5:34 PM,2.9,28
9,Fatima,11:43 AM,1.1,30
10,Diya,9:14 PM,15,29
11,Charles,1:44 PM,0.8,22
12,Charles,1:32 PM,4.5,30
14,Beatriz,8:27 PM,1.8,30
15,Ali,1:05 PM,0.6,20
16,Fatima,9:34 PM,1.8,36
17,Charles,5:39 PM,7.5,21
18,Diya,5:24 PM,5.3,47
19,Fatima,2:32 PM,2.5,25
20,Ali,11:20 AM,2.6,48
21,Beatriz,1:45 PM,8.4,26
22,Gabriel,12:09 PM,7.2,49
23,Ali,1:09 PM,1.5,27
24,Diya,6:10 PM,0.9,23
25,Diya,2:17 PM,6.6,28
26,Ali,7:16 PM,5.6,24
27,Fatima,1:11 PM,5.2,29
28,Ali,3:18 PM,13.9,25
29,Fatima,1:31 PM,5.5,30
30,Beatriz,11:54 AM,0.7,21
31,Charles,1:35 PM,8.7,31
32,Eric,5:42 PM,4.9,42
33,Fatima,7:43 PM,15,52
34,Gabriel,4:05 PM,3.6,43
35,Charles,1:08 PM,5.1,53
36,Gabriel,5:40 PM,10.3,50
37,Fatima,1:10 PM,7.1,54
38,Eric,2:09 PM,6.8,51
39,Fatima,7:31 PM,4.6,66
40,Fatima,1:52 PM,8.1,52
41,Gabriel,9:37 PM,2.4,56
42,Fatima,6:00 PM,2.1,53
43,Ali,8:07 PM,7.5,53
44,Ali,8:22 PM,5,62
45,Charles,2:18 PM,2.7,54
46,Charles,3:44 PM,14.6,55
47,Gabriel,11:16 AM,1.1,26
48,Fatima,3:58 PM,9.6,56
49,Charles,8:24 PM,1.9,27
50,Fatima,5:45 PM,3.4,57
51,Diya,9:58 PM,4.9,28
```

The data in column E shows the duration of deliveries from Garden to customers. What type of data is this? Select all that apply.

- `Quantitative data`
- Continuous data
- Qualitative data
- `Discrete data`

> This is an example of discrete data, which is counted and has a limited number of values. It is also quantitative data, which is specific and measures numerical facts.

## Question 4:Scenario 1 continued

The next thing you review is the file containing pictures of sandwich deliveries over a period of 30 days. This is an example of structured data.

- True
- `False`

>This is an example of unstructured data, which is not organized in an easily identifiable manner.

## Question 5:Scenario 1 continued

Now that you’re familiar with the data, you want to build trust with the team at Garden. You decide to impress them by taking the initiative to reach out to your social media followers. You explain that Garden is a new client, and you show them the pictures of Garden’s sandwich deliveries from the client file. Then, you ask them if they have any photos of sandwich deliveries that you can evaluate.

This is an example of going above and beyond expectations and a great way to build trust.

- True
- `False`

> Building trust involves not sharing private or sensitive client information

## Question 6:Scenario 2, questions 6-10

You’ve completed this program and are interviewing for a junior data scientist position at a company called Sewati Financial Services.

Click below to review the job description:

- [C3-Course-Challenge-Junior-Data-Scientist-Job-Description-.pdf](./resources/C3-Course-Challenge-Junior-Data-Scientist-Job-Description-.pdf)

    ```pdf

    Junior Data Scientist
    Company: Sewati Financial Services (Macon, GA)

    The Macon, Georgia, analytics team is responsible for providing analysis and insights that address the investment needs of our valued clients.
    The analysis and insights provide actionable recommendations that address market risk and the return-on-investment goals of everyone who
    places their trust in Sewati Financial Services to help them plan for a bright future.

    This position reports to the senior manager of strategy.
    12 hours ago A Full time

    Responsibilities
    - Interpret data, analyze results, and provide ongoing reports
    - Develop, implement, and monitor data collection systems
    - Acquire data from primary and secondary data sources
    - Identify, analyze, and interpret trends or patterns in data sets
    - Maintain databases and data systems
    - Filter and clean data
    - Work with management to prioritize business and information needs
    - Locate and define new process improvement opportunities

    Qualifications
    - Bachelor's degree or equivalent data analytics certification
    - 0-1 year of work experience (strong entry-level candidates will beconsidered)
    - Excellent analytical skills
    - Excellent organization skills
    - Ability to maximize data and use it effectively
    - General understanding of data collection and database design
    - General understanding of spreadsheets
    - General understanding of programming languages, such a SQL and R
    - General understanding of data visualization methods
    - General understanding of how to present findings
    - Ability to assess data to ensure it is objective and free of bias

    Sewati Financial Services is a family-owned business that has been in practice for more than 30 years. We are keenly aware that, when it comes
    to choosing a financial services company, it's essential to work with someone you trust. At Sewati Financial Services, we hold every member of
    our team to the highest standards of integrity and ethics, keeping our clients'best interests at the forefront of everything we do. Most importantly, we help them bring their retirement dreams to life.
    ```

So far, you’ve successfully completed the first interview with a recruiter. They arrange your second interview with the team at Sewati Financial Services.

Click below to read the email from the human resources director:

- [Course-3-Scenario-2_Second-Interview-Email.pdf](./resources/Course-3-Scenario-2_Second-Interview-Email.pdf)

    ```pdf
    From: Harry Sheilds <Harry.Shields@analyticsrecruitment.com>
    Date: Fri, 10/28/2021 7:09 AM
    Subject: Second interview
    To: You <You@Gmail.com>
    Good morning:
    Congratulations on reaching the next phase of the interview process for the junior data
    scientist position! My clients at Sewati Financial Services are impressed with your
    qualifications and look forward to meeting you.
    The interview will take place Wednesday at 3:30 PM. You will meet with Kai Harvey, the senior
    manager of strategy. Please note that this will be a behavioral interview. A behavioral
    interview first involves being presented with some scenarios typically encountered by junior
    data scientists. Then, you’ll be asked to consider how you would respond if faced with these
    situations in real life. Don't worry if you haven't had these experiences in a professional role;
    they’re simply interested in understanding how you would handle these kinds of scenarios.
    To help you prepare, take a look at the following topic areas:
    ● Types of bias found in data (including sampling bias)
    ● Types and use of data
    ● Types and use of metadata
    ● Filtering and sorting in spreadsheets
    ● Basic SQL commands, such as SELECT, FROM, and WHERE
    ● Data privacy
    Again, congratulations, and all the best on Wednesday!
    Best regards,
    Harry
    Harry Shields
    Recruiter
    Analytics Recruitment
    Madison, GA
    ```

You arrive 15 minutes early for your interview. Soon, you are escorted into a conference room, where you meet Kai Harvey, the senior manager of strategy. After welcoming you, he begins the behavioral interview.

Consider and respond to the following question. Select all that apply.

Our data analytics team often surveys clients to get their feedback. If you were on the team, how would you ensure the process does not cause potential bias?

- `Give participants enough time to answer each survey question.`
- `Include clients with disabilities in the survey sample.`
- Instruct participants to share their name and contact information.
- `Make sure the wording of the survey question does not encourage a specific response from participants.`

> Give participants enough time to answer each survey question.

## Question 7:Scenario 2 continued

Consider and respond to the following question. Select all that apply.

Our data analytics team often uses both internal and external data. Describe the difference between the two.

- `Internal data came from a company’s own systems. External data comes from outside the organization.`
- `Internal data is often generated from within the company. External data is generated outside the organization.`
- External data is often generated from within the company. Internal data is generated outside the organization.
- External data came from a company’s own systems. Internal data came from the organization.

> Internal data lives within a company’s own systems and is typically generated from within the company. External data lives in and is generated outside the organization.

## Question 8:Scenario 2 continued

Consider and respond to the following question. Select all that apply.

Our analysts often work within the same spreadsheet, but for different purposes. What tools would you use in such a situation?

- `Freeze the header rows`
- `Sort the data to make it easier to understand, analyze, and visualize`
- `Filter to show only the data that meets a specific criteria`
- Encrypt the spreadsheet so only you can access it

> Sorting, filtering, and freezing header rows enable data analysts on the same team to use the same dataset for different purposes.

## Question 9:Scenario 2 continued

Next, your interviewer wants to better understand your knowledge of basic SQL commands. He asks: How would you write a query that retrieves only data about people who joined our firm in 2019 from the Clients table in our database?

- `SELECT * FROM Clients WHERE start_date = '2019'`
- SELECT * WHERE Clients = '2019'
- SELECT * WHERE start_date = '2019'
- SELECT Clients WHERE start_date = '2019'

> To write a query that retrieves only data about people who joined the firm in 2019 from the Clients table, type SELECT * FROM Clients WHERE start_date=’2019’.

## Question 10:Scenario 2 continued

For your final question, your interviewer explains that Sewati Financial Services needs its clients’ trust, and this is an important responsibility for the data analytics team.

He asks you to identify which data analytics practice involves preserving a data subject’s information and activity any time a data transaction occurs.

- Sharing permissions
- Encryption
- Bias
- `Data privacy`
