# Video: Using R Markdown in RStudio

Video transcript

- Welcome back.
- Exploring the different tools available for analysis is one of the more fun parts of being a data analyst.
- By now, you've had the chance to try out tools like spreadsheets, BigQuery or other SQL tools and Tableau.
- Now we'll check out a tool you can use in RStudio, R Markdown.
- As a reminder R Markdown is a great tool for documenting your analysis at any stage.
- But especially when you've completed a project.
- Let's open up RStudio and get started with R Markdown.
- Feel free to follow along with the video and try it out on your own later.
- Or go ahead and join us now in your own RStudio account.
- We'll first install the R Markdown package by using our install packages function and R Markdown in parentheses.
- As a reminder, installing packages can take some time.
- Bright red text may show up in your console as it installs.
- That's all perfectly normal.
- Okay, let's open up a new R Markdown or RMD file using the File menu.
- If you're working along with us and you're prompted to install packages that you'll need to open your file, go ahead and click Yes.
- Right away, you might notice some of the outputs available in R Markdown.
- For now, we'll use the default HTML and document options.
- The other output options will also be available later.
- We'll add a file name and author, and then open our file.
- Next, we'll save it so we can use it later.
- So now we have an RMD file filled with metadata at the top and chunks of code in the gray sections.
- There's text in between for explaining the code and adding comments on your analysis and conclusions.
- This R Markdown document's in its original format.
- It's definitely useful and can be edited and added to, but if we want to produce a report containing all text, code and results, we need to click the knit button.
- Now we've got the report.
- It's an HTML file that you can share with others.
- Let's compare the original .rmd file with the HTML report.
- You can tell that the text has been transformed into a more viewer- friendly format.
- Also, the code chunks have all been run.
- And we now have their output: both the columns of data and the plot from an analysis on the cars dataset.
- The report's clear and formatted in a way that's easy to follow and understand.
- We could share it with stakeholders even if they've got no experience in R.
- R Markdown files are definitely an effective way to complete the data analysis process.
- You can start your analysis in R and create a report, complete with code and visualizations, all in the same workspace.
- Coming up, we'll show you more examples of how to use R Markdown to make your documentation even more effective.
- Bye for now.

## Questions & Notes

- **R Markdown**: is a great tool for documenting your analysis at any stage

- With the HTML report shown along side the .RMD file, notice that headings in the report are created when you include one or more hashtags (#) before the heading text, such as ## Including Plots. The more hashtags used, the smaller the heading font. # Including Plots creates a Header 1 style heading whereas ## Including Plots creates a Header 2 style heading.

### Question 1: A data analyst wants to find headers in their R Markdown document. What should they look for?

- [ ] Semicolons
- [x] Hashtags
- [ ] Backticks
- [ ] Spaces

> Correct: Hashtags are used for headers; for example, ### Results indicates that Results is a Header 3 style heading because there three hashtags.

## My wrapped keypoints

In this section, we learned how to use R Markdown in RStudio. Here are the key points from the video transcript:

1. **Introduction to R Markdown**: R Markdown is a tool for documenting analysis, especially at the completion stage of a project. It allows users to create dynamic documents that integrate code, text, and visualizations seamlessly.

2. **Installation of R Markdown Package**: To use R Markdown in RStudio, we first need to install the R Markdown package. This can be done using the `install.packages("rmarkdown")` function in R.

3. **Creating an R Markdown File**: In RStudio, we can create a new R Markdown file (`.Rmd`) using the File menu. After specifying the file name and author, we can open the file.

4. **Editing the R Markdown File**: The R Markdown file contains metadata at the top and chunks of code in gray sections. Text can be added between code chunks to explain the code and provide analysis insights.

5. **Knitting the Document**: To produce a report containing all text, code, and results, we need to click the knit button. This converts the R Markdown file into a readable format, such as an HTML file, suitable for sharing with others.

6. **Comparison of Original and HTML Report**: The HTML report is viewer-friendly, with transformed text and executed code chunks displaying outputs such as data columns and plots. This formatted report is easy to follow and understand, making it suitable for sharing with stakeholders, even those with no experience in R.

7. **Effectiveness of R Markdown**: R Markdown files are effective for completing the data analysis process, allowing users to conduct analysis, create visualizations, and generate reports all within the same workspace.

Overall, R Markdown serves as a valuable tool for documenting and sharing analysis workflows, enabling users to create comprehensive reports that incorporate code, text, and visualizations seamlessly.
