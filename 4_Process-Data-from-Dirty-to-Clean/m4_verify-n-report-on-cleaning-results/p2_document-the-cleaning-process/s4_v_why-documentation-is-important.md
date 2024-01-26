# VIDEO: Why documentation is important

Video transcript

- Great, you're back.
- Let's set the stage.
- The crime is dirty data.
- We've gathered the evidence.
- It's been cleaned, verified, and cleaned again.
- Now it's time to present our evidence.
- We'll retrace the steps and present our case to our peers.
- As we discussed earlier, data cleaning, verifying, and reporting is a lot like crime drama.
- Now it's our day in court.
- Just like a forensic scientist testifies on the stand about the evidence, data analysts are counted on to present their findings after a data cleaning effort.
- Earlier, we learned how to document and track every step of the data cleaning process, which means we have solid information to pull from.
- As a quick refresher, documentation is the process of tracking changes, additions, deletions, and errors involved in a data cleaning effort, changelogs are good example of this.
- Since it's staged chronologically, it provides a real-time account of every modification.
- Documenting will be a huge time saver for you as a future data analyst.
- It's basically a cheatsheet you can refer to if you're working with the similar data set or need to address similar errors.
- While your team can view changelogs directly, stakeholders can't and have to rely on your report to know what you did.
- Lets check out how we might document our data cleaning process using example we worked with earlier.
- In that example, we found that this association had two instances of the same membership for $500 in its database.
- We decided to fix this manually by deleting the duplicate info.
- There're plenty of ways we could go about documenting what we did.
- One common way is to just create a doc listing out the steps we took and the impact they had.
- For example, first on your list would be that you remove the duplicate instance,
- which decreased the number of rows from 33 to 32,
- and lowered the membership total by $500.
- If we were working with SQL, we could include a comment in the statement describing the reason for a change without affecting the execution of the statement.
- That's something a bit more advanced, which we'll talk about later.
- Regardless of how we capture and share our changelogs, we're setting ourselves up for success by being 100 percent transparent about our data cleaning.
- This keeps everyone on the same page and shows project stakeholders that we are accountable for effective processes.
- In other words, this helps build our credibility as witnesses who can be trusted to present all the evidence accurately during testimony.
- For dirty data, it's an open and shut case.

## Key Points

- **Importance of Documentation**: Documentation is crucial for presenting findings after a data cleaning effort. It involves tracking changes, additions, deletions, and errors, providing a real-time account of modifications made during the process.
- **Analogy to Crime Drama**: The video uses the analogy of crime drama, presenting the data cleaning, verifying, and reporting process as a court case where data analysts testify about their findings.
- **Changelogs as Documentation**: Changelogs, which chronologically record modifications, serve as a valuable example of documentation. They act as a cheatsheet for future reference and are particularly useful when working with similar datasets or addressing similar errors.
- **Time-Saving and Transparency**: Documentation, in the form of changelogs or other methods, is a time saver for future data analysts, offering a clear record of the steps taken. It ensures transparency, keeping everyone on the same page, and builds credibility by showing accountability for effective processes.