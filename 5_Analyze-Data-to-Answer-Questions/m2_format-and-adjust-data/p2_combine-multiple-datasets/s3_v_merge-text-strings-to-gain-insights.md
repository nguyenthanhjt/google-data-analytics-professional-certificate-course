# Merge text strings to gain insights

Video transcript

- Great to see you back.
- In this video, we'll build on what we've learned about CONCATENATE and IMPORTRANGE by exploring a new SQL query: CONCAT.
- You might remember that CONCATENATE is a function that joins together two or more text strings.
- As a quick reminder, a text string is a group of characters within a cell most often composed of letters.
- You've seen how that works within a single spreadsheet.
- But there's a similar function in SQL that allows you to join multiple text strings from multiple sources, CONCAT.
- Let's use CONCAT to combine strings from multiple tables to create new strings.
- For this example, we'll use open data from Citi Bike, which is a public bicycle sharing system in New York.
- As you've learned earlier, open data initiatives have created a ton of data for analysts to use.
- Openness or open data is free access, usage, and sharing of data.
- It's a great resource if you want to practice or experiment with the data analysis tools you've been learning here.
- You have open access to the New York city bike-sharing data, which has information about the use of shared bikes across the city.
- Now we can use CONCAT to pull and concatenate data from different columns stored here.
- The first thing we need to do is figure out which columns we need.
- That way we can tell SQL where the strings we want are.
- For example, the bike-sharing company has two different kinds of customers; one-time paying customers and subscribers.
- Let's say we want to find out what routes are most popular with different user types.
- To do that, we need to create strings of recognizable route names that we can count and sort.
- We know that the information we need is in the stations and trips table.
- We'll start building our query from there.
- First, we'll input SELECT user type to let SQL know that we want the user type as a column.
- Then we'll use CONCAT to combine the names of the beginning and ending stations for each trip in a new column.
- This will create one column based on the routes people take.
- We also need to input a title for this new column.
- We'll type in, AS route, to name the route column using those beginning and ending station names we combined with CONCAT.
- This will make these route names easy for us to read and understand.
- After that, we want SQL to count the number of trips.
- So we'll input COUNT to do that.
- We can use an asterisk to tell it to count up the number of rows in the data we're selecting.
- In this case, each row represents a trip, which is why we can just count all of the rows we've selected.
- We'll name this output as num_trips.
Play video starting at :2:46 and follow transcript2:46
Now let's also get the average trip duration for each route.
- In this case, we don't need the exact average, so we can use the ROUND function to round up.
- We'll put that first and then in the parentheses use average to get the average trip duration.
- We'll also want this data to be in integer form for this calculation, so we'll input cast as int 64.
- Big query stores numbers in a 64-bit memory system, which is why there's a 64 after integer in this case.
- Next, we'll divide it by the number of rows and tell it how far we want it to round, two decimal places.
- We'll name this output as duration.
- We'll need to tell SQL where this information is stored.
- We'll use FROM and the location we're pulling it from.
Play video starting at :3:42 and follow transcript3:42
Since we're using COUNT and AVERAGE functions in our select clause, we have to use GROUP BY to group together summary rows.
- Let's group by the start station, the end station, and the user type for this query.
- Finally, we'll use ORDER BY to tell it how we want to organize this data.
- For this, we want to figure out the most common trips so we can input the number of trips column and use DESC to put it in descending order.
- Finally, we only want the top 10, so let's add LIMIT 10.
- Now thanks to CONCAT, we can easily read these route names and trace them back to real places.
- We can see which kinds of customers are taking which routes, which can help the bike-sharing company understand their user base in different parts of the city and where to keep more bikes for people to rent.
- Being able to combine multiple pieces of data can give you new ways to organize and analyze data.
- There's a lot of different tools to help you do that.
- Now you've seen CONCAT in action, and later you will come across another similar query, JOIN.
- But up next, we'll talk more about working with strings.
- See you soon.

## Notes

The instructor is about to say "divide by the number of rows." This is incorrect. Read the Step-by-Step guide associated with this video for more information.

```sql
SELECT
  usertype,
  CONCAT(start_station_name,' to ', end_station_name) AS route,
  COUNT(*) AS number_trips,
  ROUND(AVG(CAST(tripduration AS INT64)/60), 2) AS duration_minutes
FROM
  `bigquery-public-data.new_york_citibike.citibike_trips`
GROUP BY
  usertype,
  start_station_name,
  end_station_name
ORDER BY
  number_trips DESC
LIMIT
  10
```

## Keypoints

- Introduction to CONCAT in SQL:
  - CONCAT is a SQL function used to join multiple text strings from different sources.
  - It is similar to the CONCATENATE function used in spreadsheets.
- Use Case - Citi Bike Data:
  - The video uses Citi Bike data, a public bicycle-sharing system in New York, as an example.
  - Open data initiatives provide a wealth of data for analysts.
- Building a Query Step-by-Step:
  - The goal is to find the most popular routes for different user types.
  - Columns needed: usertype, concatenated route names, count of trips, and average trip duration.
- Building the Query:
  - SELECT Clause:
    - SELECT usertype
    - CONCAT(start_station_name, " to ", end_station_name) AS route
    - COUNT(*) AS num_trips
    - ROUND(AVG(CAST(tripduration AS INT64)/60), 2) AS duration
  - FROM Clause:
    - FROM bigquery-public-data.new_york.citibike_trips
  - GROUP BY Clause:
    - GROUP BY start_station_name, end_station_name, usertype
  - ORDER BY Clause:
    - ORDER BY num_trips DESC
  - LIMIT Clause:
    - LIMIT 10
- Results and Insights:
  - The query provides insights into the most common routes, user types, and average trip duration.
  - Helps the bike-sharing company understand user preferences in different parts of the city.
