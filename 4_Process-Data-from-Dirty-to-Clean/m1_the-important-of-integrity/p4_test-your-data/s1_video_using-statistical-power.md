# Using statistical power

[VIDEO](./resources/s1_video_using-statistical-power.mp4) and [transcript](./resources/s1_video_using-statistical-power.txt)

- Hey, there.
- We've all probably dreamed of having a superpower at least once in our lives.
- I know I have.
- I'd love to be able to fly.
- But there's another superpower you might not have heard of: statistical power.
- Statistical power is the probability of getting meaningful results from a test.
- I'm guessing that's not a superpower any of you have dreamed about.
- Still, it's a pretty great data superpower.
- For data analysts, your projects might begin with the test or study.
- Hypothesis testing is a way to see if a survey or experiment has meaningful results.
- Here's an example.
- Let's say you work for a restaurant chain that's planning a marketing campaign for their new milkshakes.
- You need to test the ad on a group of customers before turning it into a nationwide ad campaign.
- In the test, you want to check whether customers like or dislike the campaign.
- You also want to rule out any factors outside of the ad that might lead them to say they don't like it.
- Using all your customers would be too time consuming and expensive.
- So, you'll need to figure out how many customers you'll need to show that the ad is effective.
- Fifty probably wouldn't be enough.
- Even if you randomly chose 50 customers, you might end up with customers who don't like milkshakes at all.
- And if that happens, you won't be able to measure the effectiveness of your ad in getting more milkshake orders since no one in the sample size would order them.
- That's why you need a larger sample size: so you can make sure you get a good number of all types of people for your test.
- Usually, the larger the sample size, the greater the chance you'll have statistically significant results with your test.
- And that's statistical power.
- In this case, using as many customers as possible will show the actual differences between the groups who like or dislike the ad versus people whose decision wasn't based on the ad at all.
- There are ways to accurately calculate statistical power, but we won't go into them here.
- You might need to calculate it on your own as a data analyst.
- For now, you should know that statistical power is usually shown as a value out of one.
- So if your statistical power is 0.6, that's the same thing as saying 60%.
- In the milk shake ad test, if you found a statistical power of 60%, that means there's a 60% chance of you getting a statistically significant result on the ad's effectiveness.
- "Statistically significant" is a term that is used in statistics.
- If you want to learn more about the technical meaning, you can search online.
- But in basic terms, if a test is statistically significant, it means the results of the test are real and not an error caused by random chance.
- So there's a 60% chance that the results of the milkshake ad test are reliable and real and a 40% chance that the result of the test is wrong.
- Usually, you need a statistical power of at least 0.8 or 80% to consider your results statistically significant.
- Let's check out one more scenario.
- We'll stick with milkshakes because, well, because I like milkshakes.
- Imagine you work for a restaurant chain that wants to launch a brand-new birthday cake flavored milkshake.
- This milkshake will be more expensive to produce than your other milkshakes.
- Your company hopes that the buzz around the new flavor will bring in more customers and money to offset this cost.
- They want to test this out in a few restaurant locations first.
- So let's figure out how many locations you'd have to use to be confident in your results.
- First, you'd have to think about what might prevent you from getting statistically significant results.
- Are there restaurants running any other promotions that might bring in new customers? Do some restaurants have customers that always buy the newest item, no matter what it is? Do some location have construction that recently started, that would prevent customers from even going to the restaurant?
- To get a higher statistical power, you'd have to consider all of these factors before you decide how many locations to include in your sample size for your study.
- You want to make sure any effect is most likely due to the new milkshake flavor, not another factor.
- The measurable effects would be an increase in sales or the number of customers at the locations in your sample size.
- That's it for now.
- Coming up, we'll explore sample sizes in more detail, so you can get a better idea of how they impact your tests and studies.
- In the meantime, you've gotten to know a little bit more about milkshakes and superpowers.
- And of course, statistical power.
- Sadly, only statistical power can truly be useful for data analysts.
- Though putting on my cape and flying to grab a milkshake right now does sound pretty good.

## Quiz

- Which statistical power is typically considered the minimum for statistical significance?
  - `0.8 (80%)`: A 0.8 or 80% statistical power is typically considered the minimum for statistical significance.
  - 0.5 (50%)
  - 0.9 (70%)
  - 0.6 (60%)

[A Gentle Introduction to Statistical Power and Power Analysis in Python](https://machinelearningmastery.com/statistical-power-and-power-analysis-in-python/)
sums it up nicely:

**Statistical power** can be calculated and reported for a completed experiment to comment on the confidence one might have in the conclusions drawn from the results of the study. It can also be used as a tool to estimate the number of observations or sample size required in order to detect an affect in an experiment.

**Optional:** If you want a more detailed explanation of statistical power and power analysis, the above link is a tutorial that also lists additional references.

## Keypoints

- Statistical Power Definition:
  - Statistical power is the probability of obtaining meaningful results from a test.
  - It is crucial for data analysts as it helps determine the effectiveness of surveys or experiments.
- Example Scenario - Milkshake Ad Test:
  - Hypothesis testing is applied to assess whether a marketing campaign (e.g., new milkshake ad) has meaningful results.
  - Using a representative sample size is essential to draw reliable conclusions.
- Sample Size Importance:
  - Larger sample sizes increase the likelihood of obtaining statistically significant results.
  - Statistical power is often measured on a scale from 0 to 1, representing the probability of reliable outcomes.
- Statistical Significance:
  - Statistically significant results indicate that the observed effects are real and not due to random chance.
  - A statistical power of at least 0.8 (80%) is typically desired for results to be considered statistically significant.
- Considerations for Sample Size:
  - Factors like diverse customer preferences or external influences must be considered to determine an appropriate sample size.
  - Measurable effects, such as increased sales or customer numbers, contribute to assessing statistical power.
- Calculation of Statistical Power:
  - Accurate calculation of statistical power involves complex statistical methods.
  - It is commonly represented as a percentage, indicating the chance of obtaining reliable results.