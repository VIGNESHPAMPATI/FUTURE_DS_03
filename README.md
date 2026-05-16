# FUTURE_DS_03 - Marketing Conversion & Funnel Intelligence

## Enterprise Analytics Portfolio Project using Power BI and Python

This project analyzes the UCI Bank Marketing dataset to understand customer conversion behavior, campaign funnel performance, and marketing efficiency.

The goal is to build a professional analytics portfolio project that combines executive dashboarding, Python-based exploratory analysis, feature engineering, and business recommendations.

## Project Objective

Bank marketing teams need to understand which customers are most likely to convert, which campaign strategies are efficient, and where prospects drop off in the funnel.

This project answers key business questions:

- What is the overall campaign conversion rate?
- Which customer segments convert best?
- Does previous campaign history improve conversion?
- Does repeated outreach improve or reduce campaign efficiency?
- Which contact methods, months, and customer profiles perform best?
- What strategic actions can improve future marketing conversion?

## Dashboard Preview

### Executive Overview

![Executive Overview](images/executive_overview.png)

### Customer Behaviour Analysis

![Customer Behaviour Analysis](images/customer_behaviour.png)

### Funnel Intelligence & Strategic Recommendations

![Funnel Intelligence](images/funnel_intelligence.png)

## Tools Used

- **Power BI** - Executive dashboard design, KPI cards, funnel visuals, segmentation analysis
- **Python** - Data analysis and feature engineering
- **Jupyter Notebook** - Analytical storytelling and documentation
- **Pandas / NumPy** - Data preparation and transformation
- **Matplotlib / Seaborn** - Exploratory visualizations
- **VS Code** - Development environment
- **GitHub** - Portfolio packaging and project documentation

## Dataset

Dataset: UCI Bank Marketing Dataset  
File used: `bank-additional-full.csv.xlsx`  
Records analyzed: **41,188 campaign records**  
Target variable: `y`, indicating whether the customer subscribed to a term deposit.

The dataset contains customer demographics, campaign contact details, previous campaign outcomes, economic indicators, and the final conversion result.

## Key KPIs

| KPI | Value |
|---|---:|
| Total campaign records | 41,188 |
| Converted customers | 4,640 |
| Non-converted customers | 36,548 |
| Overall conversion rate | 11.27% |
| Average call duration | 258.29 seconds |
| Average campaign contacts | 2.57 |
| Mobile contact conversion rate | 14.74% |
| Previous success conversion rate | 65.11% |
| Long call conversion rate, calls above 3 minutes | 19.90% |
| Campaign efficiency | 4.39% |

## Power BI Dashboard Pages

### 1. Executive Overview

The executive page summarizes campaign performance using:

- Total customers
- Conversion rate
- Converted and non-converted customers
- Average call duration
- Average campaign calls
- Funnel value by stage
- Conversion by job
- Conversion by duration group
- Contact and campaign efficiency insights

### 2. Customer Behaviour Analysis

This page focuses on customer segmentation and behavioral patterns:

- Converted customers by job
- Converted customers by education
- Conversion by previous campaign outcome
- Conversion by contact group
- Conversion by campaign intensity
- Conversion by age group
- Conversion by month
- Efficiency KPI cards

### 3. Funnel Intelligence & Strategic Recommendations

This page converts analysis into decision support:

- Advanced funnel breakdown
- Campaign intensity contribution
- Key insights
- Strategic business recommendations
- Drop-off and campaign saturation indicators

## Python Notebook Workflow

The Jupyter Notebook complements the Power BI dashboard by proving the backend analytical process.

Notebook sections include:

1. Project introduction
2. Dataset overview
3. Data cleaning
4. Feature engineering
5. Exploratory data analysis
6. Conversion analysis
7. Customer segmentation analysis
8. Campaign performance analysis
9. Visualizations using Matplotlib and Seaborn
10. Business insights
11. Strategic recommendations
12. Executive conclusion

Notebook file:

```text
notebooks/FUTURE_DS_03_Bank_Marketing_Analytics.ipynb
```

## Feature Engineering

The analysis created business-friendly fields for dashboarding and storytelling:

- `conversion_flag`
- `conversion_label`
- `age_group`
- `campaign_contact_group`
- `previous_contact_status`
- `previous_outcome_group`
- `customer_segment`
- `campaign_intensity`
- `duration_group`
- `campaign_quarter`

These features helped convert raw campaign records into meaningful business segments.

## Key Insights

1. The overall campaign conversion rate is **11.27%**.
2. Customers with previous campaign success convert at **65.11%**, making prior success the strongest conversion signal.
3. Long calls above 3 minutes convert at **19.90%**, showing that deeper engagement is associated with stronger conversion.
4. Customers contacted only once show better conversion performance than heavily contacted groups.
5. Students and retired customers are the highest-converting job segments.
6. Mobile contact performs better than telephone contact, with a **14.74%** conversion rate.
7. Campaign timing matters, with March, December, September, and October showing stronger conversion performance.

## Strategic Recommendations

- Prioritize customers with previous successful campaign outcomes.
- Improve early-contact quality instead of relying on repeated outreach.
- Build segment-specific messaging for students, retired customers, and senior customers.
- Use mobile contact as the preferred communication channel where possible.
- Review high-performing campaign months to identify timing and seasonality opportunities.
- Balance campaign volume with conversion efficiency to reduce wasted outreach.

## Analytical Limitations

- The dataset does not include a unique customer ID, so each row is treated as a campaign contact record.
- The `duration` field is useful for descriptive analysis but should not be used as a pre-campaign predictive feature because it is only known after the call.
- Some high-conversion categories have small sample sizes and should be interpreted carefully.
- External economic and business context may also influence conversion behavior.

## Project Structure

```text
FUTURE_DS_03/
  data/
    raw/
      bank-additional-full.csv.xlsx
  images/
    executive_overview.png
    customer_behaviour.png
    funnel_intelligence.png
  notebooks/
    FUTURE_DS_03_Bank_Marketing_Analytics.ipynb
  reports/
  README.md
  requirements.txt
```

## How to Run the Notebook

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open the notebook:

```text
notebooks/FUTURE_DS_03_Bank_Marketing_Analytics.ipynb
```

4. Run the notebook cells from top to bottom.

## Portfolio Value

This project demonstrates the ability to:

- Design executive-ready Power BI dashboards
- Perform Python-based exploratory data analysis
- Engineer business-friendly analytical features
- Build conversion and funnel KPIs
- Translate raw campaign data into strategic recommendations
- Connect backend analysis with dashboard storytelling

This project is designed as a professional analytics portfolio case study, showing both technical workflow and business intelligence thinking.
