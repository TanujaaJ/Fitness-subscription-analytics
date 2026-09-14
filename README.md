# Fitness-subscription-analytics
## Project overview

This project analyzes customer subscription activity for FitnessHub. The Tableau workbook examines customer retention, forecasts subscription revenue, and compares cumulative lifetime value (LTV) with customer acquisition cost (CAC).

## Dataset and data model

The analysis uses `Fitness_Subscriptions_Dataset.xlsx`, which contains two tables:
- customers: customer Id, subscription plan, acquisition channel, and CAC information
- transactions: customer Id, transaction dates, products, transaction types, and revenue
The tables are related through `Customer ID` in tableau.

## Methods and Tools
- Tableau Workbook
  
## Findings

## Customer cohort analysis
The cohort matrix groups customers by signup month and tracks the number of active customers in each month after signup.
The largest recurring decline occurs after Month 2 and 3 especially in 2025 when compared to 2024. This suggests that customers typically begin cancelling or becoming inactive after approximately two months, with the most noticeable drop appearing in Month 3. Retention continues to decrease gradually in later months more so in 2025 which has a steep decline.

## Revenue forecast
The forecast projects monthly subscription revenue for the next 12 months, from February 2026 through January 2027. Expected monthly revenue rises from approximately **$235,088K** to **$320,616K**. The combined forecast revenue for the 12-month period is approximately **$3.3M**.
The forecast mainly shows a steady upward trend. Although Tableau evaluates possible patterns repeating every 12 months, the forecast line itself does not display strong seasonality but the shaded 95% prediction interval becomes wider over time, indicating greater uncertainty for later months.

## CAC vs LTV analysis
The cumulative LTV line was compared with a constant Total CAC reference line for each signup-year cohort.
- **2024 cohort:** Total CAC is approximately **$501,537K**. Cumulative LTV increases from $438,966 in Month 3 to $505,199 in Month 4, so the cohort reaches break-even in **Month 4**.
- **2025 cohort:** Total CAC is approximately **$1,162,459**. Cumulative LTV increases from $1,140,299 in Month 5 to $1,208,333 in Month 6, so the cohort reaches break-even in **Month 6**.
The 2024 cohort recovered its acquisition cost about two months faster than the 2025 cohort.

## Key conclusions
- The most significant customer drop-off appears after Month 3, indicating that early retention efforts should focus on the first two months after signup.
- Subscription revenue is forecast to continue growing over the next 12 months, reaching approximately $320,616 per month by January 2027. It's main pattern shows sustained growth.
- The 2024 cohort reaches CAC break-even in Month 4, compared with Month 6 for the 2025 cohort.
