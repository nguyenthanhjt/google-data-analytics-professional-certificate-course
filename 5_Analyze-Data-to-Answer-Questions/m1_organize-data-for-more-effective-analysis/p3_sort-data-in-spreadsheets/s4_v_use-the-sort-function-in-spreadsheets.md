# Use the SORT function in spreadsheets

- Happy to have you back.
- Earlier in the program, we covered some basics of sorting in spreadsheets.
- We learned the differences between sorting a range and an entire sheet, and how to sort a spreadsheet using the menu.
- Now that we've laid the groundwork, it's time to move on to more advanced ways to sort information.
- We've talked about how there's two methods of sorting data in spreadsheets.
- The first method uses the Data tab in the menu of your spreadsheet program.
- The second way to store information in a spreadsheet is by writing a SORT function.
- In spreadsheets, functions are preset commands that perform a specific process.
- So in this case, the SORT function, as you might be able to guess, sorts your data.
- Let's check out this spreadsheet of party plans to witness the SORT function in action.
- The first arranged set of data is our original dataset of guests and some information about them.
- So let's say you want to sort the party guests by table to get an idea of who will be sitting where.
- To do that, start by typing a function in an empty cell.
- Just like any function, you do this by typing the equal sign, and then write SORT after it.
- After your first open parenthesis, reference the first cell in which data is collected from.
- In this case, that's A2.
- Then you'll include a colon and write the last cell you want included in the function, which is D6.
- A2 colon D6 is the range for this function.
- Next, write a comma to separate the range from what we're sorting by, which is column B.
- You should keep in mind that this part of the function doesn't recognize column letters.
- So in this case, we use the corresponding number instead, which is 2, since column B is the second column in our range.
- Now add another comma.
- In this next part you'll need to decide whether you want the data in this column to be in ascending or descending order.
- A TRUE statement is in ascending order, and FALSE is descending.
- Because we want the tables to be listed starting from table number one, we'll write TRUE for ascending, and then end the function with a closed parenthesis.
- Now, let's see our function play out.
- Our party guests are now sorted by which table they're seated.
- Once you have an idea of the data you want to be sorted and how, applying functions to your data is simple.
- Now, you have two different tools in your tool belt for sorting data.
- After you've tackled writing SORT functions, you'll want to customize sort orders, too.
- A customized sort order is when you sort data in a spreadsheet using multiple conditions.
- This means that sorting will be based on the order of the conditions you select.
- Let's go back to our party spreadsheet.
- Imagine you want the guests to be sorted by whether or not they've been sent an invitation.
- And based on that, we want those guest names to be listed alphabetically.
- You can do that easily with the "Sort range" option under Data.
- First, highlight all the data in the set from cells A1 to D6.
- Then under the Data tab in the menu, click "Sort range."
- In this case, check "Data has a header row," which makes sure that the title of the column isn't mixed into the sorting.
- Then, we'll make sure it's being sorted by "Sent invitation." Here, we want the "No" responses first and the "Yes" responses second, so we'll make sure A to Z is clicked to sort the responses in that order.
- Because we want to add an additional sorting condition, we'll now click on "Add another sort column." The guest names should be in alphabetical order.
- So let's select "Guest Names" and sort from A to Z.
- Then we'll click Sort.
- And voilà! You've officially applied a custom sort order like a champ.
- Okay, so you've tackled sorting in spreadsheets by sheet, by range, through the menu, and by using a function.
- On top of all that, you've added to your organizational skills by learning how to create custom sort orders.
- Pretty soon you'll learn another powerful tool: how to sort data using SQL.
- Even though databases can sometimes be a lot to digest, learning these skills gives you the power to rearrange data in a way that makes sense to you.
- Once you've sorted data in a way that really clicks, you'll understand why it's so valuable to you as a data analyst.
- Bye for now!

## Question

Which of the following statements accurately describe differences between the sort from a spreadsheet's Data tab and a written SORT function? Select all that apply.

- `The sort from a spreadsheet's Data tab can exclude a header row in the data range from being sorted, while the data range for a written SORT function should never contain a header row.`
- `The sort from a spreadsheet's Data tab overwrites the cells containing the unsorted data with the sorted data, while a written SORT function inserts the sorted data in a different cell range.`
- The sort from a spreadsheet's Data tab can only sort data by a single sort condition or column, while a written SORT function can sort data by multiple columns.
- The sort from a spreadsheet's Data tab can sort in ascending or descending order, while a written SORT function automatically assumes ascending order.

> The sort from a spreadsheet's Data tab can exclude a header row in the data range from being sorted, while the data range for a written SORT function should never contain a header row.

## Keypoints

- Two Methods of Sorting:
  - Recap of the two primary methods of sorting data in spreadsheets:
  - Using the Data tab in the menu.
  - Writing a `SORT` function.
- Understanding Spreadsheet Functions:
  - Functions in spreadsheets are preset commands that perform specific processes.
  - The SORT function is used to sort data in ascending or descending order.
- Sorting with the SORT Function:
  - Demonstrated the SORT function on a spreadsheet of party plans.
  - Example: Sorting party guests by table number.
  - Function syntax: =SORT(A2:D6, 2, TRUE) - sorts by column B in ascending order.
- Customized Sort Order:
  - Introduced the concept of a customized sort order based on multiple conditions.
  - Applied a custom sort order to sort guests by invitation status and then alphabetically by - guest names.
- Using "Sort Range" Option:
  - Explained how to use the "Sort range" option under Data in the menu.
  - Demonstrated sorting data based on multiple conditions using this option.
- Expanding Sorting Skills:
  - Emphasized the importance of having multiple tools for sorting data.
  - Teased the upcoming topic of sorting data using SQL, adding to the data analyst's skill set.
- Empowering Data Organization:
  - Sorting data is a powerful tool for rearranging information in a meaningful way.
  - Enhances organizational skills, crucial for a data analyst.
- Closing Remarks:
  - Recap of the sorting techniques covered.
  - Encouragement to explore and practice these skills for better data understanding.
