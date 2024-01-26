# Capture cleaning changes

Video transcript

- Hi again.
- Now that you've learned how to make your data squeaky clean, it's time to address all the dirt you've left behind.
- When you clean your data, all the incorrect or outdated information is gone, leaving you with the highest-quality content.
- But all those changes you made to the data are valuable too.
- In this video, we'll discuss why keeping track of changes is important to every data project and how to document all your cleaning changes to make sure everyone stays informed.
- This involves documentation which is the process of tracking changes, additions, deletions and errors involved in your data cleaning effort.
- You can think of it like a crime TV show.
- Crime evidence is found at the scene and passed on to the forensics team.
- They analyze every inch of the scene and document every step, so they can tell a story with the evidence.
- A lot of times, the forensic scientist is called to court to testify about that evidence, and they have a detailed report to refer to.
- The same thing applies to data cleaning.
- Data errors are the crime, data cleaning is gathering evidence, and documentation is detailing exactly what happened for peer review or court.
- Having a record of how a data set evolved does three very important things.
- First, it lets us recover data-cleaning errors.
- Instead of scratching our heads, trying to remember what we might have done three months ago, we have a cheat sheet to rely on if we come across the same errors again later.
- It's also a good idea to create a clean table rather than overriding your existing table.
- This way, you still have the original data in case you need to redo the cleaning.
- Second, documentation gives you a way to inform other users of changes you've made.
- If you ever go on vacation or get promoted, the analyst who takes over for you will have a reference sheet to check in with.
- Third, documentation helps you to determine the quality of the data to be used in analysis.
- The first two benefits assume the errors aren't fixable.
- But if they are, a record gives the data engineer more information to refer to.
- It's also a great warning for ourselves that the data set is full of errors and should be avoided in the future.
- If the errors were time-consuming to fix, it might be better to check out alternative data sets that we can use instead.
- Data analysts usually use a changelog to access this information.
- As a reminder, a changelog is a file containing a chronologically ordered list of modifications made to a project.
- You can use and view a changelog in spreadsheets and SQL to achieve similar results.
- Let's start with the spreadsheet.
- We can use Sheet's version history, which provides a real-time tracker of all the changes and who made them from individual cells to the entire worksheet.
- To find this feature, click the File tab, and then select Version history.
- In the right panel, choose an earlier version.
- We can find who edited the file and the changes they made in the column next to their name.
- To return to the current version, go to the top left and click "Back." If you want to check out changes in a specific cell, we can right-click and select Show Edit History.
- Also, if you want others to be able to browse a sheet's version history, you'll need to assign permission.
- Now let's switch gears and talk about SQL.
- The way you create and view a changelog with SQL depends on the software program you're using.
- Some companies even have their own separate software that keeps track of changelogs and important SQL queries.
- This gets pretty advanced.
- Essentially, all you have to do is specify exactly what you did and why when you commit a query to the repository as a new and improved query.
- This allows the company to revert back to a previous version if something you've done crashes the system, which has happened to me before.
- Another option is to just add comments as you go while you're cleaning data in SQL.
- This will help you construct your changelog after the fact.
- For now, we'll check out query history, which tracks all the queries you've run.
- You can click on any of them to revert back to a previous version of your query or to bring up an older version to find what you've changed.
- Here's what we've got.
- I'm in the Query history tab.
- Listed on the bottom right are all the queries that run by date and time.
- You can click on this icon to the right of each individual query to bring it up to the Query editor.
- Changelogs like these are a great way to keep yourself on track.
- It also lets your team get real-time updates when they want them.
- But there's another way to keep the communication flowing, and that's reporting.
- Stick around, and you'll learn some easy ways to share your documentation and maybe impress your stakeholders in the process.
- See you in the next video.

## Question

### **Clarification**

- The instructor stated that the first two benefits of documentation
  - 1) recalling the errors that were cleaned and
  - 2) informing others of the changes

Assume that the data errors aren't fixable. She then added that when the data errors are fixable, the documentation needs to record how the data was fixed. Data-cleaning documentation is important in both cases.

## Key Points

- After cleaning data, changes made are valuable, and documenting them is crucial for various reasons.
- Documentation involves tracking changes, additions, deletions, and errors during the data cleaning process. With 3 important things:
  - Recover data-cleaning errors
  - Inform other users of changes
  - Determine quality of data
- It's analogous to a crime scene investigation, where evidence is analyzed and documented to tell a story.
- **A changelog** is a file listing modifications made to a project in chronological order, commonly used by data analysts.
- Documentation serves to recover data-cleaning errors, inform other users of changes, and assess the quality of data for analysis.
- Creating a clean table rather than overwriting the existing one ensures the availability of the original data.
