# Frequentist Inference: 

**Frequentist inference** is the process of deriving conclusions about an underlying distribution via the observation of data. In particular, you'll practice writing Python code to apply the following statistical concepts:

   * The z-statistic
   * The t-statistic
   * The difference and relationship between the two
   * The Central Limit Theorem, including its assumptions and consequences
   * How to estimate the population mean and standard deviation from a sample
   * The concept of a sampling distribution of a test statistic, particularly for the mean
   * how to combine these concepts to calculate a confidence interval
   * Calculating confidence intervals and p-values
   * Hypothesis testing
    

There are two parts to the case study: 
   * In part A, we’ll highlight the Pythonic implementation of the concepts underlying frequentist inference. 
   * In Part B, we’ll apply those implementations to a real-world scenario.    
   
   
## Sample & population:    

In general, the sample mean we calculate will not be equal to the population mean (as we saw above). A consequence of this is that the sum of squares of the deviations from the population mean will be bigger than the sum of squares of the deviations from the sample mean. In other words, the sum of squares of the deviations from the sample mean is too small to give an unbiased estimate of the population variance. An example of this effect is given here. Scaling our estimate of the variance by the factor  𝑛/(𝑛−1)  gives an unbiased estimator of the population variance. This factor is known as Bessel's correction. The consequence of this is that the  𝑛  in the denominator is replaced by  𝑛−1 .

## Standard Normal Distribution:

![Normal_Distribution](https://user-images.githubusercontent.com/67468718/104243194-11866980-5415-11eb-8d05-166649e01d15.JPG)


## Margin of Error:

#### The margin of error can be calculated after finding the values of:
  1. Critical value of the sample
  2. Standard Error of the sample 
  
**Margin of Error = Critical value * Standard Error**
  
Critical value of the sample can be calculated using below: 
  confidence level= 95% 

  1. Let's calculate alpha: by subtract 95% (confidence level) from 100%. That gives us 5% (0.05). This alpha level is the area in both of thesetails. What we are interested in is this critical value here, so we need to do a little more math.
  2. Divide Alpha by 2 and this gives (0.025), because we're only interested in the area for one tail, not the area for both tails. So this is the area in one tail, this 5% alpha level. 
  3. Subtract 0.025 from 1 (1-0.025 = 0.975): The reason we did this step is we're subtracting this area from 1 and that gives us all of this area to the left, and that means we can look up this critical value here in the z table. 
  4. By looking at the "z table" for an area of 97.5%. My area of 97.5%, that's .975 is going to fall in between: x-axis (0.05 - 0.06 = 0.055) and y-axis (1.9)
  5. So the **critical value is going to be 1.955 (Right)** and the **critical value is going to be -1.955 (left).**
  
Standard Error of the sample can be calculated using below:  
 
 Standard Error(Sample) = 𝜎 / sqrt(n)
 
## Confidence Interval :
Confidence Interval of the mean, can be calculated using: **population_mean ± margin_error**

## p-value :

The p-value is the probability of obtaining the observed results of a test, assuming that the null hypothesis is correct; a smaller p-value means that there is stronger evidence in favor of the alternative hypothesis.

## statistical power:

‘Statistical power’ refers to the power of a binary hypothesis, which is the probability that the test rejects the null hypothesis given that the alternative hypothesis is true.

## The statistical significance:

hypothesis testing to determine statistical significance:
  * State the null hypothesis and alternative hypothesis. 
  * Calculate the p-value, the probability of obtaining the observed results of a test assuming that the null hypothesis is true. 
  * Set the level of the significance (alpha) and if the p-value is less than the alpha, you would reject the null — in other words, the result is statistically significant.





