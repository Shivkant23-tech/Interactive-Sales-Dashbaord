# STATISTICS NOTES

Topics Covered:

1. Descriptive Statistics

2. Probability Distributions

3. Hypothesis Testing

4. Correlation and Covariance

5. Statistical Significance and P-values

6. Confidence Intervals and Margin of Error

7. DESCRIPTIVE STATISTICS
   =========================

Descriptive statistics are used to summarize and understand a dataset.

## A. Mean

The mean is the average value of a dataset.

Formula:
Mean = Sum of all values / Number of values

Example:
Data = 10, 20, 30, 40, 50

Mean = (10 + 20 + 30 + 40 + 50) / 5
Mean = 30

## B. Median

The median is the middle value when data is arranged in ascending or
descending order.

Example:
Data = 10, 20, 30, 40, 50

Median = 30

For an even number of observations, the median is the average of the
two middle values.

## C. Mode

The mode is the value that occurs most frequently in a dataset.

Example:
Data = 10, 20, 20, 30, 40

Mode = 20

## D. Standard Deviation

Standard deviation measures how spread out the data is around the mean.

A small standard deviation means the values are close to the mean.

A large standard deviation means the values are more spread out.

Example:
Dataset A = 48, 49, 50, 51, 52
Dataset B = 20, 35, 50, 65, 80

Dataset B has a larger standard deviation because its values are more
spread out.

2. PROBABILITY DISTRIBUTIONS
   ============================

A probability distribution describes how the possible values of a random
variable are distributed and how likely each value is.

Common probability distributions include:

## A. Normal Distribution

A normal distribution is a continuous probability distribution with a
bell-shaped curve.

Properties:

* Symmetric around the mean
* Mean = Median = Mode
* Approximately 68% of observations fall within 1 standard deviation
* Approximately 95% fall within 2 standard deviations
* Approximately 99.7% fall within 3 standard deviations

## B. Binomial Distribution

The binomial distribution describes the number of successes in a fixed
number of independent trials.

Example:

* Number of heads when a coin is flipped 10 times
* Number of successful customers out of 100 customers

## C. Poisson Distribution

The Poisson distribution models the number of events occurring within a
fixed interval of time or space.

Example:

* Number of customers arriving at a shop per hour
* Number of website requests per minute

Important Properties:

* Probability values range from 0 to 1.
* The total probability of all possible outcomes equals 1.

3. HYPOTHESIS TESTING FUNDAMENTALS
   ==================================

Hypothesis testing is a statistical method used to determine whether
there is enough evidence to support a claim about a population.

## A. Null Hypothesis (H0)

The null hypothesis represents the default assumption.

Example:
H0: There is no difference between two groups.

## B. Alternative Hypothesis (H1)

The alternative hypothesis represents the claim or difference being tested.

Example:
H1: There is a difference between two groups.

## C. General Steps

1. Define the research question.
2. State the null hypothesis.
3. State the alternative hypothesis.
4. Select a significance level (alpha).
5. Select an appropriate statistical test.
6. Calculate the test statistic and p-value.
7. Compare the p-value with alpha.
8. Draw a statistical conclusion.

Common Hypothesis Tests:

* Z-test
* T-test
* Chi-square test
* ANOVA
* Proportion tests

4. CORRELATION AND COVARIANCE
   =============================

## A. Correlation

Correlation measures the strength and direction of the relationship
between two variables.

Pearson correlation coefficient ranges from -1 to +1.

+1  = Perfect positive correlation
0  = No linear correlation
-1  = Perfect negative correlation

Example:
If study hours increase and exam scores also increase, the variables may
have a positive correlation.

IMPORTANT:
Correlation does not prove causation.

A strong correlation between two variables does not necessarily mean that
one variable causes the other.

## B. Covariance

Covariance indicates whether two variables tend to increase or decrease
together.

Positive covariance:
Both variables tend to increase together.

Negative covariance:
One variable tends to increase when the other decreases.

Covariance is useful for understanding the direction of a relationship,
while correlation is easier to compare because it is standardized between
-1 and +1.

5. STATISTICAL SIGNIFICANCE AND P-VALUES
   ========================================

A p-value helps determine how compatible the observed data is with the
null hypothesis.

General interpretation:

Small p-value:
There is stronger evidence against the null hypothesis.

Large p-value:
There is not enough evidence to reject the null hypothesis.

Common significance level:

Alpha = 0.05

Decision rule:

If p-value < 0.05:
Reject the null hypothesis.

If p-value >= 0.05:
Fail to reject the null hypothesis.

IMPORTANT:
A p-value is NOT the probability that the null hypothesis is true.

Statistical significance also does not automatically mean that an effect
is practically important. Effect size and the real-world context should
also be considered.

6. CONFIDENCE INTERVALS AND MARGIN OF ERROR
   ============================================

A confidence interval provides a range of plausible values for a
population parameter based on sample data.

Example:

Sample mean = 75
95% Confidence Interval = 72 to 78

This means the interval produced by the chosen confidence procedure is
72 to 78. Under repeated sampling, a 95% confidence interval procedure
would capture the true population parameter about 95% of the time.

Common Confidence Levels:

* 90%
* 95%
* 99%

## A. Margin of Error

The margin of error represents the amount of uncertainty around an
estimate.

For a simple confidence interval:

Confidence Interval = Estimate +/- Margin of Error

Example:

Estimated average = 100
Margin of error = 5

Confidence Interval:

100 +/- 5

Lower limit = 95
Upper limit = 105

Factors Affecting Margin of Error:

* Sample size
* Confidence level
* Variability in the data

Generally, increasing the sample size reduces the margin of error,
assuming other factors remain similar.

# PYTHON EXAMPLE

The following Python libraries can be useful for statistical analysis:

import pandas as pd
import numpy as np
from scipy import stats

Example Dataset:

data = [10, 20, 20, 30, 40, 50]

Mean:

np.mean(data)

Median:

np.median(data)

Standard Deviation:

np.std(data)

Mode:

stats.mode(data, keepdims=True)

# KEY TAKEAWAYS

1. Mean, median, and mode describe the central tendency of data.
2. Standard deviation describes data variability.
3. Probability distributions describe possible outcomes and their
   probabilities.
4. Hypothesis testing helps evaluate statistical claims.
5. Correlation measures the strength and direction of a linear
   relationship.
6. Covariance describes how two variables change together.
7. A p-value helps evaluate evidence against the null hypothesis.
8. Statistical significance should be interpreted together with effect
   size and practical importance.
9. Confidence intervals provide a range of plausible values for a
   population parameter.
10. Margin of error describes uncertainty around an estimate.

# PRACTICE IDEAS

1. Calculate mean, median, mode, and standard deviation for a sales
   dataset.
2. Plot a histogram and identify whether the data resembles a normal
   distribution.
3. Perform a t-test between two groups.
4. Calculate correlation between advertising spend and sales.
5. Calculate covariance between two numerical variables.
6. Perform a hypothesis test using a 0.05 significance level.
7. Calculate a 95% confidence interval for a sample mean.
8. Compare confidence intervals using different sample sizes.
9. Interpret p-values from statistical tests.
10. Build a complete statistical analysis report using Python,
    NumPy, Pandas, and SciPy.
