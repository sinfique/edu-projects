Yandex.Afisha Data Analysis

Project Overview
This project involves an in-depth analysis of data from the Yandex.Afisha service, a platform where users can find information about events in various cities and purchase tickets. Yandex.Afisha collaborates with event organizers and ticket operators who supply event details and manage ticket sales.

Problem Statement
In November 2024, the product department observed an unexpected trend: ticket sales for some events were increasing, while for others, they were decreasing. This shift in user preferences required immediate investigation to understand its underlying causes.

Research Questions
The analysis aimed to answer the following key questions:

Is the change in user preferences due to seasonality, shifts in audience demographics, or other contributing factors?

Which events began attracting more viewers, and which organizers and venues emerged as leaders?

Do mobile users exhibit different activity patterns compared to users booking tickets from stationary computers?

Tools Used
Yandex.Datalens: A dashboard was developed for initial analysis and visualization (accessible at: https://datalens.yandex/4paeueyblw1oq).

Python: Used for exploratory data analysis (EDA) and statistical hypothesis testing to supplement dashboard insights and provide deeper understanding.

Goals and Objectives
Project Goal
To conduct an exploratory data analysis of the Yandex.Afisha service data for the specified period of 2024, identify key insights into changes in user preferences and event popularity, and test statistical hypotheses regarding behavioral differences between mobile and stationary device users.

Project Objectives
Data Loading and Initial Familiarization: Load the provided datasets, assess their volume, correctness, and correspondence to the description, and outline initial preprocessing steps.

Data Preprocessing: Clean the data by handling missing values and outliers, checking for explicit and implicit duplicates and errors, and performing data type conversions. This includes converting all financial data to Russian rubles and creating new columns such as revenue per ticket (one_ticket_revenue_rub), month, and seasonality.

Exploratory Data Analysis (EDA): Thoroughly study:

Seasonal changes in order distribution across various segments: event type, device type, and age restrictions.

Revenue dynamics from the sale of one ticket depending on the event type in the summer and autumn periods.

Daily and weekly user activity in the autumn of 2024, including the dynamics of the total number of orders, daily active users (DAU), average number of orders per user, and average ticket price.

The popularity of events and partners, analyzing the distribution by regions and the contribution of various ticket operators.

Statistical Data Analysis: Test two key hypotheses proposed by the product team regarding the activity of mobile and stationary device users:

Hypothesis that the average number of orders per mobile application user is higher than for stationary device users.

Hypothesis that the average time between orders for mobile application users is longer than for stationary device users.

Formulating a General Conclusion and Recommendations: Based on all the insights obtained, formulate concise conclusions and offer actionable recommendations for the product team.

Data Information
The analysis encompassed 290,849 ticket order records and 22,427 event records, covering the period from June 1 to October 30, 2024. The data underwent successful preprocessing, including handling missing values and outliers, unifying currency to rubles, and adding aggregated features such as revenue per ticket, month, and seasonality. After preprocessing, 287,499 records were included in the final analysis.

Key Analysis Results
Seasonality and Event Popularity:
With the arrival of autumn (September-October), there was a noticeable increase in the total number of orders, confirming a significant seasonal factor.

Concerts, theater, and "other" were the most in-demand event types. In autumn, the share of theater, sports, and Christmas tree events increased compared to the summer period.

The average cost of a single ticket generally decreased in autumn. Across different event categories, the average price decreased for concert, theater, and Christmas tree categories; for other categories, the price changed insignificantly, except for stand-up, where the price slightly increased.

Regarding age restrictions, events rated 16+ were most popular, though their share decreased in the autumn, while the share of events without age restrictions, conversely, increased.

User Activity:
Daily activity analysis showed an increase in the number of unique users (DAU) and a slight rise in the number of orders. All observed metrics displayed notable peaks and troughs.

Weekly cyclicity was identified: the average number of orders and orders per user peaked on Tuesdays, but on this day, the average ticket price was also at its minimum.

No clear cyclicity was observed for other key metrics (number of orders, DAU, orders per user, average check) based on days of the week.

There was some decrease in activity on weekends compared to weekdays. On weekdays, the average number of orders was 2905, unique users 937, and average ticket price 178. On weekends, the average number of orders was 2395, unique users 887, and average ticket price 193.

Leaders Among Regions and Partners:
The Kamenevsky District and Severoyarskaya Oblast were clear leaders in both event diversity and the number of orders, contributing 40% of the total orders.

Among ticket partners, "Lovi Bilet!" and "Bilety Bez Problem" made the largest contribution to revenue and the number of processed orders. These partners processed 34% of all orders and generated 28% of the revenue.

Hypothesis Testing Results
Two hypotheses regarding the activity of mobile and desktop device users were tested based on autumn data. Users who made orders from both device types were excluded to ensure sample independence.

Hypothesis 1: The average number of orders per mobile app user is higher compared to desktop users.
P-value: 0.000

At a significance level of α=0.05: REJECT the null hypothesis.

Conclusion: There IS statistically significant evidence that the average number of orders per mobile app user is higher than for desktop users. The average number of orders was 2.86 for mobile and 1.97 for desktop.

Hypothesis 2: The average time between orders for mobile app users is higher compared to desktop users.
P-value: 0.000

At a significance level of α=0.05: REJECT the null hypothesis.

Conclusion: There IS statistically significant evidence that the average time between orders for mobile app users is higher than for desktop users. The average time between orders was 13.79 days for mobile and 18.07 days for desktop.

Recommendations
Based on this analysis, the following recommendations are proposed for the product team:

Leverage seasonality to optimize marketing campaigns. Given the increase in orders in autumn, intensify advertising efforts during this period, focusing on theater, sports, and Christmas tree events, which showed the highest growth.

Optimize the experience for desktop users. Since Hypothesis 1 showed differences in behavior (number of orders per user), focus on improving the conversion funnel or retention for the less active group. For instance, since desktop users make fewer orders, consider simplifying the purchasing process or sending email reminders.

Maintain strong relationships with leading partners and regions. Considering their significant contribution to revenue and order volume, explore expanding cooperation or conducting joint promotions with "Lovi Bilet!" and "Bilety Bez Problem," as well as increasing the number of events in the Kamenevsky District and Severoyarskaya Oblast.

Utilize weekly cyclicity. As weekdays, and Tuesdays in particular, demonstrate higher activity, consider planning promotional launches or intensifying ad messages on this day to maximize this peak in demand.