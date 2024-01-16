# A Gentle Introduction to Statistical Power and Power Analysis in Python

> by Jason Brownlee on April 24, 2020 in Statistics

The statistical power of a hypothesis test is the probability of detecting an effect, if there is a true effect present to detect.

Power can be calculated and reported for a completed experiment to comment on the confidence one might have in the conclusions drawn from the results of the study. It can also be used as a tool to estimate the number of observations or sample size required in order to detect an effect in an experiment.

In this tutorial, you will discover the importance of the statistical power of a hypothesis test and now to calculate power analyses and power curves as part of experimental design.

After completing this tutorial, you will know:

- Statistical power is the probability of a hypothesis test of finding an effect if there is an effect to be found.
- A power analysis can be used to estimate the minimum sample size required for an experiment, given a desired significance level, effect size, and statistical power.
- How to calculate and plot power analysis for the Student’s t test in Python in order to effectively design an experiment.

**Kick-start your project** with my new book Statistics for [Machine Learning](https://machinelearningmastery.com/statistics_for_machine_learning/), including *step-by-step tutorials* and the *Python source code* files for all examples.

Let’s get started.

## Tutorial Overview

This tutorial is divided into four parts; they are:

1. Statistical Hypothesis Testing
2. What Is Statistical Power?
3. Power Analysis
4. Student’s t Test Power Analysis

## Statistical Hypothesis Testing - Kiểm đinh giả thuyết thống kê

A statistical hypothesis test makes an assumption about the outcome, called the null hypothesis.

For example, the null hypothesis for the Pearson’s correlation test is that there is no relationship between two variables. The null hypothesis for the Student’s t test is that there is no difference between the means of two populations.

The test is often interpreted using a p-value, which is the probability of observing the result given that the null hypothesis is true, not the reverse, as is often the case with misinterpretations.

p-value (p): Probability of obtaining a result equal to or more extreme than was observed in the data.
In interpreting the p-value of a significance test, you must specify a significance level, often referred to as the Greek lower case letter alpha (a). A common value for the significance level is 5% written as 0.05.

The p-value is interested in the context of the chosen significance level. A result of a significance test is claimed to be “statistically significant” if the p-value is less than the significance level. This means that the null hypothesis (that there is no result) is rejected.

p <= alpha: reject H0, different distribution.
p > alpha: fail to reject H0, same distribution.
Where:
Significance level (alpha): Boundary for specifying a statistically significant finding when interpreting the p-value.
We can see that the p-value is just a probability and that in actuality the result may be different. The test could be wrong. Given the p-value, we could make an error in our interpretation.

There are two types of errors; they are:

Type I Error. Reject the null hypothesis when there is in fact no significant effect (false positive). The p-value is optimistically small.
Type II Error. Not reject the null hypothesis when there is a significant effect (false negative). The p-value is pessimistically large.
In this context, we can think of the significance level as the probability of rejecting the null hypothesis if it were true. That is the probability of making a Type I Error or a false positive.

What Is Statistical Power?