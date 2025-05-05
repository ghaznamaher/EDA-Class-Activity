# EDA-Class-Activity

Feature Summary
1. Total Sale
 The product of Quantity and Price Per Unit.
Relevance:

This feature represents the final value of each transaction.

It's essential for revenue analysis, customer value segmentation, and identifying high-value transactions.

Enables correlation and trend analysis in relation to customer segments, and product categories.

2. Day of Week
Relevance:

Useful for understanding weekly purchase behavior.

Helps identify high-traffic days or slow days, enabling better marketing and staffing decisions.

Key for scheduling promotions or targeted campaigns.

3. Hour
   Hours couldn't be extracted as time data was not provided.

 *BRIEF OVERVIEW OF DATA  (Heat Map)


1. Quantity vs. Total Spent (Correlation: 0.69)
Strong positive correlation.

Indicates that as quantity increases, total spent tends to increase as well — this is expected, as buying more generally results in higher spend.

2. Price Per Unit vs. Total Spent (Correlation: 0.61)
Moderate positive correlation.

Suggests that more expensive items also lead to higher total spend, even if quantity remains constant.

3. Quantity vs. Price Per Unit (Correlation: -0.055)
Very weak negative correlation.

 Outlier  Report

Handeled outliers in the Total Spent variable using the Interquartile Range (IQR) method.

Step 1: Calculate IQR

First Quartile (Q1): 25th percentile of Total Spent

Third Quartile (Q3): 75th percentile of Total Spent

Interquartile Range (IQR) = Q3 – Q1

Step 2: Determine Bounds

Lower Bound = Q1 – 1.5 × IQR

Upper Bound = Q3 + 1.5 × IQR

Step 3: Outlier Handling (Chosen Method: Removal)

Filtered out rows where Total Spent falls outside the lower and upper bounds.

This removes extreme low or high values that may distort analysis.

Essentially no significant relationship — customers are equally likely to buy high or low quantities regardless of item price.

