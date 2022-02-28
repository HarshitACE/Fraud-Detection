# Fraud-Detection

## What is Benford's Law? 

Benford's law states that the frequency of occurance of the leading digits in a naturally occuring numerical distribution is predictable and non-uniform but closer to a _power distribution law._ This was first noticed by Newcomb in 1881 when he noticed the pattern in the numbers in the log book. Where the pages in front were much more worn than the latter pages. This showed him that is why the leading digit is much more likely to be small than large. 

The probablity of the digits are given by the following formula: 
$$ Pr(D1 = d) = \log10(1 + 1/d) $$ 

Benford's Law is used to model demographic growth , financial indexes and any Benford Dataset. \\

## How is it used in _Fraud Detection_? 
This is one of the most important and popular application of modelling using Benford's law. This works on the principal given as follows: 
> Manipulated or fraudulent data do not tend to confirm to Benford's Law, whereas unmanipulated data do. 

In general we can say that Benford's Law is the **Distribution of Distributions.**

### Applying Benford's Law
Those subjects are financial and accounting data harmonize to naturally existing numbers. If we assume that someone owns a stock mutual fund with a value of $1,000. For his fund to arrive $2,000 in rate, it would have to double by growing 100%. Apart from that, to further grow from $2,000 to $3,000, it would only need to increase it by 50%. As we previously mentioned for the first digit to be a 4, it needs to grow by another 33%. As Benford’s law predicts, for the leading digit 1 to become 2, there needs to be more growth than for the 3 to become 4, and so on. The fact that a Benford distribution is a “distribution of distributions,” financial projects have a tendency to comfort.

## Scope of this Project
We are going to see the fraud detection aspect of Benford's law in action using the following 2 cases: 
1. American Presidential Elections, 2016
2. Russian Presidential Elections, 2018

### Assumptions
1. The numbers need to be random and not assigned, with no imposed minimums or maximums. 
2. The numbers should cover several orders of magnitude, and the dataset should be large; recommendations suggests for 100 to 1000 samples in a data set at a minimum. But we have seen Benford’s law holding true for data with as little as 50 samples. 

### Chi-Square Test
The goodness of fit test that it is commonly used in order to make the simulation with Benfardw’s Law is the Chisquare test, which is a frequently used method that determines if an empirical (observed) distribution differs significantly from a theoretical (expected) distribution. Let us assume the null Hypothesis :
$$ H_0 : \text{observed and theoretical distributions are the same}$$
A significance level (p-value) is used is 0.05.
