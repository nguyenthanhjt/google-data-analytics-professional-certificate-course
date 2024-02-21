# VLOOKUP in action

Video transcript

- Hi and welcome back.
- In a previous video, we talked about VLOOKUP for data cleaning.
- We also discussed the importance of preparing our spreadsheet before putting VLOOKUP to use.
- Now we're going to experience it in action.
- As a quick reminder, VLOOKUP is a spreadsheet function that vertically searches for a certain value in a column to return a corresponding piece of information.
- Let's start with VLOOKUP syntax.
- This example, 103 is a value to search for.
- A2:B26 is the range that will be searched.
- As you may remember, VLOOKUP will not recognize column names such as A, B, or C.
- We use a number to indicate the column.
- Lastly, FALSE tells VLOOKUP to find an exact match.
- If this said true, the function will return only a close match, which might not be what we want.
- Now let's put VLOOKUP to use.
- One of the most common things data analysts do with VLOOKUP is populating data in one spreadsheet from another.
- Here's an example.
- Let's say we're working with data that exists in two different spreadsheets, but we need information from both in order to answer our business question.
- VLOOKUP can connect two sheets together on a matching column to populate one single sheet.
- Check it out.
- In this spreadsheet, we have employee ID numbers and their rates of pay.
- In this spreadsheet we have the same employee ID numbers and how many hours each person worked.
- We can use VLOOKUP to search for the rate of pay from the employee rates spreadsheet and add it to the employee hours spreadsheet.
- The formula is equals VLOOKUP open parentheses, then A2, which is the first employee ID number and the employee hours spreadsheet.
- Next, we add a comma, the name of the spreadsheet we want to search in, employee rates.
- Be sure to put single quotation marks around the spreadsheet name and add an exclamation point after it.
- This is the way to reference the other spreadsheet.
- Next, we add the range, which is A2 through B5.
- As you saw in a previous video, we can also choose to add dollar signs to lock the range with absolute cell references.
- This prevents them from changing when copying the formula to other cells.
- Add another comma, then a two.
- The two indicates that we want to search for a match in the second column, column B for rate of pay.
- Finally, one more comma and we add false to look up an exact match.
- Drag the formula down the column and now we can use a simple multiplication formula to calculate each person's paycheck by multiplying hours worked by our newly created pay rate column.
- Great work.
- In an upcoming reading, you'll learn even more about VLOOKUP and access some helpful VLOOKUP reminders and resources.
- VLOOKUP is one of the more complicated functions , so keep practicing.

## Notes

- Syntax: `VLOOKUP(103, A2:B26, 2, FALSE)`
  - `103`: a value to search for
  - `A2:B26`: is the range that will be searched
  - `2`: a number indicate the column (not A, B , C)
  - `FALSE`: tells VLOOKPUP to find an exact match
- Example in video: `=VLOOKUP(A2,'Employee Rates'!$A$2:$B$5,2, FALSE)`
  - A2:

## Questions

Would you like to follow along with the instructor using the same spreadsheet? To use the template for the spreadsheet, click the links below and select "Use Template." The template has two tabs for the worksheets, Employee Hours and Employee Rates. 

Link to template: [VLOOKUP in Action Example](https://docs.google.com/spreadsheets/d/1f39uwSgf7N-bgc5GMAtaSefUPw0EIaAB4eKau7t0SXU/template/preview?resourcekey=0-fTi9xv6oG-88MRHHfVkHGQ)

OR If you don't have a Google account, you can download the spreadsheet from the attachment [vlookup-in-action-example.xlsx](./resources/vlookup-in-action-example.xlsx).

- If you enter FALSE as the last input parameter in a VLOOKUP function, VLOOKUP will search for _____.  
  - `an exact match`
  - the closest match
  - a text string
  - a numeric value

> If you enter FALSE as the last input parameter in a VLOOKUP function,  VLOOKUP will search for an exact match.

## Keypoints

- **Introduction to VLOOKUP**: The video briefly recaps the definition of VLOOKUP as a spreadsheet function that vertically searches for a specific value in a column to return a corresponding piece of information.
- **VLOOKUP Syntax Example**: The syntax of a VLOOKUP function is explained using an example. The syntax includes the value to search for (e.g., 103), the range to be searched (e.g., A2:B26), a number indicating the column (since VLOOKUP doesn't recognize column names), and the parameter FALSE to find an exact match.
- **Common Usage of VLOOKUP**: One of the most common applications of VLOOKUP is demonstrated. It involves populating data in one spreadsheet from another by connecting them based on a matching column. The example involves two spreadsheets: one with employee ID numbers and rates of pay, and another with the same employee ID numbers and hours worked.
- **Step-by-Step VLOOKUP Example**: The video provides a step-by-step example of using VLOOKUP to search for the rate of pay from the "Employee Rates" spreadsheet and adding it to the "Employee Hours" spreadsheet. The formula is explained in detail, including the use of single quotation marks and exclamation points to reference the other spreadsheet.
- **Handling Absolute Cell References**: The importance of using absolute cell references (e.g., $A$2:$B$5) to lock the range and prevent changes when copying the formula to other cells is emphasized.
- **Result and Further Calculations**: After applying the VLOOKUP formula, the video demonstrates further calculations, such as using a simple multiplication formula to calculate each person's paycheck by multiplying hours worked by the newly created pay rate column.
- **Encouragement to Practice**: The video concludes by encouraging viewers to practice using VLOOKUP, acknowledging that it is one of the more complicated functions.