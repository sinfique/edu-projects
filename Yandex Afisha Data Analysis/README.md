Yandex.Books Data Analysis
Author
Chertova Nataliya

Date
June 05, 2025

Project Overview
This project focuses on analyzing user activity data from the Yandex Books service. The primary goal is to understand user behavior, particularly focusing on the time spent reading and listening to books within the application, and to test a specific hypothesis related to user loyalty and Lifetime Value (LTV).

Problem Statement
The project aims to investigate whether users who contribute higher Lifetime Value (LTV) are more loyal, which is hypothesized to manifest as spending, on average, more time reading and listening to books in the application.

Project Goals and Objectives
Project Goal
To analyze data received from the Yandex Books service and test the hypothesis that users who bring higher LTV are more loyal, and therefore, spend, on average, more time reading and listening to books in the application.

Project Objectives
Data Loading and Evaluation: Download and evaluate the provided data, specifically user data from Moscow and St. Petersburg with their total activity hours from the yandex_knigi_data.csv file.

Data Preprocessing: Check for duplicate user IDs, compare group sizes, their statistics, and distribution.

Statistical Hypothesis Testing: Statistically test the hypothesis that users from St. Petersburg spend, on average, more time reading and listening to books in the application than users from Moscow. This will be done using a one-sided hypothesis test with two samples.

Analytical Report Preparation: Prepare an analytical report summarizing the data analysis results.

Hypothesis Testing: St. Petersburg vs. Moscow User Activity
The core hypothesis tested in this project is: users from St. Petersburg spend, on average, more time reading and listening to books in the application than users from Moscow.

Null Hypothesis (H 
0
​
 ): μ 
SPb
​
 ≤μ 
Moscow
​
  (The average activity time of users in St. Petersburg is not greater than in Moscow.)

Alternative Hypothesis (H 
1
​
 ): μ 
SPb
​
 >μ 
Moscow
​
  (The average activity time of users in St. Petersburg is greater, and this difference is statistically significant.)

Analytical Report Summary
Test Methodology
For the analysis, Student's t-test was chosen. This test is optimal for the task conditions, involving two samples that meet the required criteria:

Normality of the sample mean: Ensured due to a sufficient amount of data.

Independence of observations: Ensured by excluding overlapping users.

Equality of sample variances: Confirmed by Fisher's F-test.

A significance level (α) of 5% was adopted for hypothesis testing, which is a standard value for this type of test.

Test Results
P-value: 0.33

Conclusion
Based on the obtained p-value of 0.33, which is greater than the chosen significance level of 0.05, we fail to reject the null hypothesis.

This indicator suggests that we do not have enough statistically significant evidence to claim that the average user activity in hours in the two groups (Moscow and St. Petersburg) differs. In other words, based on this analysis, we cannot conclude that users from St. Petersburg spend, on average, more time reading and listening to books in the application than users from Moscow.

Possible Explanations for the Results
This result can be explained by the following:

No True Difference: There truly is no significant difference in average activity time between users from St. Petersburg and Moscow. If this is the case, then the LTV difference (if observed) between cities is influenced by factors other than average time spent reading/listening in the app.

Insufficient Test Power (Type II Error): There might be a difference between the groups, but the test was not powerful enough to detect it. This could be due to factors like sample size, variability within the data, or the effect size being too small to be detected with the current setup.