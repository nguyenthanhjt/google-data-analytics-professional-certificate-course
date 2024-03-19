# Video: Welcome to the `tidyverse`

Video transcript

- Welcome back.
- As we discussed earlier, packages are a big part of what makes R so great.
- Packages offer a helpful combination of code, reusable R functions, descriptive documentation, tests for checking operability, and sample data sets.
- And for lots of data analysts, at the top of the list of useful packages is tidyverse.
- Tidyverse is actually a collection of packages in R with a common design philosophy for data manipulation, exploration, and visualization.
- Using tidyverse can help you work your way through pretty much the entire data analysis process.
- The packages in tidyverse work together naturally.
- I started learning about tidyverse when I was working on a survey project.
- It felt like I was stepping into a more advanced zone of R.
- I understood the basics, but now I was finding out how the tidyverse improves on the basics.
- That's when I got even more excited about working in R.
- I realized that the more I put into learning about the tidyverse, the more I get out of it.
- On top of that, the community support for tidyverse is strong too.
- It's one of the reasons why tidyverse is considered a key part of programming for most R users.
- The principles associated with tidyverse, which you'll learn both here and at your job, have been widely adopted by the R community.
- You'll find lots of tutorials and examples related to the tidyverse online that show you these principles and how they're applied to data analytics.
- Okay, let's install the tidyverse.
- You can follow along on your own, using your RStudio cloud account.
- Check out the reading for more details.
- Earlier, you learned how to find Base R packages using the function install packages.
- To install packages like the tidyverse that aren't in Base R, we'll use the install packages function.
- As we discussed earlier, this function calls the tidyverse and other packages from CRAN.
- Let's talk about why CRAN was created.
- Since packages not in Base R are mostly made by R users, people need a reliable way to check and validate submitted code.
- CRAN makes sure any R content open to the public meets the required quality standards.
- So, if it's sourced through CRAN, you can feel good that the package is authentic and valid.
- Another major source of packages and other R content is GitHub.
- Now, we'll get back to installing the tidyverse.
- We'll first type install.
-packages.
- Then, between the parentheses, we'll type tidyverse in quotes.
- The quotes aren't always necessary, but best practice is to use quotes to make sure that we are accurate.
- We'll press Enter and wait for RStudio to install tidyverse.
- When we click on our packages tab, we come across a lot of new packages on the list.
- That's tidyverse.
- You might have noticed that none of the packages are checked off.
- We need to load them first before we can use them.
- But that's a mighty long list.
- So, let's just load the package named tidyverse for now, using the library function.
- The return shows that not only was tidyverse loaded, but eight other packages were too.
- It also shows a list of conflicts.
- Conflicts happen when packages have functions with the same names as other functions.
- Basically, the last package loaded is the one whose functions will be used, so we'll stick with the tidyverse functions.
- But it's important to note that these messages only appear once.
- So, as you get more used to R, you'll be able to figure out if you want to use certain functions over others.
- The loaded packages are ggplot2, tibble, tidyr, readr, purrr, dplyr, stringr, and forcats.
- These packages are the core of the tidyverse because you'll use them in almost every analysis.
- All of them work together to make your data analysis smooth and efficient.
- With these packages, tidyverse helps you do everything from importing and transforming data to exploring and visualizing it.
- We'll check out this core of packages soon, and we'll use them even more as we continue working in RStudio.
- If you're working on your own in R, you can check out some of the other packages too.
- The packages available in tidyverse change a lot, but you can always check for updates by running tidyverse_update() in your console.
- You can then update the packages in a couple of ways.
- If you use the update packages function, it'll update all of your packages.
- That might take a while.
- So, if you just want to update one package, you can use the install packages function again with the package name as your argument in parentheses.
- You should update packages regularly to make sure you've got the latest version in your code.
- Conflict notifications are just one type of message that can show up in the console.
- You might find warnings and error messages as well.
- A quick search using the help tab will usually tell you what the message means and what, if anything, you'll need to do to address it.
- Coming up, we'll keep moving through the tidyverse.
- You'll find out more about why tidyverse is such an integral part of R.
- See you.

## Question & Notes

- Packages offer a helpful combination of code, reusable R functions, descriptive documentation, tests for checking operability, and sample data sets
- **Tidyverse (R)**: A system of packages in R with a common design philosophy for data manipulation, exploration, and visualization.
- **Conflict**: happen when packages have functions with the same names as other functions
- 8 core tidyverse packages:
  - gglot2
  - tibble
  - tidyr
  - readr
  - purr
  - dplyr
  - stringr
  - forcats
- `Update.packages()`: update all packages
- `Install.packages("package-name")`: update a specific package

### Question 1: Tidyverse is a collection of packages in R with a common design philosophy

- [x] True
- [ ] False

> Tidyverse is a collection of packages in R with a common design philosophy. The tidyverse packages are especially useful for data manipulation, exploration, and visualization.