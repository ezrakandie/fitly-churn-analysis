# Fit.ly Subscriber Churn Analysis

A data validation and exploratory churn analysis for a fitness
subscription app, joining account, support, and in-app activity data
to identify what's driving a 28.5% churn rate.

## Approach
1. **Data validation** — checked every column across three source
   files for nulls, duplicates, valid categories, and cross-table
   join integrity before any analysis.
2. **Combining the data** — aggregated support and activity logs to
   one row per customer, joined onto account info.
3. **Exploratory analysis** — examined churn against engagement,
   support experience, and plan type.
4. **Metric proposal** — identified a leading-indicator KPI the
   business can act on before cancellation.

## Key Findings
- **Engagement is the strongest churn signal**: customers with zero
  logged activity churn at 54%, vs. 4% for customers with 3+ events —
  a 12x spread.
- **Support resolution speed matters more than ticket volume**:
  churned customers waited 18.7 hrs on average for resolution vs.
  6.7 hrs for retained customers — ticket count itself was only
  weakly related to churn.
- **Free-plan customers churn ~2x more often** than paid tiers (41%
  vs. 22–26%), and are also the least engaged segment.

## Recommended KPI: 30-Day Engagement Rate
Baseline: **17.2%**. Customers active in the last 30 days churn at
8.7%, vs. 32.6% for inactive customers — a leading indicator the
business can act on before cancellation, rather than a lagging one
that only confirms the loss after the fact.

## Recommendations
- Trigger re-engagement outreach at 30 days of inactivity (highest-
  leverage group: 38.5% of the base, churning at 54%)
- Set a support resolution SLA (e.g. 8 business hours)
- Build a structured Free-to-paid upgrade path
- Formalize GDPR/data-erasure request handling as a
