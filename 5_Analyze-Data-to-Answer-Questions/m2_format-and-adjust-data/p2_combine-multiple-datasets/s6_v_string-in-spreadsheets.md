# Video: Strings in spreadsheets

- Hey, welcome back.
- So far we've worked with strings in both SQL and spreadsheets before, and we've learned that they usually have similar functions.
- In this video, we'll take another look at LEN, LEFT, RIGHT and FIND.
- You've come across these functions used in SQL, but now you'll find out how they work in spreadsheets.
- Going back to our bike sharing dataset, let's check out one of their spreadsheets.
- This is one of the Trip Data spreadsheets.
- In the starttime and stoptime columns, there are strings that contain information about date and time of each ride.
- This is all useful data, but chances are we'll only need part of the strings to make a formula or answer a question.
- For example, these strings contain multiple data points, like date and time.
- But if we're trying to find the average time between start times, we won't need the date.
- We can actually use LEN, LEFT and RIGHT, and FIND to split the timestamps into separate columns if we want.
- Let's build a simple formula to separate the dates in these strings.
- We know that LEN tells us the length of a string.
- Let's check how long these datetime strings are now.
- To start, we'll input the first part of the formula.
- And then we'll just select one of the cells with the datetime string in it.
- These strings are 19 characters long.
- We can use the FIND function to locate specific characters in a string.
- Keep in mind, this is case-sensitive.
- So if you're using FIND to pull a substring, make sure that you've input the substring correctly.
- We notice that all of the datetime strings have a space separating the date and the timestamp.
- So we can actually use FIND to figure out where the date ends.
- Okay, seems like the space is the 11th character in this string.
- So the timestamp substring will start at character 12.
- We can use the LEFT and RIGHT functions to select which parts of the string we want to isolate in a new column.
- We'll use RIGHT on one of these cells to indicate that we want to grab the right side.
- And like we've come across before, LEFT actually works exactly the same way.
- Now we can apply that to the rest of column C to pull those timestamps.
- As a data analyst, being able to work with strings is a key skill, especially when you find yourself working with data from outside sources.
- Hopefully you're a little bit more comfortable applying LEN, RIGHT, LEFT and FIND functions in both SQL and spreadsheets.
- Later on, we'll use these functions to perform even more complicated formulas, so feel free to try them out on some data yourself, maybe even some open data like we've been using today.
- See you later.

## Question

In a spreadsheet, cell J10 contains the date and time value 2/23/2021 7:00. What is the correct syntax to return only the four-digit time portion of the cell value?

- `=RIGHT(J10, 4)`
- =LEFT(J10, 4)
- =LEFT(4.J10)
- =RIGHT(4,J10)

> To return only the time portion of the cell value, the syntax is =RIGHT(J10, 4). The time, 7:00, is located four characters from the right of the string.
