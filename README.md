# Population Health Spending & Life Expectancy Analysis

## Business Question
*Which countries and demographic groups exhibit the greatest disparity between healthcare spending and life expectancy outcomes — and what drives spending inefficiency?*

This project analyzes global population health data across 170+ countries to identify where healthcare investment fails to translate into longer, healthier lives — informing value-based care strategy and resource allocation decisions.

---

## Why This Matters
Global healthcare spending exceeds $8.5T annually, yet life expectancy varies by more than 30 years across countries with similar spending levels. Identifying spending inefficiency patterns is foundational to public health policy, ACO performance management, and value-based care program design.

---

## Key Findings
- *Life expectancy gap of 20+ years* identified between high-spending and low-spending nations at similar income levels
- *High-spending countries* do not consistently produce better life expectancy outcomes — revealing systemic inefficiency in care delivery
- *Spending growth trend* shows accelerating per-capita costs without proportional life expectancy improvements over time
- *Correlation analysis* confirms diminishing returns on healthcare spending beyond a threshold, particularly in high-income countries

---

## Python Analysis Highlights
- Segmented countries into spending tiers using pandas quantile() and cut()
- Ranked countries by spending-to-life expectancy efficiency ratio using groupby() and rank()
- Built correlation analysis between per-capita spending and life expectancy using corr() and scatter visualizations
- Performed multi-year trend analysis using pivot_table() and time-series aggregation

---

## Data Quality Challenges
- Resolved inconsistent country name formats across WHO and World Bank datasets
- Standardized spending metrics across different reporting years and population denominators
- Handled missing life expectancy values using regional median imputation for 15+ countries

---

## Tools & Technologies
| Layer | Tool |
|---|---|
| Data Processing | Python (pandas, numpy, matplotlib, seaborn) |
| Analysis | Python (Google Colab) |
| Visualization | Tableau |
| Data Source | WHO Global Health Expenditure Database / Our World in Data |

---

## Dashboard Features
- Country-level spending vs. life expectancy scatter analysis
- Spending efficiency ratio by region and income group
- Multi-year spending trend visualization
- Geographic heat map of life expectancy by country

**[View Tableau Dashboard](https://public.tableau.com/app/profile/lokesh.reddy2043/viz/PopulationHealthAnalysis_17823656433670/Dashboard1)**

---

## Analytical Approach
1. Ingested and cleaned global health dataset (170+ countries, multiple years)
2. Segmented countries into spending tiers and income groups
3. Built spending efficiency ratio (life expectancy per $1,000 per capita spending)
4. Designed dashboard for both executive summary and country-level drill-down

---

## Recommendations
- Prioritize preventive care investment in high-spending, low-outcome regions
- Benchmark low-cost, high-outcome countries as models for value-based care design
- Redirect resources toward social determinants of health in countries with persistent life expectancy gaps
- Monitor spending growth trends as early indicators of future inefficiency

---

## Domain Context
This analysis applies concepts central to *population health management, **value-based care strategy, and **health economics* — areas where understanding the relationship between spending and outcomes directly impacts plan design, policy decisions, and member health.

---

## About
Built by *Lokesh Bayyapu*, PharmD, MS Health Data Science  
Healthcare Data Analyst | Medicare Advantage & Population Health  
[LinkedIn](https://www.linkedin.com/in/lokeshreddy1) | [Tableau Public](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)
