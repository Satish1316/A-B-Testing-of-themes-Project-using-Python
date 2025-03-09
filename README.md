# A/B Testing of Themes Project

This project conducts an **A/B Testing** analysis to compare user engagement between two different website themes: **Dark** and **Light**. The goal is to determine which theme performs better based on key user interaction metrics like **Click Through Rate (CTR)**, **Conversion Rate**, and **Bounce Rate**.

## Dataset Overview

The dataset used in this project consists of 1000 user session entries with the following metrics:

| **Metric**            | **Description** |
|-----------------------|-----------------|
| **Click Through Rate** | Proportion of users clicking links or buttons after visiting the website. |
| **Conversion Rate**    | Percentage of users who signed up after viewing a page. |
| **Bounce Rate**        | Percentage of users leaving after viewing one page. |
| **Scroll Depth**       | Pixels representing how far users scroll down the page. |
| **Session Duration**   | Time (seconds) users spend on the website. |
| **Purchases**          | Whether the user made a purchase (Yes/No). |
| **Added_to_Cart**      | Whether the user added items to their cart (Yes/No). |

## Summary of Key Metrics

Here is a snapshot of the descriptive statistics for important engagement metrics:

| Metric                  | Mean  | Std Dev | Min   | Max   |
|-------------------------|-------|---------|-------|-------|
| **Click Through Rate**   | 0.25  | 0.139   | 0.01  | 0.499 |
| **Conversion Rate**      | 0.253 | 0.139   | 0.01  | 0.498 |
| **Bounce Rate**          | 0.505 | 0.172   | 0.20  | 0.799 |
| **Scroll Depth** (px)    | 50.32 | 16.90   | 20.01 | 79.99 |
| **Session Duration** (s) | 924.99| 508.23  | 38.00 | 1797.00 |

## Visual Analysis

### 1. Click Through Rate vs Conversion Rate

We observe the relationship between **Click Through Rate (CTR)** and **Conversion Rate** for users interacting with each theme. 

| Theme | Avg Click Through Rate | Avg Conversion Rate |
|-------|------------------------|---------------------|
| Dark  | 0.28                   | 0.26                |
| Light | 0.22                   | 0.24                |

This table shows that users interacting with the **Dark** theme tend to have slightly higher click-through and conversion rates than those using the **Light** theme.

### 2. Bounce Rate Comparison

| Theme | Avg Bounce Rate |
|-------|-----------------|
| Dark  | 0.49            |
| Light | 0.52            |

The **Light** theme has a slightly higher average **Bounce Rate**, suggesting that users may be more likely to leave the page without further interaction compared to the **Dark** theme.

## Statistical Testing

To assess the significance of the differences between themes, we conducted hypothesis tests on the key metrics:

- **Click Through Rate**: p-value < 0.05, indicating a statistically significant difference in favor of the **Dark** theme.
- **Conversion Rate**: p-value ≈ 0.054, which suggests a trend but not statistically significant.

| Metric               | t-statistic | p-value  | Result                        |
|----------------------|-------------|----------|-------------------------------|
| Click Through Rate    | 2.45        | 0.015    | Significant difference         |
| Conversion Rate       | 1.92        | 0.054    | Marginally non-significant     |

## Key Insights

- **CTR**: The **Dark theme** has a significantly higher click-through rate than the **Light theme**, making it a more engaging option for users.
- **Conversion Rate**: Though the **Dark theme** shows a trend towards higher conversion rates, the difference is not statistically significant.
- **Bounce Rate**: Users interacting with the **Light theme** tend to bounce slightly more than those using the **Dark theme**.

## Conclusion

Based on the results:
- **The Dark theme** outperforms the **Light theme** in **Click Through Rate**.
- There is no conclusive evidence that **Conversion Rate** differs significantly, though the **Dark theme** shows some potential for higher conversions.
- **Bounce Rate** indicates that users are slightly more likely to leave the site when interacting with the **Light theme**.

