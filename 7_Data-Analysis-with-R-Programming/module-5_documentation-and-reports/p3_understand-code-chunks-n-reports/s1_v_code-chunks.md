# Video: Code chunks

Video transcipt

- Hi again, we've learned a lot about R Markdown or RMD Files and how they can be formatted and converted into reports for stakeholders.
- We've also explored the YAML header and the comments, descriptions, and explanations for the analysis shown in the report.
- Now comes the heart of an RMD File.
- The code.
- Code added to an RMD File is usually called a code chunk.
- We've shown you these code chunks in some of the RStudio sessions we've been running.
- You may have noticed code chunks if you've been practicing along with us.
- Now we'll show you what they're all about.
- Earlier, we worked with the PalmerPenguins dataset.
- We ran some code to analyze the data and create visualizations.
- After this step, we'd probably want to set up a practice report with notes about our analysis.
- We'll do that here and incorporate some code and visuals.
- Let's start by opening up RStudio and then the script with R programming.
- The GGplot_hook file.
- We could share this file directly with others, but it's not very effective.
- It's hard to read and doesn't always include any takeaways so we'll create a new.
- Rmd file instead.
- We'll add a title and author.
- Now we have two tabs in our script pane.
- We can toggle between them.
- Just like with browser tabs.
- We'll save our new.
- Rmd file.
- This file is in the template format.
- We'll delete everything except the header section and start our own.
- We already set up the header section.
- We don't need to make any changes there.
- Instead of deleting, we could make edit section by section.
- Adding our own comments and code along the way.
- But deleting the file contents gives us a blank space to work in and helps us avoid potential errors from mixing our own comments and code with the pre-existing ones in the template.
- Before we add any code, we want to describe its purpose.
- The first code chunk, we'll set up our R environment by loading our packages using the library function.
- On a new line, we'll type two hashtags to format a header for this section, followed by the header text setting up my environment.
- Then we'll add a note about the code.
- We've added apostrophes before and after tidyverse and palmerpenguins because they're the names of the packages which makes them part of the actual code.
- Now we'll add our code.
- RStudio has a handy code menu that we can use to insert a code chunk.
- There's also a button in our script pane that lets us add code chunks.
- This creates a gray section in our file and chunk delimiters.
- A delimiter is a character that indicates the beginning or end of a data item.
- You could also type these delimiters directly in the file.
- Three backticks, followed by an r in braces to begin the code chunk and three backticks to end it.
- Or you could use the keyboard shortcuts, Control plus Alt plus I on a PC or Chromebook, and Command plus Option plus I on a Mac.
- Since we're in RStudio, the code menu works just fine.
- Inside the first brace, we'll label our code chunk.
- After the R we'll add a space and then type loading packages.
- This adds another layer to our organization.
- We can now easily find this code chunk and its label using the contents menu at the bottom of our script pane.
- Next, between our delimiters, we'll add our first code chunk, which we use to load our two packages.
- Even if they're already loaded, loading them again make sure that our packages will be updated to the latest version.
- We can type starting on the line after the first delimiter.
- But since we also have our programming file available, we'll copy and paste from there.
- Now we can run our code right in the file to check it for errors.
- There's the code output.
- We can also change our code chunk options.
- There's options for changing the output and for turning off warnings and messages.
- These are useful for when you're ready to create a final report for stakeholders.
- You'll have control over what you'll show them in the report.
- For example.
- if you get warnings with your output that don't impact your findings, you can turn off the warnings for stakeholders.
- So the code chunks are the key to making this report a good learning tool and eventually a document worth presenting to stakeholders.
- When you have code embedded in a file and can show its output, you can provide evidence for your findings and share your sources.
- If you need more evidence for how R Markdown can help you document your analysis we've got it coming next.
- See you then.

## Question & Notes

- **Delimiter**: a character that indicates the beginning or end of a data item
- Code chunk keyboard shortcut:
  - PC/Chrome book: `Ctrl + alt + I`
  - Mac: `command + option + I` (Window + alt + I)

### Practice along the video

If you would like to follow along with the video, then complete the steps below to access the ggplot_hook.R file:

To start, log into your RStudio (Posit) Cloud account in a new tab. Open the project that you have been working with [this link](https://posit.cloud/content/6208304).

If you haven't gone through this process already, at the top right portion of the screen you will see a "red stamp" indicating this project as a Temporary Copy.

Click on the adjacent button, Save a Permanent Copy, and the project will be saved in your main dashboard for use with future lessons.

Once that is completed, navigate to the file explorer in the bottom right and click through to access the R script file: `Course 7 -> Week 5 -> ggplot_hook.R`

OR [ggplot_hook.R](./resources/ggplot_hook.R)

Once opened, you may follow along with the rest of the video to create an R Markdown (.rmd) file for sharing purposes.

**Note**: You may have noticed that the instructor had created an .html version from the R Markdown document for sharing purposes.

In order to generate a highly structured and quality R Markdown document, you may want to review the video lecture on [Structure of markdown](https://www.coursera.org/learn/data-analysis-r/lecture/ix21Z/structure-of-markdown-documents) documents  before moving to the next activity.

### Question 1: Fill in the blank: Code added to a(n)  _____ file is usually called a code chunk

- [x] rmd
- [ ] markdown
- [ ] HTML
- [ ] data

> Correct: Code added to a .rmd file is usually called a code chunk.

### Question 2: A data analyst writes in a code chunk and puts three backticks at the end of their code to mark the end of the data item. What are these backticks?

- [x] Delimiter
- [ ] Inline code
- [ ] YAML
- [ ] Metadata

> Correct: The delimiter is a character that indicates the beginning or end of a data item. In RMarkdown, ```{r } and ``` can be used as delimiters for code chunks.  
