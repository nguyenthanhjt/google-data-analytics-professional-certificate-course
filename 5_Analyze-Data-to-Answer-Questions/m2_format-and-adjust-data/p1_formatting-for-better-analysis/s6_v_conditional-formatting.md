# Conditional formatting

Video transcript

- Hi again.
- So earlier we talked about conditional formatting as a spreadsheet tool that changes how cells appear when values meet specific conditions.
- This lets you add visual cues to your spreadsheets that make it easier to understand your table at a glance, and it makes the information in the worksheet clearer to your stakeholders.
- In this video, we'll take that even further by combining conditional formatting and data validation to create custom tools for our spreadsheets.
- So far, we've used conditional formatting to highlight empty cells that still needed data so that we could quickly pinpoint what information our table was missing and add it in.
- Now, let's build on that by using it to make our scheduling table easier to read at a glance.
- Here's a table we worked with when we covered data validation.
- It's tracking the status of different tasks on our project for our team to check on.
- But now there's even more tasks than the last time we looked at it.
- This table has useful information, but it takes a second to understand.
- Right now we don't have a visual on how many tasks are in progress or how many upcoming deadlines there are.
- But if we color-coded those elements of the table, we could quickly see key pieces of data really easily.
- Let's start with the Status column, column C.
- In the last example, we created these drop- down menus with the data validation tool.
- Now we can use conditional formatting to add some color.
- Let's go to the conditional formatting option under the Format menu.
- This brings up a sidebar where we can select our range rule in formatting style.
- We need to decide which rows to apply our formatting to when the condition we set is met.
- We can click this button in the range options to select all of the rows we're applying the formatting to instead of typing it in.
- Now that we have those cells selected, we can choose the rule that we want to apply to these cells.
- We already have drop-down menus with specific text.
- So we can choose "Format Cells if...
- Text is exactly" from the rules.
- For our first rule, let's write "Not Yet Started" as the text condition.
- Then we'll choose a color to apply to those cells that have "Not Yet Started" in them.
- Let's use red.
- Now all cells that have "Not Yet Started" selected from the drop- down menu will be red.
- Let's hit the "Add another rule" button to add conditional formatting to other status options.
- Let's add the condition "In Progress" next.
- We can make that one yellow.
- And then we'll add one last rule for "Ready." Let's choose green.
- And there.
- Now we have an easy-to- understand visual cue that tells us how many tasks are in progress, and how many are completed.
- We can also combine data validation and conditional formatting to track upcoming deadlines.
- We have a column of dates called "Review By This Date." First, let's use the data validation functionality to make sure users only enter valid dates.
- We'll go back to the Data dropdown at the top, pull up Data validation, and select Date as our criteria.
- Then we can go to the Format menu at the top.
- Go down to conditional formatting and open the sidebar again.
- We'll click the "Select range" icon and select the "Review By This Date" column.
- Now under Format rules, we can select "Date is after," which will give us another option.
- Let's choose "today."
- And finally, let's choose the color for these cells.
- So if the date listed in these rows is after today, it'll be filled in orange.
- You can also choose a specific locked date if needed.
- But for now, let's go with today.
- Now all of the upcoming review dates have an easy-to-see color code, so anyone using this table can quickly reference these deadlines.
- You'll find that some spreadsheet programs, like Excel, have built-in color codes that you can use, too.
- And there you go.
- Now you know how to use data validation and conditional formatting to create custom tools and visual cues that make your information easy to understand.
- There's a lot of different ways to use these tools, so feel free to experiment with them in your own spreadsheets.
- Coming up, we'll keep learning about new tools for spreadsheets and SQL.
- Bye for now.

## Question

If you followed along with the instructor in the Data Validation video, click Continue and use the same spreadsheet to continue following along.

If you didn't previously follow along, or hopped around videos, click the link below and select "Use Template" to follow along with this video.

Link to template: [Project Spreadsheet - for Conditional Formatting](https://docs.google.com/spreadsheets/d/1n-DgzjmR3dAZwBTI0XtvQHNrkwxYGOGxdcZTpxzA6LQ/template/preview#gid=1265595766)

OR If you don't have a Google account, you can download the spreadsheet directly from the attachment: [project-spreadsheet_for-conditional-formatting.xlsx](./resources/project-spreadsheet_for-conditional-formatting.xlsx)

### Question 1: Conditional formatting can be used for which spreadsheet tasks? Select all that apply

- `Color-coding cells that contain dates after today`
- Adding a dropdown menu
- `Highlighting cells tha contain the word “ready”`
- Allowing users to input only structured data and formulas

> Conditional formatting is a spreadsheet tool that changes how cells appear when values meet specific conditions. It can be used to change a cell’s color in order to highlight it.

## Section Overview

This video discusses the use of conditional formatting as a spreadsheet tool to enhance the visual representation of data. It emphasizes combining conditional formatting with data validation to create custom tools and visual cues for better spreadsheet comprehension.

- Purpose of Conditional Formatting:
  - Conditional formatting is a tool that alters how cells appear based on specific conditions, adding visual cues to improve understanding at a glance.
- Combining Conditional Formatting and Data Validation:
  - The video builds on previous knowledge of data validation, incorporating conditional formatting to make scheduling tables easier to read.
  - Demonstrates using conditional formatting to highlight different task statuses and upcoming deadlines.
- Example: Status Column Formatting:
  - The Status column (e.g., "Not Yet Started," "In Progress," "Ready") is color-coded using conditional formatting.
  - Specific rules are applied based on text conditions, and each status is assigned a unique color for quick visual identification.
- Example: Upcoming Deadlines Formatting:
  - Data validation is used to ensure valid dates in the "Review By This Date" column.
  - Conditional formatting is applied to highlight dates that are after the current date, using an orange color.
  - Provides flexibility to choose specific dates if required.
- Benefits of Visual Cues:
  - Visual cues, such as color-coded status and upcoming deadlines, enhance the user's ability to quickly grasp key information in the spreadsheet.
- Custom Tools and Visual Cues:
  - Users can leverage data validation and conditional formatting to create custom tools and visual cues tailored to their specific spreadsheet needs.
- Experimentation and Exploration:
  - Encourages users to experiment with these tools in their own spreadsheets to discover different ways to enhance data presentation.
- Built-in Color Codes:
  - Some spreadsheet programs, like Excel, offer built-in color codes that users can utilize for conditional formatting.
