# Video: Structure of markdown documents

Video transcript

- Hello there. Earlier, we showed you how to get started using R markdown.
- We created a Markdown document called an RMD file, which is super useful for making and saving a final report that summarizes your data exploration and analysis findings.
- In this video, we'll check out the structure of the text in an RMD file and how you could format it to better organize and emphasize your findings.
- Let's go into RStudio and open the file we saved earlier called R Markdown Intro.
- If you're working along with us and don't have a file saved, you can open up a new R Markdown or RMD file using the file menu.
- If you're prompted to install packages, go ahead and click Yes.
- Click Okay to open with the default options and then save your file.
- Now let's dig deeper into this file. We'll start at the top. This is the YAML header section.
- YAML is a language for data that translates it, so it's readable.
- Fun fact: YAML originally stood for yet another markup language.
- This section is called out using three dashes on the first and last lines.
- This syntax automatically creates the YAML header section when it's used in an RMD file.
- In an RMD file, this section's basically for metadata or the data about the data in the rest of the file.
- The title, author, date and file type of an output are automatically included when you create a new file.
- There's lots of different functions and formatting options in this section.
- For now, just make sure you have at least the four details we've got in our file now.
- You can use the template that appears when you open the file and just edit over it.
- Or you can start from scratch using the three dashes to create the YAML section and the rest of the content in the file.
- We'll cover these steps over the next few videos and in the other program resources.
- Next, let's check out the text in the white areas of our file.
- Think of the text as a way to comment on and explain your code and analysis and any visualizations you're including.
- You can format the text to include links, ordered lists, equations and more.
- The text is formatted using Markdown, the syntax we introduced earlier.
- We've included a reading that shows you all of the ways to format text, as well as lots of other great Markdown tips and tricks.
- You'll also learn some more formatting examples in the next video.
- For now, let's try some examples that are in this file.
- On line 12, there's two hashtags and a space before the words R Markdown.
- Hashtags are used for headers.
- The more hashtags, the smaller the header.
- The space is important as well.
- Otherwise RStudio won't recognize that this is a header.
- Let's knit our file again.
- There's the R Markdown header in the HTML file.
- If we add two more hashtags in the dot RMD file and click knit once again, the output changes.
- The header's now smaller.
- We'll change it back because the original format made sense.
- Since this header is introducing information about R Markdown that comes in the next two paragraphs, we want to emphasize it.
- In the first paragraph of this section, there's a brief summary of Markdown.
- There's a link in the text, and it's formatted using angle brackets.
- Using these brackets results in a clickable link in the output.
- That's a handy feature if you want to refer to any helpful links or include them as sources for your analysis.
- In the next paragraph, knit is set off with two asterisks on either side of the word.
- This bolds the word.
- Using one asterisk on either side would instead italicize the word.
- Let's scroll down to the last paragraph.
- Here we've got some in-line code, which can be inserted directly into the text of a dot RMD file.
- The code appears in a gray box like the code chunks we'll talk about soon.
- Using in-line code like this lets you refer to the code directly as you explain it.
- Let's knit our file one more time.
- All the formatting works together to make a well designed, readable file that's easy to share with stakeholders and team members.
- That's it for now.
- But there's lots more to learn about creating your own reports.
- Stay tuned.

## Questions & Notes​

- **YAML**: a language for data that translates it so it's readable (originally stood for yet another markup language)

### Question 1: A data analyst wants to make one of the headers in their R Markdown document smaller. What should they include in the markdown text to do this?

- [ ] Spaces
- [x] Hashtags
- [ ] Semicolons
- [ ] Backticks

> Correct: Hashtags are used for headers; the more hashtags, the smaller the header.

### Question 2: A data analyst inserts some code directly into their R Markdown file so that they can refer to it directly in their write-up. What is this called?

- [ ] YAML header
- [ ] R notebook
- [x] Inline code
- [ ] Markdown

> Correct: Inline code can be inserted directly into the text of an .rmd file.

## My wrapped keypoints

- **Opening the R Markdown File**: We begin by opening the R Markdown file we previously saved, named "R Markdown Intro," in RStudio. If you don't have a file saved, you can create a new one using the file menu and save it accordingly.

- **Understanding YAML Header**: The YAML (YAML Ain't Markup Language) header section is the first part of the R Markdown file enclosed by three dashes at the beginning and end. It contains metadata such as the title, author, date, and output format. This section provides essential information about the document.

- **Text Formatting with Markdown**: The main body of the R Markdown file consists of white areas where text can be formatted using Markdown syntax. Markdown allows for various formatting options like headers, links, lists, and equations, making the text more readable and organized.

- **Headers and Formatting**: Headers are created using hashtags (#), with more hashtags indicating smaller headers. The space after the hashtags is crucial for RStudio to recognize it as a header. We can customize the formatting to suit the document's structure and emphasize important sections.

- **Text Examples**: The video demonstrates formatting examples within the R Markdown file, such as creating clickable links using angle brackets and applying bold or italic styles to text using asterisks. In-line code can also be included within the text, displayed in a gray box for clarity.

- **Rendering the Document**: After making changes to the R Markdown file, we can render it to preview how it will look in the selected output format. This ensures that the formatting and content are correctly displayed, enhancing readability for stakeholders and team members.

- **Conclusion**: R Markdown files provide a structured and versatile way to document analysis findings, combining text, code, and visualizations in a single, easy-to-share document. Learning to utilize Markdown formatting effectively enhances the clarity and professionalism of the report.
