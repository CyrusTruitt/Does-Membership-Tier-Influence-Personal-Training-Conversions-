# Does Membership Tier Influence Personal Training Conversions?

## Overview
This project analyzes gym membership data to identify factors influencing whether members purchase personal training sessions. The goal is to provide actionable insights that could help improve personal training conversion rates.

## Data Info
- Data File: [GYM membership .xlsx](https://github.com/user-attachments/files/19807028/GYM.membership.xlsx)
- Source: Provided internally for academic project use
- Sample Size: ~1,000 observations (gym members)
- Number of Variables: 12
- Key Variables:
    - MemberID: Unique identifier for each member
    - Age: Quantitative, in years
    - Gender: Qualitative
    - Income: Quantitative, annual income
    - Tier: Qualitative (membership tier – Basic, Premium, VIP)
    - Tenure: Quantitative, length of membership in months
    - Signed_up_for_PT: Binary (1 = yes, 0 = no) → response variable

## Hypotheses Explored
- Higher-income individuals are more likely to purchase personal training.

- Membership tier significantly influences personal training conversion.

- Tenure length correlates positively with the likelihood of signing up for PT.

- There is a difference in conversion rates between genders.

- Age is a significant predictor of personal training uptake.

## Step-by-Step Process
#### 1. Data Cleaning & Preprocessing
- Removed missing values and outliers.

- Recoded categorical variables (e.g., Tier and Gender).

- Created binary outcome variable: Signed_up_for_PT.
#### 2. Exploratory Data Analysis (EDA)
- Created visualizations:
    - Bar plots for tier vs PT sign-up rate
    - Distribution of PT sign-ups by age and income
- Generated summary statistics for all variables
#### 3. Model Building (Logistic Regression)
- Built a logistic regression model to predict the probability of a member signing up for PT.

- Included predictors: Age, Income, Tier, Gender

- Assessed multicollinearity and model fit
#### 4. Model Evaluation
- Interpreted coefficients using odds ratios

- Analyzed statistical significance using p-values

- Evaluated goodness-of-fit and predictive performance

## Results summary
#### Personal Training Conversion Rates:
- 54.2% of Premium members purchased personal training
- 49.5% of Standard members purchased personal training

#### Logistic Regression Findings:
- The overall model was statistically significant (p = 0.0015), indicating that at least one predictor contributed meaningfully to predicting PT purchase.

- Age was the only significant predictor (p = 0.0002). Each additional year of age increased the odds of purchasing PT by about 2.2%.

- Membership Tier, Visit Frequency, and Average Time in Gym were not statistically significant, meaning they had no reliable effect on PT purchase likelihood in the model.

#### Visual Insights:
- Bar Chart: Showed a small difference in PT uptake between Premium and Standard members.

- Odds Ratio Plot: Clearly showed that only Age had a confidence interval above 1, indicating significance.

- Box Plot: Showed almost identical gym time distributions between members who did and did not purchase personal training.

## Key Takeaways
- Membership tier did not significantly affect personal training conversion. While Premium members had a slightly higher conversion rate than Standard members, this difference was not statistically meaningful after accounting for other variables.
- Age was the only significant predictor. Older members were more likely to purchase personal training, with each additional year of age increasing the odds slightly but consistently.
- Gym usage patterns had no predictive value. Neither average time spent in the gym nor number of visits per week were associated with higher likelihood of purchasing personal training.
#### Implication: 
Gyms should consider targeting personal training offers based on demographic factors like age rather than membership level or gym engagement alone.

## Visual
