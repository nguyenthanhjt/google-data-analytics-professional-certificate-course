# Video: Annotation Layer

Video transcript

- Hi. Great to have you back.
- Coming up we'll learn how to customize the look and feel of our plots using the label and annotate functions.
- In everyday language to annotate means to add notes to a document or diagram to explain or comment upon it.
- In ggplot 2 adding annotations to your plot can help explain the plot's purpose or highlight important data.
- When you present your data visuals to stakeholders, you may not have much time to meet with them.
- Labels and annotations will point their attention to key things and help them quickly understand your plot.
- Let's start with the label function.
- It's super useful for adding informative labels to a plot such as titles, subtitles, and captions.
- For example, we can add a title to our plot that shows the relationship between body mass and flipper length for the three penguin species.
- A title will clearly indicate the purpose of the plot.
- Let's go over the code.
- First, we add a plus sign to add a new layer to our plot.
- Next in the parentheses, following the label function, we write the word title, then an equal sign than the specific text we want in our title.
- Let's log into RStudio Cloud and check it out.
- First, let's load the ggplot2 package in the penguins dataset.
- Remember, put the plus sign at the end of a line of code.
- It's easy to forget.
- R automatically displays the title at the top of the plot.
- We can also add a subtitle to our plot to highlight important information about our data.
- To do this, we enter the code for a subtitle in the same way as a title.
- Remember to add a comma after the title argument before you enter your subtitle.R automatically displays the subtitle just below the title.
- We can add a caption to our plot in the same way.
- Captions let us show the source of our data.
- The palmer penguins data was collected from 2007 to 2009 by Dr.Kristen Gorman, a member of the Palmer Station Long Term Ecological Research program.
- Let's cite Dr.
- Gorman in our caption.
- R automatically displays the caption at the bottom right of our plot.
- Titles, subtitles, and captions are labels that we put outside of the grid of our plot to indicate important information.
- If we want to put text inside the grid to call out specific data points, we can use the annotate function.
- For example, let's say we want to highlight the data from the Gentoo penguins.
- We can use the annotate function to add some text next to the data points that refer to the Gentoos.
- This text will clearly communicate what the plot shows and reinforce an important part of our data.
- Okay, let's check out the code.
- In the parentheses of the annotate function, we've got information on the type of label, the specific location of the label and the context of the label.
- In this case, we want to write a text label.
- We also want to place it near the Gentoo data points.
- Let's put it at the following coordinates: x-axis equals 220 millimeters and y-axis equals 3,500 grams.
- Finally, let's write our text.
- The Gentoos are the largest.
- Let's run it.
- Check it out.
- R automatically places the text label on the correct coordinates in our plot.
- We can customize our annotation even more.
- Let's say we want to change the color of our text.
- Well, we can add color equals followed by the name of the color.
- Let's try purple.
- We can also change the font style and size of our text.
- Use font face and size to write the code.
- Let's bold our text and make it a little larger.
- We can even change the angle of our text.
- For example, we can tilt our text at a 25 degree angle to line it up with our data points.
- Let's try it.
- That looks great.
- By this point, our code is getting pretty long.
- If you want to use less code, you can store your plot as a variable in R.
- As a quick reminder to create a variable in R you type the variable name then a less than sign, followed by a dash.
- Let's try it with the variable name p.
- Now, instead of writing all the code again, we can just call p and add an annotation to it like this.
- You get the same result.
- Some people like to see every step of their code listed out in front of them.
- So there are advantages to doing it the longer way.
- It's really up to you.
- I just want you to know that you've got options.
- Hopefully, this gives you an idea of some of the ways you can customize your plots.
- Labels and annotations can be really helpful when it comes to highlighting important parts of your data and communicating key points.
- That's all for now.
- Coming up, you'll learn some useful ways to save your plots in ggplot2.
- See you next time.

## Questions & Notes

- **Annotate**: to add notes to a document or diagram to explain or commnent upon it
  - Title
  - Sub-title
  - Captions

```r
ggplot(data = penguins) +
  geom_point(mapping =  aes(x = flipper_length_mm, y = body_mass_g, color = species)) +
  labs(title =  "Palmer Penguins: Body mass vs Flipper Length")
```

### Question 1: What do the label and annotate functions do?

- [ ] Choose a geom  
- [ ] Load a dataset  
- [x] Customize the look and feel of your plots
- [ ] Display subsets of your data

> Correct: The label and annotate functions customize the look and feel of your plots.

## My wrapped keypoints

1. **Introduction to Annotation**: Annotations in ggplot2 are used to add notes or labels to a plot to explain or highlight important aspects of the data. This is particularly useful when presenting data visuals to stakeholders, as annotations can quickly draw attention to key points.

2. **Label Function**: The `label` function in ggplot2 is used to add informative labels to plots, such as titles, subtitles, and captions. Titles and subtitles are displayed outside the plot grid, while captions typically appear at the bottom right corner of the plot.

3. **Adding Titles, Subtitles, and Captions**: Users can add titles, subtitles, and captions to their plots using the `label` function. These labels provide context and information about the plot's purpose and data source.

4. **Annotate Function**: The `annotate` function in ggplot2 is used to add text or geometric objects inside the plot grid to highlight specific data points or patterns. Users can customize the appearance of annotations, including text color, font style, size, and angle.

5. **Customizing Annotations**: Annotations can be customized by specifying parameters such as text color, font style, size, and angle. Users can also adjust the position of annotations to align with specific data points or regions of interest.

6. **Storing Plots as Variables**: Users can store plots as variables in R, allowing them to reuse the plot without rewriting all the code. This can help simplify code and make it more efficient, especially for complex plots with multiple annotations.

7. **Options for Customization**: There are multiple ways to customize plots in ggplot2, and users have the flexibility to choose the approach that best suits their preferences and workflow. Whether it's listing out every step of the code or storing plots as variables, ggplot2 provides options for customization.

Annotations play a crucial role in enhancing the interpretability and visual appeal of plots, helping users effectively communicate key insights from their data to stakeholders.
