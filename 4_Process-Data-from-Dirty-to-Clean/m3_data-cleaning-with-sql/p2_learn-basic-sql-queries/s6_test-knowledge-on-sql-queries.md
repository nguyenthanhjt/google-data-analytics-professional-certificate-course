# Test your knowledge on SQL queries

## Question 1:What are some key benefits of using SQL for data analytics projects? Select all that apply

- `Powerful data cleaning tools`
- `Manage huge amounts of data`
- `Adaptable for multiple database programs`
- Insertable images and text formatting

> SQL can handle huge amounts of data, can be adapted and used for multiple database programs, and offers powerful tools for cleaning data. 

## Question 2:Which SQL function cleans string variables by extracting a substring from a string variable?

- `SUBSTR`
- LENGTH
- LEN
- COUNTIF

> `SUBSTR` cleans string variables by extracting a substring from a string variable.

## Question 3:You are working with a database table that contains data about playlists, and you discover there are duplicate entries. What SQL clause will remove the duplicates from the playlist_id column?

- SELECT REMOVE playlist_id
- `SELECT DISTINCT playlist_id`
- SELECT ONLY playlist_id
- SELECT DUPLICATE playlist_id

> To remove duplicates from the **playlist_id** column, use the clause: `DISTINCT` playlist_id. `DISTINCT` is a keyword that is added to a SQL `SELECT` statement to retrieve only non-duplicate entries.

## Question 4:You are working with a database table that contains data about turtles. What SQL clause will return any turtle ages that are less than three digits long from the turtle_age column?

- `LENGTH(turtle_age) < 3`
- LENGTH(turtle_age) > 3
- LENGTH turtle_age < 3
- LENGTH turtle_age > 3

> To return any turtle ages that are less than three digits long from the turtle_age column, use the clause: `LENGTH(turtle_age) < 3`. `LENGTH` returns the length of a text string by counting the number of characters or digits it contains.

## Question 5:You are working with a database table that contains data about cookbooks. What SQL clause will retrieve the first eight letters of each data point in the recipe_name column, then store the result in a new column called recipe_listing?

- `SUBSTR(recipe_name, 1, 8) AS recipe_listing`
- SUBSTR(recipe_name, 1, 8) new_recipe_listing
- SUBSTR(recipe_name, 8) AS recipe_listing
- SUBSTR(recipe_name, 8) to recipe_listing

> To retrieve the first eight letters of each data point in the recipe_name column, then store the result in a new column called recipe_listing, use the clause: `SUBSTR(recipe_name, 1, 8) AS recipe_listing`. `SUBSTR` extracts a substring from a string variable, and AS assigns the new column for the extracted substring.
