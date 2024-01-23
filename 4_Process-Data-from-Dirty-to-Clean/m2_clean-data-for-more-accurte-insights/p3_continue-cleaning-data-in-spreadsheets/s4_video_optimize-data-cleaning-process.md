# Optimize the data-cleaning process

VIDEO Transcript

- Welcome back.
- You've learned about some very useful data- cleaning tools that are built `RIGHT` into spreadsheet applications.
- Now we'll explore how functions can optimize your efforts to ensure data integrity.
- As a reminder, a function is a set of instructions that performs a specific calculation using the data in a spreadsheet.
- The first function we'll discuss is called `COUNTIF`.
- `COUNTIF` is a function that returns the number of cells that match a specified value.
- Basically, it counts the number of times a value appears in a range of cells.
- Let's go back to our professional association spreadsheet.
- In this example, we want to make sure the association membership prices are listed accurately.
- We'll use `COUNTIF` to check for some common problems, like negative numbers or a value that's much less or much greater than expected.
- To start, let's find the least expensive membership: $100 for student associates.
- That'll be the lowest number that exists in this column.
- If any cell has a value that's less than 100, `COUNTIF` will alert us.
- We'll add a few more rows at the bottom of our spreadsheet,
then beneath column H, type "member dueS less than $100." Next, type the function in the cell next to it.
- Every function has a certain syntax that needs to be followed for it to work.
- Syntax is a predetermined structure that includes all required information and its proper placement.
- The syntax of a `COUNTIF` function should be like this: Equals `COUNTIF`, open parenthesis, range, comma, the specified value in quotation marks and a closed parenthesis.
- It will show up like this.
Where I2 through I72 is the range, and the value is less than 100.
- This tells the function to go through column I, and return a count of all cells that contain a number less than 100.
- Turns out there is one! Scrolling through our data, we find that one piece of data was mistakenly keyed in as a negative number.
- Let's fix that now.
- Now we'll use `COUNTIF` to search for any values that are more than we would expect.
- The most expensive membership type is $500 for corporate members.
- Type the function in the cell.
This time it will appear like this: I2 through I72 is still the range, but the value is greater than 500.
There's one here too.
- This entry has an extra zero.
- It should be $100.
The next function we'll discuss is called `LEN`.
- `LEN` is a function that tells you the `LEN`gth of the text string by counting the number of characters it contains.
- This is useful when cleaning data if you have a certain piece of information in your spreadsheet that you know must contain a certain `LEN`gth.
- For example, this association uses six-digit member identification codes.
- If we'd just imported this data and wanted to be sure our codes are all the correct number of digits, we'd use `LEN`.
- The syntax of `LEN` is equals `LEN`, open parenthesis, the range, and the close parenthesis.
- We'll insert a new column after Member ID.
Then type an equals sign and `LEN`.
- Add an open parenthesis.
- The range is the first Member ID number in A2.
- Finish the function by closing the parenthesis.
- It tells us that there are six characters in cell A2.
- Let's continue the function through the entire column and find out if any results are not six.
- But instead of manually going through our spreadsheet to search for these instances, we'll use conditional formatting.
- We talked about conditional formatting earlier.
- It's a spreadsheet tool that changes how cells appear when values meet specific conditions.
- Let's practice that now.
- Select all of column B except for the header.
- Then go to Format and choose Conditional formatting.
- The format rule is to format cells if not equal to six.
Click "Done." The cell with the seven inside is highlighted.
Now we're going to talk about `LEFT` and `RIGHT`.
- `LEFT` is a function that gives you a set number of characters from the `LEFT` side of a text string.
- `RIGHT` is a function that gives you a set number of characters from the `RIGHT` side of a text string.
- As a quick reminder, a text string is a group of characters within a cell, commonly composed of letters, numbers, or both.
- To see these functions in action, let's go back to the spreadsheet from the cosmetics maker from earlier.
- This spreadsheet contains product codes.
- Each has a five-digit numeric code and then a four-character text identifier.
But let's say we only want to work with one side or the other.
- You can use `LEFT` or `RIGHT` to give you the specific set of characters or numbers you need.
- We'll practice cleaning up our data using the `LEFT` function first.
- The syntax of `LEFT` is equals `LEFT`, open parenthesis, the range, a comma, and a number of characters from the `LEFT` side of the text string we want.
- Then, we finish it with a closed parenthesis.
- Here, our project requires just the five-digit numeric codes.
- In a separate column, type equals `LEFT`, open parenthesis, then the range.
- Our range is A2.
- Then, add a comma, and then number 5 for our five- digit product code.
- Finally, finish the function with a closed parenthesis.
- Our function should show up like this.
- Press "Enter." And now, we have a substring, which is the number part of the product code only.
- Click and drag this function through the entire column to separate out the rest of the product codes by number only.
Now, let's say our project only needs the four-character text identifier.
For that, we'll use the `RIGHT` function, and the next column will begin the function.
- The syntax is equals `RIGHT`, open parenthesis, the range, a comma and the number of characters we want.
- Then, we finish with a closed parenthesis.
- Let's key that in now.
- Equals `RIGHT`, open parenthesis, and the range is still A2.
- Add a comma.
- This time, we'll tell it that we want the first four characters from the `RIGHT`.
- Close up the parenthesis and press "Enter." Then, drag the function throughout the entire column.
Now, we can analyze the product in our spreadsheet based on either substring.
- The five-digit numeric code or the four character text identifier.
- Hopefully, that makes it clear how you can use `LEFT` and `RIGHT` to extract substrings from the `LEFT` and `RIGHT` sides of a string.
- Now, let's learn how you can extract something in between.
- Here's where we'll use something called `MID`.
- `MID` is a function that gives you a segment from the `MID`dle of a text string.
- This cosmetics company lists all of its clients using a client code.
- It's composed of the first three letters of the city where the client is located, its state abbreviation, and then a three- digit identifier.
- But let's say a data analyst needs to work with just the states in the `MID`dle.
- The syntax for `MID` is equals `MID`, open parenthesis, the range, then a comma.
- When using `MID`, you always need to supply a reference point.
- In other words, you need to set where the function should start.
- After that, place another comma, and how many `MID`dle characters you want.
- In this case, our range is D2.
- Let's start the function in a new column.
Type equals `MID`, open parenthesis, D2.
- Then the first three characters represent a city name, so that means the starting point is the fourth.
- Add a comma and four.
- We also need to tell the function how many `MID`dle characters we want.
- Add one more comma, and two, because the state abbreviations are two characters long.
- Press "Enter" and bam, we just get the state abbreviation.
- Continue the `MID` function through the rest of the column.
We've learned about a few functions that help separate out specific text strings.
- But what if we want to combine them instead? For that, we'll use `CONCATENATE`, which is a function that joins together two or more text strings.
- The syntax is equals `CONCATENATE`, then an open parenthesis inside indicates each text string you want to join, separated by commas.
- Then finish the function with a closed parenthesis.
- Just for practice, let's say we needed to rejoin the `LEFT` and `RIGHT` text strings back into complete product codes.
- In a new column, let's begin our function.
Type equals `CONCATENATE`, then an open parenthesis.
- The first text string we want to join is in H2.
- Then add a comma.
- The second part is in I2.
- Add a closed parenthesis and press "Enter".
- Drag it down through the entire column,
Play video starting at
and just like that, all of our product codes are back together.
The last function we'll learn about here is `TRIM`.
- `TRIM` is a function that removes leading, trailing, and repeated spaces in data.
- Sometimes when you import data, your cells have extra spaces, which can get in the way of your analysis.
For example, if this cosmetics maker wanted to look up a specific client name, it won't show up in the search if it has extra spaces.
- You can use `TRIM` to fix that problem.
- The syntax for `TRIM` is equals `TRIM`, open parenthesis, your range, and closed parenthesis.
- In a separate column,
Play video starting at
type equals `TRIM` and an open parenthesis.
- The range is C2, as you want to check out the client names.
- Close the parenthesis and press "Enter".
- Finally, continue the function down the column.
`TRIM` fixed the extra spaces.
Now we know some very useful functions that can make your data cleaning even more successful.
- This was a lot of information.
- As always, feel free to go back and review the video and then practice on your own.
- We'll continue building on these tools soon, and you'll also have a chance to practice.
- Pretty soon, these data cleaning steps will become second nature, like brushing your teeth.

## Keypoints

- COUNTIF Function:
  - COUNTIF returns the number of cells within a range that match a specified value.
  - Example: Using COUNTIF to find members with dues less than $100 and those with dues - higher than $500.
- LEN Function:
  - LEN returns the length of a specified piece of information in a cell.
  - Example: Using LEN to determine the length of Member IDs in the dataset.
- Conditional Formatting:
  - Changes cell appearance based on specific conditions.
  - Example: Highlighting cells in column B where the length is not equal to 6.
- LEFT and RIGHT Functions:
  - LEFT returns a set number of characters from the left side of a text string.
  - RIGHT returns a set number of characters from the right side of a text string.
  - Example: Using LEFT to extract the first five characters and RIGHT to extract the - last four characters.
- MID Function:
  - MID returns a segment from the middle of a text string.
  - Example: Extracting a two-letter state code from the middle of a cell in the dataset.
- CONCATENATE Function:
  - CONCATENATE joins together two or more text strings.
  - Example: Combining values from columns H and I.
- TRIM Function:
  - TRIM removes leading, trailing, and repeated spaces in data.
  - Example: Using TRIM to clean and standardize data in a specific column.