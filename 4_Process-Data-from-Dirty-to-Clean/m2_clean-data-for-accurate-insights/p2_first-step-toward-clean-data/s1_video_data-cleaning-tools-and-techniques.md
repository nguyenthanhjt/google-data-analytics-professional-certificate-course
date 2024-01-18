# Data-cleaning tools and techniques

VIDEO transcript.

- Hi.
- Now that you're familiar with some of the most common types of dirty data, it's time to clean them up.
- As you've learned, clean data is essential to data integrity and reliable solutions and decisions.
- The good news is that spreadsheets have all kinds of tools you can use to get your data ready for analysis.
- The techniques for data cleaning will be different depending on the specific data set you're working with.
- So we won't cover everything you might run into, but this will give you a great starting point for fixing the types of dirty data analysts find most often.
- Think of everything that's coming up as a teaser trailer of data cleaning tools.
- I'm going to give you a basic overview of some common tools and techniques, and then we'll practice them again later on.
- Here, we'll discuss how to remove unwanted data, clean up text to remove extra spaces and blanks, fix typos, and make formatting consistent.
- However, before removing unwanted data, it's always a good practice to make a copy of the data set.
- That way, if you remove something that you end up needing in the future, you can easily access it and put it back in the data set.
- Once that's done, then you can move on to getting rid of the duplicates or data that isn't relevant to the problem you're trying to solve.
- Typically, duplicates appear when you're combining data sets from more than one source or using data from multiple departments within the same business.
- You've already learned a bit about duplicates, but let's practice removing them once more now using this spreadsheet, which lists members of a professional logistics association.
- Duplicates can be a big problem for data analysts.
- So it's really important that you can find and remove them before any analysis starts.
- Here's an example of what I'm talking about.
- Let's say this association has duplicates of one person's $500 membership in its database.
- When the data is summarized, the analyst would think there was $1,000 being paid by this member and would make decisions based on that incorrect data.
- But in reality, this member only paid $500.
- These problems can be fixed manually, but most spreadsheet applications also offer lots of tools to help you find and remove duplicates.
- Now, irrelevant data, which is data that doesn't fit the specific problem that you're trying to solve, also needs to be removed.
- Going back to our association membership list example, let's say a data analyst was working on a project that focused only on current members.
- They wouldn't want to include information on people who are no longer members,
- or who never joined in the first place.
- Removing irrelevant data takes a little more time and effort because you have to figure out the difference between the data you need and the data you don't.
- But believe me, making those decisions will save you a ton of effort down the road.
- The next step is removing extra spaces and blanks.
- Extra spaces can cause unexpected results when you sort, filter, or search through your data.
- And because these characters are easy to miss, they can lead to unexpected and confusing results.
- For example, if there's an extra space and in a member ID number, when you sort the column from lowest to highest, this row will be out of place.
- To remove these unwanted spaces or blank cells, you can delete them yourself.
- Or again, you can rely on your spreadsheets, which offer lots of great functions for removing spaces or blanks automatically.
- The next data cleaning step involves fixing misspellings, inconsistent capitalization, incorrect punctuation, and other typos.
- These types of errors can lead to some big problems.
- Let's say you have a database of emails that you use to keep in touch with your customers.
- If some emails have misspellings, a period in the wrong place, or any other kind of typo, not only do you run the risk of sending an email to the wrong people, you also run the risk of spamming random people.
- Think about our association membership example again.
- Misspelling might cause the data analyst to miscount the number of professional members if they sorted this membership type and then counted the number of rows.
- Like the other problems you've come across, you can also fix these problems manually.
- Or you can use spreadsheet tools, such as spellcheck, autocorrect, and conditional formatting to make your life easier.
- There's also easy ways to convert text to lowercase, uppercase, or proper case, which is one of the things we'll check out again later.
- All right, we're getting there.
- The next step is removing formatting.
- This is particularly important when you get data from lots of different sources.
- Every database has its own formatting, which can cause the data to seem inconsistent.
- Creating a clean and consistent visual appearance for your spreadsheets will help make it a valuable tool for you and your team when making key decisions.
- Most spreadsheet applications also have a "clear formats" tool, which is a great time saver.
- Cleaning data is an essential step in increasing the quality of your data.
- Now you know lots of different ways to do that.
- In the next video, you'll take that knowledge even further and learn how to clean up data that's come from more than one source.

## Keypoints

This section emphasizes the importance of clean data and introduces common tools and techniques for data cleaning.

- **Overview of Data Cleaning Tools and Techniques**:
  - Clean data is crucial for data integrity and reliable analysis.
  - Spreadsheets offer various tools for data cleaning, and techniques may vary based on the dataset.
  - The section provides a teaser trailer of data cleaning tools, focusing on removing unwanted data, cleaning up text, fixing typos, and ensuring consistent formatting.
- **Steps in Data Cleaning**:
  - Before removing unwanted data, it's recommended to make a copy of the dataset to preserve the original data.
  - Duplicates are common issues, especially when combining data from different sources. Tools within spreadsheet applications can help identify and remove duplicates.
  - Irrelevant data, which doesn't fit the specific problem, needs to be removed to ensure focused analysis.
  - Removing extra spaces and blanks is crucial to avoid unexpected issues during sorting, filtering, or searching. Spreadsheet functions can automate this process.
  - Fixing misspellings, inconsistent capitalization, and typos is essential for accurate analysis. Spreadsheet tools like spellcheck, autocorrect, and conditional formatting can assist.
  - Removing formatting is important when dealing with data from various sources to create a consistent visual appearance.
- **Examples and Practical Considerations**:
  - Practical examples, such as a professional logistics association's membership list, illustrate the impact of data issues on analysis.
  - Emphasizes the significance of cleaning data that comes from multiple sources.
- **Next Steps**:
  - The video sets the stage for more in-depth learning about cleaning data from multiple sources in the next section.
