# Frequentist-Inference

# Part A

## 1. Learning objectives

- the z-statistic
- the t-statistic
- the difference and relationship between the two
- the Central Limit Theorem, including its assumptions and consequences
- how to estimate the population mean and standard deviation from a sample
- the concept of a sampling distribution of a test statistic, particularly for the mean
- how to combine these concepts to calculate a confidence interval

## 2. An introduction to sampling from the normal distribution

In this section, you've been introduced to the scipy.stats package and used it to draw a small sample from the standard normal distribution. You've calculated the average (the mean) of this sample and seen that this is not exactly equal to the expected population parameter (which we know because we're generating the random variates from a specific, known distribution). You've been introduced to two ways of calculating the standard deviation; one uses n in the denominator and the other uses n-1 (Bessel's correction). 

## 3. Sampling distributions

Let's imagine we live in a town of 50,000 people and we know the height of everyone in this town. We will have 50,000 numbers that tell us everything about our population. We'll simulate these numbers now and put ourselves in one particular town, called 'town 47', where the population mean height is 172 cm and population standard deviation is 5 cm.

![image](https://user-images.githubusercontent.com/86930309/223910675-7ab3d51c-30e8-4351-98c6-8f584631815f.png)

Now we will randomly sample 10 people to measure.

![image](https://user-images.githubusercontent.com/86930309/223910873-9da7135a-720a-4446-b39a-f9398eb1efa8.png)

Lets do a random trial every day for a year, calculating the mean of each daily sample of 10.

![image](https://user-images.githubusercontent.com/86930309/223911152-75349868-d18c-4520-9453-8e61f1cc488f.png)

This is a year's worth of samples but for a sample size of 50.

## 4. Learning outcomes

Having completed this project notebook, you now have hands-on experience:

- Sampling and calculating probabilities from a normal distribution
- Identifying the correct way to estimate the standard deviation of a population (the population parameter) from a sample
- Sampling distribution and now know how the Central Limit Theorem applies
- How to calculate critical values and confidence intervals

# Part B

## Hospital Medical Charges

## 1. Imagine that a hospital has hired you as their data scientist. An administrator is working on the hospital's business operations plan and needs you to help them answer some business questions.

## 2. In this assignment notebook, you're going to use frequentist statistical inference on a data sample to answer the questions:

- Has the hospital's revenue stream fallen below a key threshold?
- Are patients with insurance really charged different amounts than those without?


![image](https://user-images.githubusercontent.com/86930309/223912716-d3e884c5-9baa-46cf-8042-8b2bf25f3805.png)

## 3. This frequency distribution shows that a majority of the charges are below the mean and there are a few outliners that are very high at $60,000.

## 4. The administrator is concerned that the actual average charge has fallen below 12,000, threatening the hospital's operational model. On the assumption that these data represent a random sample of charges, how would you justify that these data allow you to answer that question? And what would be the most appropriate frequentist test, of the ones discussed so far, to apply?

Here we would use a one sided interval since we are concerned if the the average charge has fallen below a single value of 12,000. We need to t-test the assumption that the average charge has gone down below 12,000.

## 5. Given the nature of the administrator's concern, what is the appropriate confidence interval in this case? A *one-sided* or *two-sided* interval? Calculate the critical value and the relevant 95% confidence interval for the mean, and comment on whether the administrator should be concerned.

We need to use a one-sided interval since we are trying to find a single number, (12,000) where the true mean is greater or less than 12,000 using a 95% confidence interval.

## 6. State the null and alternative hypothesis here:

We are assuming that the variances of the two groups are the same. That people are charged the same with insurance and without it

## 7. look through the documentation for statistical test functions in scipy.stats. You'll see the above t-test for a sample, but can you see an equivalent one for performing a z-test from a sample? Comment on your answer.

A:__There is no equivalent for performing a Z-test from a sample. Z-test are for populations. A Z-test determines if two population means are not the same, the sample size is big and when we know the variances.

## 8. Learning outcomes

Having completed this project notebook, you now have good hands-on experience:

- Using the central limit theorem to help you apply frequentist techniques to answer questions that pertain to very non-normally distributed data from the real world
- Performing inference using such data to answer business questions
- Forming a hypothesis and framing the null and alternative hypotheses
- Testing this using a t-test
