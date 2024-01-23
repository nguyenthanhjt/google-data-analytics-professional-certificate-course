# Test your knowledge on cleaning data in spreadsheets

## Question 1:What is the relationship between a text string and a substring?

- A text string is a column of data within a table. A substring is one cell within that column.
- A text string is a row of data within a table. A substring is one cell within that row.
- `A text string is a group of characters within a cell. A substring is a smaller subset of that text string.`
- A text string is the list of attributes at the top of columns within a table. A substring is a single attribute within that list.

> A text string is a group of characters within a cell. A substring is a smaller subset of that text string.

## Question 2:A data analyst uses the COUNTIF function to count the number of times a value less than 50 occurs between spreadsheet cells D2 through F100. What is the correct syntax?

- =COUNTIF(D2:F100,">50")
- =COUNTIF(D2:F100,>50)
- `=COUNTIF(D2:F100,"<50")`
- =COUNTIF(D2:F100,<50)

> The correct syntax is `=COUNTIF(D2:F100,"<50")`. `COUNTIF` will return the number of cells that match a value. **D2:F100** is the range. And **“<50”** is the specified value.

## Question 3:Fill in the blank: To remove leading, trailing, and repeated spaces in data, analysts use the ____ function

- RIGHT
- LEFT
- `TRIM`
- MID

> `TRIM` is a function that removes leading, trailing, and repeated spaces in data.

## Question 4:Which spreadsheet tool searches for matches to a specified value in one column, returning a corresponding piece of information from another location?

- LEN
- SPLIT
- `VLOOKUP`
- CONCATENATE

> `VLOOKUP` searches for matches to a specified value in one column, returning a corresponding piece of information from another location.
