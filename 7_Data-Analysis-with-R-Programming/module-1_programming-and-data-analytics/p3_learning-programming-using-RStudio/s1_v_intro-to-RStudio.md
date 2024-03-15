# Video: Intro to RStudio

Video transcript

- Hey there.
- It's time to take our tour of RStudio.
- The examples we'll look at are from RStudio Cloud, but RStudio works in a similar way across all platforms.
- Feel free to use the platform that works best for you.
- Later on if you want to learn more, you'll find resources on how to download and install RStudio on your own device.
- RStudio's an IDE or integrated development environment.
- This means that RStudio brings together all the tools you might want to use in a single place.
- The R console which we explored earlier is one part of this environment.
- RStudio also includes an editor for writing code, and tools for managing your data and creating visuals.
- RStudio is built specifically for use with R.
- It'll help maximize your productivity as a data analyst.
- Data analysis is like driving a car.
- You can think of R and RStudio as different parts of this car.
- R is like the car engine.
- RStudio is kind of like the accelerator, the steering wheel, and dashboard all-in-one.
- It lets you tell the engine what to do and helps you get to where you want to go.
- Just as a speedometer and navigation system make driving much easier, RStudio's environment makes using R much easier.
- In an earlier reading, you learned how to access RStudio.
- So let's log into RStudio now and explore.
- The RStudio environment has four main windows called panes.
- Each pane helps you perform different functions.
- The first time you open RStudio, you'll see three panes.
- A fourth pane is hidden by default, but it's easy to open.
- Just click on File in the menu, then select New File and R Script.
- RStudio has lots of keyboard shortcuts.
- To learn more check out Keyboard Shortcuts Help.
- You can make the panes smaller or larger by clicking on the minimize or maximize buttons at the upper right of each pane.
- You can also click and drag the borders of the panes to adjust their size.
- Click on the Panes button for more feature options.
- Now that we've got all four panes open, let's explore each of them.
- We'll start on the lower left and move clockwise from there.
- You might recognize the R console from an earlier reading.
- As a quick refresher, the console is the place where you give commands to R.
- For example, we can tell R to show us a summary of the penguins data that we used in an earlier video to create visuals.
- You'll need to install and load the palmer penguins dataset if you haven't done so already.
- Above the console in the upper left is the source editor pane.
- You'll use the source editor when working with R Scripts.
- There are two main ways of writing code in RStudio: using the console or using the source editor.
- You can type commands directly into the console, but they'll be forgotten when you close your current session.
- As we've discussed, it's important to be able to reproduce and share all the steps of your analysis.
- If you save your script in the editor, you can access your work again at any time and show others how you did it.
- The source editor and the console also work together in RStudio.
- When you execute code in the editor, the code automatically appears in the console.
- If you're working on a long analysis, this makes it easy to execute the entire code all at once or run specific sections of it as you go along.
- Let's run some code in the editor and check it out.
- Pro tip: Always keep in mind that R is case-sensitive.
- Here we use a capital V for the View function.
- Next, let's go to the Environment pane in the upper right.
- Here you'll find all the data you currently have loaded and can easily organize and save it.
- For example if you import data from a spreadsheet, it'll be visible in the Environment pane.
- You can view each object in the Environment pane by clicking on it.
- You can also toggle between a List view and a Grid view.
- To the right of the Environment tab, you'll find the History tab.
- All your previous commands are saved here and they're easy to search and re-execute.
- You'll find the most recent line of code at the bottom of the list.
- You can copy any line to the command console by double-clicking it.
- In the lower right, you'll see a pane that has tabs for Files, Plots, Packages, and Help.
- The Files tab gives you access to your file directory and shows the contents of the current working folder.
- You can easily find and manage all your files and create new project folders.
- Next is the Plots tab.
- If we create a plot, the result appears here.
- For example, we can create a scatter plot with the penguins dataset we used earlier.
- You'll learn more about creating plots in RStudio later on.
- Earlier, we talked about R packages which are custom solutions to data problems developed by R users.
- RStudio gives you access to a library of R packages known as the tidyverse.
- You can upgrade, install, and manage your library in the Packages pane.
- Packages loaded in your current session have a check mark.
- Later on, we'll explore the tidyverse in more detail.
- Finally, click on the Help tab.
- Here you can find helpful resources for R and RStudio.
- There are tons of resources out there to help answer all your questions.
- Be sure to take advantage of them.
- That's our tour of RStudio.
- We're just scratching the surface of what RStudio can do.
- Soon you'll get to explore RStudio in more detail.
- Speaking as a data professional, I love working in RStudio.
- It makes my work so much easier, faster, and better.
- Congratulations on finishing another step in your data analyst learning journey.
- Coming up, we'll learn some basic programming concepts.
- Then we'll start working with R.
- For those of you who are new to programming, you're about to write your first lines of code.
- See you then.

## Questions & Notes

- Would you like to set up an RStudio account to follow along with the steps in this video?

Complete the next Hands-On Activity: [Cloud access to RStudio](./s2_pq_activity_cloud-access-to-RStudio.md), and then click Continue below to play the rest of this video.

- If you would like to preview or install the dataset used in this video, refer to the [palmerpenguins package](https://allisonhorst.github.io/palmerpenguins/) for the detailed information.

**Note**: At the point of **Plot tab**, you may not have installed the 'ggplot' package, which would normally allow you to generate a plot for the penguins data set.

In order for the upcoming plot algorithm to work first type and execute each line of the syntax below, which will install the 'tidyverse' package:

```r
install.packages("tidyverse")
library(tidyverse)

## ggplot
ggplot(data = penguins, aes(x=flipper_length_mm, y=body_mass_g))+geom_point(aes(color=species))
```

Once the above library is installed and loaded the ggplot syntax coming up next will successfully generate a plot.

You will have a much more in-depth exploration of ggplot parameters and other data visualizations in the upcoming video lecture, [Visualizations in R and tidyverse](../../module-4_more-about-visualizations-aesthetics-n-annotations/p1_create-data-visualizations-in-R/s2_v_visualization-basic-in-R-and-tidyverse.md)

### Question: In RStudio, you can execute code in both the R console pane and the source editor pane

- True
- False

> Correct: In RStudio, you can execute code in both the R console pane and the source editor pane.

## **Key Points:**

1. **RStudio Overview:**
   - RStudio is an integrated development environment (IDE) specifically built for use with R.
   - It consolidates all necessary tools for R programming into one interface, enhancing productivity for data analysts.
   - RStudio provides tools like the R console, source editor, and data management utilities.

2. **R Console:**
   - The R console is where commands are executed in R.
   - It allows users to interact directly with R, typing commands and receiving immediate responses.
   - Commands typed directly into the console are forgotten when the session ends, but they can be saved in scripts for future use.

3. **Source Editor:**
   - The source editor is used for writing and saving R scripts.
   - Scripts written in the source editor can be saved and accessed later, facilitating reproducibility and sharing of analyses.
   - Code executed in the editor automatically appears in the console, allowing for easy execution and debugging.

4. **Environment Pane:**
   - The environment pane displays all currently loaded data objects.
   - It provides a visual representation of the user's workspace, showing imported datasets and other objects.
   - Users can toggle between list and grid views and organize their data efficiently.

5. **History and Files Panes:**
   - The history pane stores previous commands, making them easily accessible for reuse.
   - The files pane allows users to navigate their file directory, manage files, and create new project folders within RStudio.

6. **Plots and Packages Panes:**
   - The plots pane displays graphical outputs generated by R code, such as plots and charts.
   - The packages pane provides access to R packages, including installation, management, and loading/unloading functionalities.

7. **Help Tab:**
   - The help tab offers access to resources for R and RStudio, including documentation, tutorials, and community forums.
   - Users can find answers to questions and seek assistance when encountering challenges in their R programming journey.

By familiarizing oneself with the RStudio environment and its various panes, data analysts can efficiently manage their workflow, write code, explore data, and create visualizations, enhancing their proficiency in R programming.
