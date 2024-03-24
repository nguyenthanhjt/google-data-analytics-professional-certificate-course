# Reading: Output formats in R Markdown

You can save this reading for future reference. Feel free to download a PDF version of this reading below:

[Ouput formats available in RMarkdown.pdf](https://d3c33hcgiwev3.cloudfront.net/HMmvfrAKSl6Jr36wCjpejg_f7ff98b532974cfca3bdea0be6731e4f_Output-formats-available-in-RMarkdown.pdf?Expires=1711411200&Signature=QXAeayWrlLAmB4DHPb-PhuGaNa8q5ocqO4Hrm7b0VtS16xyHiWufQQocQkxggkmKgKnEtGESXg59~V3U1EH39sCkAvlT8Ar8eRSCZm6kzc-eVO4l0CwjK-z-8zgEVIXBSadq0rnh0VKr1exlHpZx1coqH9WT1uJ-OtBNvn35Q8E_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

OR download [here](./resources/Output-formats-available-in-RMarkdown.pdf)

This reading will explore the different types of output formats you can produce with R Markdown.

## Setting the output of an R Markdown document

When working in RStudio, you can set the output of a document in R Markdown by changing the YAML header.

For example, the following code creates an HTML document:

```yaml
---
title: "Demo"
output: html_document
---
```

And the following code creates a PDF document:

```yaml
---
title: "Demo"
output: pdf_document
---
```

The Knit button in the RStudio source editor renders a file to the first format listed in its output field (HTML is the default). You can render a file to additional formats by clicking the dropdown menu next to the knit button.

## Available document outputs

In addition to the default HTML output (html_document), you can create other types of documents in R Markdown using the following output settings:

- `pdf_document`: This creates a PDF file with LaTeX (an open-source document layout system). If you don’t already have LaTeX, RStudio will automatically prompt you to install it.
- `word_document`: This creates a Microsoft Word document (.docx).
- `odt_document`: This creates an OpenDocument Text document (.odt).
- `rtf_document`: This creates a Rich Text Format document (.rtf).
- `md_document`: This creates a Markdown document (which strictly conforms to the original Markdown specification)
- `github_document`: This creates a GitHub document which is a customized version of a Markdown document designed for sharing on GitHub.

For a detailed guide to creating different types of R Markdown documents, check out the [Documents chapter in R Markdown: The Definitive Guide](https://bookdown.org/yihui/rmarkdown/documents.html).

## Notebooks

A notebook (`html_notebook`) is a variation on an HTML document (`html_document`). Overall, the output formats are similar; the main difference between them is that the rendered output of a notebook always includes an embedded copy of the source code.

Notebooks and HTML documents also have different purposes. HTML documents are good for communicating with stakeholders. Notebooks are better for collaborating with other data analysts or data scientists.

To learn more, check out the section on [Notebooks](https://rmarkdown.rstudio.com/lesson-10.html) in the R Markdown documentation.

## Presentations

You can also use R Markdown to produce presentations. Automatically inserting the results of your R code into a presentation can save you lots of time.

R Markdown renders files to specific presentation formats when you use the following output settings:

- `beamer_presentation`: for PDF presentations with beamer
- `ioslides_presentation`: for HTML presentations with ioslides
- `slidy_presentation`: for HTML presentations with Slidy
- `powerpoint_presentation`: for PowerPoint presentations
- `revealjs::revealjs_presentation`: for HTML presentations with reveal.js (a framework for creating HTML presentations that requires the reveal.js package)

To learn more, check out the section on [Slide Presentations](https://rmarkdown.rstudio.com/lesson-11.html) in the R Markdown documentation.

## Dashboards

Dashboards are a useful way to quickly communicate a lot of information. The [`flexdashboard`](https://github.com/rstudio/flexdashboard) package lets you publish a group of related data visualizations as a dashboard. Flexdashboard also provides tools for creating sidebars, tabsets, value boxes, and gauges.

To learn more, visit the [flexdashboard for R](https://rmarkdown.rstudio.com/flexdashboard/) page and the [Dashboards](https://rmarkdown.rstudio.com/lesson-12.html) section in the R Markdown documentation.

## Shiny

Shiny is an R package that lets you build interactive web apps using R code. You can embed your apps in R Markdown documents or host them on a webpage.

To call Shiny code from an R Markdown document, add `runtime: shiny` to the YAML header:

```yaml
---
title: "Shiny Web App"
output: html_document
runtime: shiny
---
```

To learn more about Shiny and how to use R code to add interactive components to an R Markdown document, check out the [Shiny tutorial](https://shiny.rstudio.com/tutorial/) from RStudio.

## Other formats

Other packages provide even more output formats:

- The [`bookdown`](https://github.com/rstudio/bookdown) package is helpful for writing books and long-form articles.
- The [`prettydoc`](https://github.com/yixuan/prettydoc/) package provides a range of attractive themes for R Markdown documents.
- The [`rticles`](https://github.com/rstudio/rticles) package provides templates for various journals and publishers.

Visit the [RStudio Formats](https://rmarkdown.rstudio.com/formats.html) page in the R Markdown documentation for a more comprehensive list of output formats and packages.

## Additional resources

For more information, check out these additional resources:

- The [R Markdown gallery](https://rmarkdown.rstudio.com/gallery.html) from RStudio has tons of examples of the outputs you can create with R Markdown.
- The [R Markdown Formats chapter](https://r4ds.had.co.nz/r-markdown-formats.html) in the R for Data Science book provides more details about the output formats introduced in this reading. This reading was compiled from information in this book.
