# Recognize and remedy dirty data

Video transcript

- Hey, there.
- In this video, we'll focus on common issues associated with dirty data.
- These includes spelling and other texts errors, inconsistent labels, formats and field lane, missing data and duplicates.
- This will help you recognize problems quicker and give you the information you need to fix them when you encounter something similar during your own analysis.
- This is incredibly important in data analytics.
- Let's go back to our law office spreadsheet.
- As a quick refresher, we'll start by checking out the different types of dirty data it shows.
- Sometimes, someone might key in a piece of data incorrectly.
- Other times, they might not keep data formats consistent.
- It's also common to leave a field blank.
- That's also called a null, which we learned about earlier.
- If someone adds the same piece of data more than once, that creates a duplicate.
- Let's break that down.
- Then we'll learn about a few other types of dirty data and strategies for cleaning it.
- Misspellings, spelling variations, mixed up letters, inconsistent punctuation, and typos in general, happen when someone types in a piece of data incorrectly.
- As a data analyst, you'll also deal with different currencies.
- For example, one dataset could be in US dollars and another in euros, and you don't want to get them mixed up.
- We want to find these types of errors and fix them like this.
- You'll learn more about this soon.
- Clean data depends largely on the data integrity rules that an organization follows, such as spelling and punctuation guidelines.
- For example, a beverage company might ask everyone working in its database to enter data about volume in fluid ounces instead of cups.
- It's great when an organization has rules like this in place.
- It really helps minimize the amount of data cleaning required, but it can't eliminate it completely.
- Like we discussed earlier, there's always the possibility of human error.
- The next type of dirty data our spreadsheet shows is inconsistent formatting.
- In this example, something that should be formatted as currency is shown as a percentage.
- Until this error is fixed, like this, the law office will have no idea how much money this customer paid for its services.
- We'll learn about different ways to solve this and many other problems soon.
- We discussed nulls previously, but as a reminder, nulls are empty fields.
- This kind of dirty data requires a little more work than just fixing a spelling error or changing a format.
- In this example, the data analysts would need to research which customer had a consultation on July 4th, 2020.
- Then when they find the correct information, they'd have to add it to the spreadsheet.
- Another common type of dirty data is duplicated.
- Maybe two different people added this appointment on August 13th, not realizing that someone else had already done it or maybe the person entering the data hit copy and paste by accident.
- Whatever the reason, it's the data analyst job to identify this error and correct it by deleting one of the duplicates.
- Now, let's continue on to some other types of dirty data.
- The first has to do with labeling.
- To understand labeling, imagine trying to get a computer to correctly identify panda bears among images of all different kinds of animals.
- You need to show the computer thousands of images of panda bears.
- They're all labeled as panda bears.
- Any incorrectly labeled picture, like the one here that's just bear, will cause a problem.
- The next type of dirty data is having an inconsistent field length.
- You learned earlier that a field is a single piece of information from a row or column of a spreadsheet.
- Field length is a tool for determining how many characters can be keyed into a field.
- Assigning a certain length to the fields in your spreadsheet is a great way to avoid errors.
- For instance, if you have a column for someone's birth year, you know the field length is four because all years are four digits long.
- Some spreadsheet applications have a simple way to specify field lengths and make sure users can only enter a certain number of characters into a field.
- This is part of data validation.
- Data validation is a tool for checking the accuracy and quality of data before adding or importing it.
- Data validation is a form of data cleansing, which you'll learn more about soon.
- But first, you'll get familiar with more techniques for cleaning data.
- This is a very important part of the data analyst job.
- I look forward to sharing these data cleaning strategies with you.

## Questions

Fill in the blank: Data _____ is a cleaning feature to check the accuracy and quality of data before adding or importing it.

- security
- `validation`: Data validation is a cleaning feature to check the accuracy and quality of data before adding or importing it.
- mapping
- governance

## Keypoints

- Common Issues Associated with Dirty Data:
  - Spelling and other text errors.
  - Inconsistent labels, formats, and field length.
  - Missing data (nulls).
  - Duplicate data.
- Recognizing and Fixing Dirty Data:
  - Spelling Errors:
    - Examples: Misspellings, spelling variations, mixed-up letters, inconsistent punctuation, and typos.
    - Importance: Typos can occur when someone types in data incorrectly, leading to dirty data.
    - Solution: Implement data integrity rules, such as spelling and punctuation guidelines.
  - Inconsistent Formatting:
    - Examples: Formatting errors like showing currency as a percentage.
    - Importance: Inconsistent formatting can lead to misinterpretation of data.
    - Solution: Fix formatting errors to ensure accurate representation of numerical data.
  - Nulls (Missing Data):
    - Definition: Nulls are empty fields that require more attention than fixing a simple error.
    - Example: Researching and adding information to fields with missing data.
    - Importance: Nulls can hinder analysis and decision-making.
    - Solution: Research and update missing data based on accurate information.
  - Duplicate Data:
    - Examples: Duplicate entries created by different users or accidental copy-paste.
    - Importance: Duplicate data can skew metrics and cause confusion during analysis.
    - Solution: Identify and correct duplicate entries by removing one of them.
  - Labeling Issues:
    - Definition: Incorrect labels can lead to misclassification, affecting analysis.
    - Example: Inconsistent labels in datasets.
    - Importance: Proper labeling is crucial for accurate data interpretation.
    - Solution: Ensure consistent and accurate labeling, especially in classification tasks.
  - Inconsistent Field Length:
    - Definition: Field length determines the number of characters that can be entered into a field.
    - Example: Assigning incorrect field lengths, leading to potential errors.
    - Importance: Proper field length helps avoid errors in data entry.
    - Solution: Specify correct field lengths to ensure data accuracy.
- Data Validation:
  - Definition: Data validation is a tool for checking the accuracy and quality of data before adding or importing it.
  - Importance: Data validation is part of data cleansing to ensure accurate and reliable data.
  - Solution: Implement data validation techniques as part of data cleaning strategies.
- Upcoming Topics:
  - The video hints at upcoming topics, including more techniques for cleaning data.
  - Emphasizes the importance of data cleaning in the data analyst's job.
