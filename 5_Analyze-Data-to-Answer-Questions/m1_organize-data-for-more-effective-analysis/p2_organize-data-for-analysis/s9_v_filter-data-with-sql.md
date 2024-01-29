# Filter data with SQL

- Hey, great to see you again.
- Earlier we talked about why you should organize your data, no matter what part of the lifecycle it's in.
- Just like any collection, it's easier to manage and care for a group of things when there's structure around them.
Play video starting at ::15 and follow transcript0:15
Now we should keep in mind that organization isn't just about making things look orderly.
- It's also about making it easier to search and locate the data you need in a quick and easy way.
- As a data analyst, you'll find yourself rearranging and sifting through databases pretty often.
- Two of the most common ways of doing this are with sorting and filtering.
- We've briefly discussed sorting and filtering before, and it's important you know exactly what each one does.
- Sorting is when you arrange data into a meaningful order to make it easier to understand, analyze, and visualize.
- Sorting ranks your data based on a specific metric that you can choose.
- You can sort data in spreadsheets and databases that use SQL.
- We'll get to all the cool functions you can use in both a little later on.
- A common way to sort items when you're shopping on a website is from lowest to highest price, but you can also sort by alphabetical order, like books in a library.
- Or you can sort from newest to oldest, like the order of text messages in a phone.
- Or nearest to furthest away, like when you're searching for restaurants online.
- Another way to organize information is with a filter.
- Filtering is showing only the data that meets a specific criteria while hiding the rest.
- Typically you can use filters when you want to narrow down the amount of data you want to sift through.
- Say you're searching for green sneakers online.
- To save time, you filter for green shoes only.
- Using a filter slims down larger data sets to smaller subsets that are relevant to what you need.
- Sorting and filtering are two actions you probably perform a lot online.
- Whether you're sorting movie showtimes from earliest to latest, or filtering your search results to just images, you're probably already familiar with how helpful they can be for making sense of data.
- Now let's take that knowledge and apply it.
- When it comes to sifting through large, disorganized piles of data, filters are your friend.
- You might remember from a previous video that you can use filters and spreadsheet programs, like Excel and Sheets, to only display data from rows that match the range or condition you've set.
- You can also filter data in SQL using the WHERE clause.
- The WHERE clause works similarly to filtering in a spreadsheet because it returns rows based on a condition you name.
- Let's learn how you can use a WHERE clause in a database.
- We'll use BigQuery to access the database and run our query.
- If you're joining us, open up your tool of choice for using SQL and reference the earlier resource on how to access the dataset.
- Otherwise, watch as the WHERE clause does its thing.
- Here's the database.
Play video starting at :3:5 and follow transcript3:05
You might recognize it from past videos.
- Basically, it's a long list of movies.
- Each row includes an entry for the columns named Movie_Title, Release_Date, Genre, Director, Cast_Members, Budget, and Total_Revenue.
- It also includes a link to the film's Wikipedia page.
- If you scroll down the list, the list goes on for a long time.
- Of course, we won't need to go through everything to find the data we want.
- That's the beauty of a filter! In this case, we'll use the WHERE clause to filter the database and narrow down the list to movies in the comedy genre.
- To start, we'll use the SELECT command followed by an asterisk.
- In SQL, an asterisk selects all of the data.
- On a new line, we'll type FROM and the name of the database: movie_data.movies.
- To filter the movies by comedy, we're going to type WHERE, then list the condition, which is Genre.
Play video starting at :4:5 and follow transcript4:05
Genre is a column in the dataset, and we only want to select rows where the cell in the Genre column exactly matches "Comedy." Next we'll type the equals sign and write the specific genre we're filtering for, which is comedy.
- Since the data in the Genre column is a string format, we have to use single or double quotations when writing it.
- And keep in mind that capitalization matters here, so we have to make sure that the letter casing matches the column name exactly.
- And now we can click Run to check out the results.
- What we're left with is a shorter list of comedy movies.
- Pretty cool, right? Here's something else you should know.
- You can apply multiple filters to a database.
- You can even sort and filter data at the same time for even more precise results.
- As a data analyst, knowing how to sort and filter data will make you a superstar.
- That's all for now.
- Coming up, we'll get down to the nitty-gritty of sorting functions in spreadsheets.
- See you there!

## Key Takeaways

- **Efficient Data Exploration**: Sorting and filtering are crucial for efficiently exploring and analyzing large datasets.
- **SQL WHERE Clause**: The WHERE clause in SQL serves as a powerful tool for filtering data based on specified conditions.
- **Syntax Importance**: Attention to syntax details, including quotation marks and capitalization, is critical for accurate filtering in SQL.
- **Data Analyst's Superpower**: Proficiency in sorting and filtering data is a key skill that can elevate a data analyst's capabilities.
