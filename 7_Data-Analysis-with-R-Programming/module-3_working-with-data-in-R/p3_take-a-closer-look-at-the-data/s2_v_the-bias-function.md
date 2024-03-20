# Video: The bias function

Video transcript

- Hey, welcome back.
- By now, you've already learned the importance of fair unbiased data in data analysis.
- In R, we can actually quantify bias by comparing the actual outcome of our data with the predicted outcome.
- There's a pretty complicated statistical explanation behind this.
- But with the bias function in R, we don't have to perform this calculation by hand.
- Basically the bias function finds the average amount that the actual outcome is greater than the predicted outcome.
- It's included in the sim design package.
- So it's helpful to install that and practice on your own.
- If the model is unbiased, the outcome should be pretty close to zero.
- A high result means that your data might be biased.
- A good thing to know before you analyze it.
- Let's say we're working with a local weather channel to determine if their weather predictions are biased.
- First we need to install and load a package called Sim design.
- We'll use the bias function to compare forecasted temperatures with actual temperatures.
- For this example we'll just take a small sample of our weather data and input them here.
- We'll label this the actual temp.
- Then, we'll put in the predictions.
- And then the bias function.
- When we run this we find out that the result Is 0.71.
- That's pretty close to zero but the prediction seemed biased towards lower temperatures which, means they aren't as accurate as they could be.
- And now that the local weather channel knows about this, they can find the problem in their system that's causing biased predictions.
- This doesn't mean that their predictions will be perfect all the time, but they'll be more accurate overall.
- Let's try another example, in this scenario we're working for a game store.
- The store has been keeping a record of how many copies of new games they sell on release day.
- They want to compare those numbers to their actual sales so that they could find out if they are ordering new stock according to their actual needs.
- Just like the previous example, we will start by inputting our sales data, will label that actual underscore sales and add the data points.
- Next will input the amount of stock they ordered as predicted underscore sales and then input those data points.
And now we have our data ready to go.
- As you learned in the first example the bias function compares the actual outcome and the predicted outcome of the data to determine the average amount the actual outcome is greater than the predicted outcome.
- An unbiased model should be close to zero.
- Let's run the bias function on our sales data now, like before we'll just type bias to start the function and then actual underscore sales and predicted underscore sales in the parentheses.
- When we press enter...
- Wow, the result is negative 35.
- That's pretty far from zero.
- The predicted outcome is larger than the actual outcome which means they may be ordering too much stock for release days.
- Now that they've used the bias function to compare these data points, they can reevaluate their stocking practices to avoid buying more stock than they need at once.
- And that's it for now.
- We've covered a lot together.
- We learned how to create data frames.
- We tried out some basic data cleaning functions.
- We got a little preview of how data viz in R can help us better understand our data.
- And finally we learned how to use the bias function.
- I've still got a lot more I want to tell you about R and if the data visualizations we created in this module, we're exciting for you, I've got great news.
- Coming up, we'll learn all about data viz in R, but first you've got a weekly challenge to tackle.
- I know you're going to do great.
- And if you want to review any of the material we've covered in these videos, feel free.
- This might be the first time you've encountered R so it's a great opportunity to practice something new.
- Your code might throw up some errors at first.
- That's just part of writing code.
- Learning from our mistakes is how we grow.
- I'll see you afterwards for our next adventure in R.

## Questions & Notes

```r
install.packages("SimDesign")

library(SimDesign)

# use bias function to compare forecasted temperatures with actual temperatures

actual_temp <- c(68.3, 70, 72.4, 71, 67, 70)
predicted_temp <- c(67.9, 69, 71.5, 70, 67, 69)
bias(actual_temp, predicted_temp) # [1] 0.7166667 -> close to zero

# Scenario: working for game store
# The store has been keeping a record of how many copies of new games they sell on release day.
# They want to compare those numbers to their actual sales so that they could find out if they are ordering new stock according to their actual needs.

actual_sales <- c(150, 203, 137, 247, 116, 287)
predicted_sales <- c(200, 300, 150, 250, 150, 300)
bias(actual_sales, predicted_sales) # -35 -> far from zero 
# -> predicted outcome is larger than actual outcome which means they may be ordering too much stock for release days
```

## My wrapped keypoints

In this section, titled "The bias function," the video introduces viewers to the concept of quantifying bias in data analysis using the bias function in R. Here's a breakdown of the key points from the video:

1. **Introduction to Bias Measurement:**
   - The video emphasizes the importance of fair and unbiased data in data analysis.
   - It introduces the concept of quantifying bias by comparing actual outcomes with predicted outcomes.

2. **Using the Bias Function:**
   - The bias function in R, included in the sim design package, automates the calculation of bias.
   - By comparing actual and predicted outcomes, the bias function determines the average amount by which the actual outcome exceeds the predicted outcome.

3. **Example Scenarios:**
   - Two example scenarios are provided to illustrate the application of the bias function:
     - Evaluating bias in weather predictions from a local weather channel.
     - Assessing bias in stock ordering practices for a game store based on release day sales.

4. **Interpreting Results:**
   - A result close to zero indicates minimal bias, while a high or low result suggests bias in the predictions.
   - Interpretation of results guides actions for improving prediction accuracy and reducing bias in future analyses.

5. **Conclusion and Next Steps:**
   - The video concludes by summarizing the topics covered, including creating data frames, basic data cleaning functions, and using the bias function.
   - Viewers are encouraged to embrace challenges and errors as part of the learning process, with anticipation for future lessons on data visualization in R.

Overall, the section highlights the practical application of the bias function in assessing and mitigating bias in data analysis, emphasizing its role in improving the accuracy and reliability of predictive models.