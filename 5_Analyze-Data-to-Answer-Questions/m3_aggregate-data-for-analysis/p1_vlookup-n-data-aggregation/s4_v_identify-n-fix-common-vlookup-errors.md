# Identify and fix common VLOOKUP errors

Video transcript

- When people start out in data analytics, they often think that those of us who've been in the field for a while know everything.
- But trust me, we're all still figuring things out.
- And a lot of the time that means troubleshooting.
- Troubleshooting has to do with asking the right questions, and that's what we'll focus on in this video.
- We'll learn how you can use troubleshooting to solve all kinds of problems.
- To do this, we'll need to talk about some of the limitations of VLOOKUP and then practice fixing some of the most common problems that data analysts face.
- Some of the troubleshooting questions I like to ask myself: How should I prioritize these issues? Trying to solve lots of problems all at once can feel overwhelming.
- I find it helps when you take things one at a time.
- Next I ask, In a single sentence, what's the issue I'm facing? This helps to clarify what's really going on, so I don't get bogged down with extra details.
- After all, if you don't have a clear objective before looking at the data, you can find just about anything.
- It's always best to start with your own clear understanding of the situation.
- Then let the data tell you if you're on the right track or not.
- The next question I ask myself is, What resources can help me solve the problem? The internet is one of the best resources out there.
- If you have a question, chances are thousands of others run into exactly the same thing.
- So a quick search can be really helpful.
- And it's good to remember that people are resources, too.
- Don't be afraid to ask questions.
- Not only is it a great way to learn, it can also help you build strong relationships with your colleagues.
- And a final important question I think about: How can I stop this problem from happening in the future? If a new procedure or guideline can stop the same issue from popping up again, that's a great time-saver.
- All right.
- Let's start by noting that VLOOKUP only returns the first match it finds, even if there are lots of possible matches.
- Something else to keep in mind is that VLOOKUP can only return a value from the data to the right.
- It can't look left.
Play video starting at :2:8 and follow transcript2:08
Good news.
- There's a simple solution.
- Data analysts usually get around the problem by copying and pasting a column to the left of the data they want to look at.
- This way, the lookup value is in the leftmost column and the data they want is to the right of it.
Play video starting at :2:24 and follow transcript2:24
Here's another problem I see a lot.
- Let's say the first few rows of a VLOOKUP have returned the correct result.
- But when you drive the function down the column, problems start popping up.
Play video starting at :2:36 and follow transcript2:36
This is probably because the table array part of the function hasn't been locked or made absolute.
Play video starting at :2:43 and follow transcript2:43
An absolute reference is a reference that is locked so that rows and columns won't change when copied.
- You can fix this issue by wrapping the table array in dollar signs.
- As you learned a while back, the dollar sign controls how the reference will be updated.
- They make sure that the corresponding part of the reference doesn't change.
- Something else that can throw off your VLOOKUP results are version control issues.
- In other words, a function worked perfectly at first, but then something in the spreadsheet it was referencing changed.
- For example, maybe a user inserted a column.
- So now the columns in your function no longer direct VLOOKUP to the right place.
- When something like this happens, it'll return an incorrect value.
- There are a few actions data analysts can take to ensure this doesn't happen.
- First, lock the spreadsheet.
- This stops other people from making changes.
Play video starting at :3:35 and follow transcript3:35
To do this in Sheets, select Data, then Protected sheets and ranges.
- In other spreadsheet applications, there are other tools that do the same thing.
- Next, choose what you want to protect.
- In this case, we want to protect the entire sheet.
- Then you can set permissions to either show a warning or restrict who can edit.
- Choose only you, then Done.
Play video starting at :3:58 and follow transcript3:58
But keep in mind, there will be times when other people need to work in the spreadsheet, so locking them out might make you pretty unpopular with your coworkers.
- When that's the case, you can use MATCH, which is a function used to locate the position of a specific lookup value and can help you with version control.
- We won't get into that right now, but just know that it's an option in case you ever need it.
- The final problem we'll talk about has to do with exact and approximate matching.
- When using VLOOKUP, you're likely to get different results, depending on whether you enter the word TRUE or FALSE within your function.
- TRUE tells VLOOKUP to look for approximate matches, and FALSE tells VLOOKUP to look for exact matches.
- So if a function looks like this, it's telling VLOOKUP to find the closest match to the text or number we're looking for.
- It's important to know that VLOOKUP starts at the top of a specified range and searches downward vertically in each cell to find the right value.
- It stops searching when it finds any value that's greater than or equal to the lookup value.
- That's why data analysts typically use FALSE, like this.
- That way VLOOKUP only returns the exact match to what you've entered in the lookup value.
- VLOOKUP is one of the most popular lookup and reference functions in spreadsheets.
- It's also one of the trickiest.
- Coming up, you'll learn about more of these common challenges.
- Everything you learn will help you run into fewer problems when you start using VLOOKUP as a future data analyst.

## Notes

- Troubleshooting questions
  - How should I priortize these issues?
  - In a single sentence, what's the issue I'm facing?
  - What recources can help me solve the problem?
  - How can I stop this problem from happening in the future?
- Absoulute reference: a reference that is locked so that rows and columns won't change when copied.
- `MATCH`: a function used to locate the position of a specific lookup value
- `TRUE` tells VLOOKUP to look for approximately matches
- `FALSE` tells VLOOKUP to look for exact matches
- `VLOOKUP(A2, 'Sheet 2'!A:B, 2, TRUE)`: it's telling VLOOKUP to find the closest match

## Question

- VLOOKUP has certain limitations. One limitation is that it only returns the first match it finds within the specified range. Another limitation is that VLOOKUP can only search through the first column in a spreadsheet.
  - True
  - `False`

> VLOOKUP only returns the first match it finds within a specified range and can only search in columns to the right.

- In the function =VLOOKUP(K2,'Sheet 4'!A:B,2,TRUE), what does the word TRUE indicate?
  - TRUE tells VLOOKUP to search for as many matches as it can find in the specified range.
  - TRUE tells VLOOKUP to start at the top of the specified range.
  - TRUE tells VLOOKUP to search for exact matches.
  - `TRUE tells VLOOKUP to search for approximate matches`.

> In the function =VLOOKUP(K2,'Sheet 4'!A:B,2,TRUE), TRUE tells VLOOKUP to search for approximate matches.

## Keypoints

- **Introduction to Troubleshooting**: The video starts by acknowledging that troubleshooting is a common practice in data analytics. The importance of asking the right questions to solve problems is emphasized.
- **Prioritizing Issues**: One of the suggested troubleshooting strategies is to prioritize issues. It's recommended to tackle problems one at a time to avoid feeling overwhelmed.
- **Clarifying the Issue**: Another strategy is to articulate the issue in a single sentence. This helps in focusing on the core problem without getting lost in unnecessary details.
- **Understanding the Situation**: The importance of having a clear understanding of the situation before delving into data analysis is highlighted. Letting the data confirm if you're on the right track is crucial.
- **Utilizing Resources**: The video suggests leveraging resources for problem-solving. The internet is presented as a valuable resource, and the importance of asking questions and learning from colleagues is emphasized.
- **Preventing Future Problems**: An essential question in troubleshooting is how to prevent the problem from happening in the future. Implementing new procedures or guidelines can be a time-saving solution.
- **Limitations of VLOOKUP**: The video discusses some limitations of VLOOKUP. It only returns the first match it finds, and it can only return a value from the data to the right; it cannot look left.
- **Solution for Left Lookup**: To overcome the limitation of left lookup, data analysts often copy and paste a column to the left of the data they want to look at. This way, the lookup value becomes the leftmost column.
- **Table Array Locking**: Problems with VLOOKUP results during column expansion might be due to the table array part of the function not being locked or made absolute. The importance of using absolute references (e.g., $A$2:$B$5) is explained.
- **Version Control Issues**: Changes in the spreadsheet, such as inserting a column, can disrupt VLOOKUP results. Locking the spreadsheet or using the MATCH function for version control is suggested.
- **Exact and Approximate Matching**: VLOOKUP behavior differs when using TRUE or FALSE for approximate or exact matching, respectively. The video explains that TRUE looks for approximate matches, while FALSE looks for exact matches.
- **VLOOKUP Challenges**: VLOOKUP is acknowledged as one of the most popular lookup and reference functions but is also recognized as tricky. Viewers are encouraged to continue learning about common challenges associated with VLOOKUP.
