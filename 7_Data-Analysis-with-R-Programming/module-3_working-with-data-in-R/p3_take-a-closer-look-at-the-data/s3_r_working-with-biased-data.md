# Working with biased data

## Addressing biased data with R

![A woman is standing, holding a speech bubble. Several other speech bubbles are on the ground near her.](./resources/img-1.png)

This scenario was shared by a quantitative analyst who collects data from people all over the world. They explain how they discovered bias in their data, and how they used R to address it:

“I work on a team that collects survey-like data. One of the tasks my team does is called a side-by-side comparison. For example, we might show users two ads side-by-side at the same time. In our survey, we ask which of the two ads they prefer. In one case, after many iterations, we were seeing consistent bias in favor of the first item. There was also a measurable decrease in the preference for an item if we swapped its position to second.

So we decided to add randomization to the position of the ads using R. We wanted to make sure that the items appeared in the first and second positions with similar frequencies. We used `sample()` to inject a randomization element into our R programming. In R, the `sample()` function allows you to take a random sample of elements from a data set. Adding this piece of code shuffled the rows in our data set randomly. So when we presented the ads to users, the positions of the ads were now random and controlled for bias. This made the survey more effective and the data more reliable.”

## Key takeaways

The `sample()` function is just one of many functions and methods in R that you can use to address bias in your data. Depending on the kind of analysis you are conducting, you might need to incorporate some advanced processes in your programming. Although this program won’t cover those kinds of processes in detail, you will likely learn more about them as you get more experience in the data analytics field. 

## Additional resources

- [**Bias function**](https://www.rdocumentation.org/packages/SimDesign/versions/2.2/topics/bias): This web page is a good starting point to learn about how the bias function in R can help you identify and manage bias in your analysis.

- [**Data Science Ethics**](https://datasciencebox.org/02-ethics.html): This online course provides slides, videos, and exercises to help you learn more about ethics in the world of data analytics. It includes information about data privacy, misrepresentation in data, and applying ethics to your visualizations.