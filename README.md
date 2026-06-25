# Population Health Spending & Life Expectancy Analysis

## Business Question
*Which countries exhibit the greatest disparity between healthcare spending and life expectancy outcomes — and what drives spending inefficiency?*

This project analyzes global population health data across 6 major nations from 1970-2020 to identify where healthcare investment fails to translate into longer, healthier lives — informing value-based care strategy and resource allocation decisions.

---

## Why This Matters
Global healthcare spending exceeds $8.5T annually, yet life expectancy varies dramatically across countries with similar spending levels. Identifying spending inefficiency patterns is foundational to public health policy, ACO performance management, and value-based care program design.

---

## Key Findings
- *USA highest spender at $4,388 average* but ranks last in healthcare efficiency among all 6 nations
- *Japan most efficient* — achieves highest life expectancy per dollar spent (42.77 life years per $1,000)
- *High-spending countries* do not consistently produce better life expectancy outcomes — revealing systemic inefficiency in care delivery
- *Spending growth trend* shows accelerating per-capita costs without proportional life expectancy improvements over time
- *USA spending increased by $5,426* since 1990 — highest growth of all nations analyzed
- *Correlation analysis* confirms diminishing returns on healthcare spending beyond a threshold, particularly in high-income countries

---

## Python Analysis Highlights
- Segmented countries into spending tiers using pandas quantile() and cut()
- Ranked countries by spending-to-life expectancy efficiency ratio using groupby() and rank()
- Built correlation analysis between per-capita spending and life expectancy using corr() and scatter visualizations
- Performed multi-year trend analysis using pivot_table() and time-series aggregation

---

## SQL Analysis Highlights

### Query 1 — Top Nations by Healthcare Spending & Life Expectancy
- Used GROUP BY and AVG aggregations to rank countries by average spending and life expectancy
- Identified USA as highest spender at $4,388 average but with lowest efficiency score (17.28)

### Query 2 — Healthcare Spending Growth by Decade
- Used CASE WHEN statements to segment data into decades (1970s-2020s)
- Revealed all nations show dramatic spending growth post-1990 with USA leading at $6,623 recent average

### Query 3 — Healthcare Efficiency Score Analysis
- Built custom efficiency metric: Life Expectancy gained per $1,000 spent
- Japan ranked most efficient (42.77) vs USA least efficient (17.28) despite highest spending

### Query 4 — Historical vs Recent Spending Comparison
- Used conditional aggregation with CASE WHEN to compare pre/post 1990 spending
- USA showed largest spending increase of $5,426 — highest growth among all nations

### Key SQL Techniques Used
- GROUP BY with multiple aggregations
- CASE WHEN for decade segmentation
- Conditional aggregation for period comparison
- Custom calculated efficiency metrics
- ORDER BY for ranked analysis

---

## Data Quality Challenges
- Validated 274 records across 6 nations with zero missing values
- Standardized country name formats for consistent grouping and aggregation
- Verified spending currency consistency across all nations and time periods
- Confirmed life expectancy measurements aligned across all reporting periods

---

## Tools & Technologies
| Layer | Tool |
|---|---|
| Data Processing | Python (pandas, numpy, matplotlib, seaborn) |
| Analysis | Python (Google Colab), SQL (SQLite) |
| Visualization | Tableau |
| Data Source | Seaborn Health Expenditure Dataset (healthexp) |

---

## Dashboard Features
- Country-level spending vs life expectancy scatter analysis
- Spending efficiency ratio by country
- Multi-year spending trend visualization from 1970-2020
- Country-level life expectancy comparison

**[View Tableau Dashboard](https://public.tableau.com/app/profile/lokesh.reddy2043/viz/PopulationHealthAnalysis_17823656433670/Dashboard1)**

---

## Analytical Approach
1. Ingested and cleaned healthcare expenditure dataset (274 records, 6 nations, 1970-2020)
2. Segmented countries into spending tiers and efficiency groups
3. Built spending efficiency ratio (life expectancy per $1,000 per capita spending)
4. Designed dashboard for both executive summary and country-level drill-down

---

## Recommendations
- Prioritize preventive care investment in high-spending, low-outcome regions — USA efficiency score of 17.28 vs Japan 42.77 represents a 2.5x improvement opportunity
- Benchmark Japan and Great Britain as models for value-based care design given highest efficiency scores
- Redirect resources toward social determinants of health in countries with persistent life expectancy gaps
- Monitor spending growth trends as early indicators of future inefficiency
- Redirecting 10% of USA healthcare spending toward preventive care initiatives could improve efficiency score by an estimated 15-20% based on Japan and Great Britain benchmarks

---

## Domain Context
This analysis applies concepts central to *population health management, **value-based care strategy, and **health economics* — areas where understanding the relationship between spending and outcomes directly impacts plan design, policy decisions, and member health.

---

## About
Built by *Lokesh Bayyapu*, PharmD, MS Health Data Science
Healthcare Data Analyst | Medicare Advantage & Population Health
[LinkedIn](https://www.linkedin.com/in/lokeshreddy1) | [Tableau Public](https://public.tableau.com/app/profile/lokesh.reddy2043/vizzes)
