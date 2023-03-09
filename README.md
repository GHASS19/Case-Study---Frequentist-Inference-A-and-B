# Frequentist-Inference

## Part A

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

4. Learning outcomes

Having completed this project notebook, you now have hands-on experience:

- Sampling and calculating probabilities from a normal distribution
- Identifying the correct way to estimate the standard deviation of a population (the population parameter) from a sample
- Sampling distribution and now know how the Central Limit Theorem applies
- How to calculate critical values and confidence intervals
