# Test your knowledge on VLOOKUP

## Question 1:Fill in the blank: The purpose of _____ is to gather data from multiple sources in order to combine it into a single, summarized collection

- data collection
- `data aggregation`
- data transfer
- data blending

> The purpose of data aggregation is to gather data from multiple sources in order to combine it into a single, summarized collection.

## Question 2:Which function can be used to change a text string in spreadsheet cell B11 to a numerical value?

- =MATCH(B11)
- =CONVERT(B11)
- `=VALUE(B11)`
- =NUM(B11)

> The function =VALUE(B11) can be used to change the text string in spreadsheet cell B11 to a numerical value.

## Question 3:What is the purpose of the absolute references within the function =AVERAGE($B$2:$B$11)?

- Ensure the rows and columns will not change if the function is copied
- Represent missing values in a formula or function
- Make formulas and functions unconditional
- Remove unnecessary instructions from a formula or function

> The purpose of absolute references is to ensure the rows and columns will not change if the function is copied.

## Question 4: In this spreadsheet, which VLOOKUP function will search for the height of the building in Shenzhen?

|                | A                         | B                | C              | D              |
| -------------- | ------------------------ | ----------------- | -------------- | -------------- |
| 1              | Location                 | Building          | Height         | Year completed |
| 2              | Dubai                    | Burj Khalifa      | 2,717 feet     | 2010           |
| 3              | Shanghai                 | Shanghai Tower    | 2,073 feet     | 2015           |
| 4              | Mecca                    | Makkah Royal Clock Tower | 1,972 feet     | 2012    |
| 5              | Shenzhen                 | Ping An Finance Center   | 1,965 feet     | 2017    |
| 6              | St. Petersburg           | Lakhta Center     | 1,516 feet     | 2019           |
| 7              | Chicago                  | Willis Tower      | 1,451 feet     | 1974           |

- `=VLOOKUP(“Shenzhen”, A2:D7, 3, FALSE)`
- =VLOOKUP(Shenzhen, A2,D7, 3, TRUE)
- =VLOOKUP(Shenzhen, A2:D7, 2, TRUE)
- =VLOOKUP(“Shenzhen” A2-D7, 2, FALSE)

> Correct
To search for the height of the building in Shenzhen, the correct function is =VLOOKUP(“Shenzhen”, A2:D7, 3, false). “Shenzhen” is the reference. A2:D7 is the table array. The 3 indicates the number of the column from which the value should be returned. And the word FALSE instructs the function to return an exact match.
