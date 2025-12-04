# Case-Study
# Financial Data Extraction & KPI Analysis (Werkstudent Data Engineering Case Study)

## Overview
This project extracts and analyzes financial performance data for publicly listed U.S. companies. 
The goal is to demonstrate the ability to design a real data pipeline end-to-end: 
data extraction, cleaning, validation, KPI engineering, visualization, and insight generation.

The final structured dataset contains ** companies** across **3 or more  recent fiscal years**, 
. The analysis includes **10+ key financial KPIs** 
covering profitability, efficiency, valuation, and growth.

---

## Data Pipeline Summary
**Source Data**
- S&P 500 ticker list from Wikipedia
- Financial statements extracted via Yahoo Finance API (`yfinance`)

**Pipeline Stages**
1. Web scraping of ticker symbols
2. API-based financial data extraction
3. Data cleaning & null handling
4. KPI engineering
5. Data validation and coverage assessment
6. Visualization & insight generation
7. Export to structured CSV dataset

---

## Dataset Structure
| Field | Description |
|-------|-------------|
ticker | Stock ticker symbol (unique identifier)
company_name | Full company name
country | Country of headquarters
industry | Industry classification
year | Fiscal year of reported data
revenue | Total revenue
revenue_unit | Unit of currency
net_income | Net income
gross_profit | Profit after cost of goods sold
ebitda | Earnings before interest, tax, depreciation & amortization
total_assets | Total company assets
total_liabilities | Total obligations
employees | Full-time employees
market_cap | Market capitalization
enterprise_value | Company valuation metric
ev_to_ebitda | Valuation multiple
gross_margin | Gross Profit / Revenue
operating_margin | EBITDA / Revenue
net_profit_margin | Net Income / Revenue
roa | Net Income / Total Assets
revenue_growth | YoY % change in revenue
net_income_growth | YoY % change in net income
revenue_per_employee | Efficiency productivity metric

---

## KPIs Included
- Profitability: **Gross Margin, Operating Margin, Net Profit Margin**
- Growth: **Revenue Growth, Net Income Growth**
- Efficiency: **ROA, Revenue per Employee**
- Valuation: **EV/EBITDA, Enterprise Value**

---

## Visualizations
- Top 10 companies by revenue
- Revenue vs. net profit margin scatter plot
- Top 10 revenue per employee
- Valuation multiples (EV/EBITDA)
- Missing value & availability analysis chart

---

## Key Insights
- Revenue is highly concentrated among a few mega-cap firms.
- Profitability varies more by industry than by revenue scale.
- Growth trends differ significantly post-pandemic across sectors.
- Revenue per employee highlights operational efficiency leaders.

---

## Limitations
- Yahoo Finance does not consistently provide equity or cash flow fields.
- ROE and Debt-to-Equity metrics were removed due to insufficient coverage.
- First-year growth metrics inherently show missing values.

This reflects a realistic data engineering decision-making process,
prioritizing metric reliability over completeness.

---

## Future Improvements
- Integrate FinancialModelingPrep or SEC EDGAR API to extend KPI depth
- Automate pipeline scheduling & storage versioning
- Add BI dashboards using PowerBI / Tableau / Streamlit

---

## Repository Structure
