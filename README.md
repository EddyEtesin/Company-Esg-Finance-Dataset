# Company-Esg-Finance-Dataset

# Company ESG and Financial Efficiency Analysis

## Overview

This project provides a comprehensive analysis of ESG (Environmental, Social, Governance) performance alongside key financial indicators across various companies and industries. The goal is to understand how sustainability metrics relate to profitability, growth, and operational efficiency.

The analysis combines environmental and financial data to identify companies and sectors that are both financially successful and environmentally responsible. It is especially useful for analysts, investors, and stakeholders focused on sustainable performance.

---

## Objectives

- Identify companies with high carbon emissions but strong ESG performance.
- Discover firms with low or negative growth but outstanding ESG scores.
- Analyze revenue efficiency relative to carbon emissions.
- Evaluate profit efficiency relative to energy consumption.
- Determine which industries deliver the highest ESG value per dollar of market capitalization.

---

## Dataset Description

The dataset includes company-level ESG and financial performance data, with the following key features:

- **ESG Metrics**: `ESG_Environmental`, `ESG_Social`, `ESG_Governance`, `ESG_Overall`
- **Financial Data**: `Revenue`, `ProfitMargin`, `MarketCap`, `GrowthRate`
- **Sustainability Metrics**: `CarbonEmissions`, `EnergyConsumption`
- **Categorical Fields**: `CompanyName`, `Industry`

---

## Key Analyses

### 1. Carbon Emissions vs ESG Environmental Score
Grouped companies to identify those with the highest total carbon emissions and compared them with their environmental ESG scores. The goal was to highlight firms that are high emitters but still score well in ESG, indicating efforts toward sustainable practices.

### 2. Low Growth and High ESG
Calculated the 10th percentile of growth rates and the 90th percentile of ESG overall scores. Companies with below-threshold growth and above-threshold ESG scores were filtered to spotlight sustainability-focused companies that may not be expanding financially but are leading in governance and responsibility.

### 3. Revenue per Ton of Carbon Emission by Industry
Computed average revenue per ton of carbon emission by industry, identifying sectors that generate significant value with relatively low environmental impact.

### 4. Profit per Unit of Energy Consumed
Derived profit using revenue and profit margin:
```python
df["Profit"] = df["Revenue"] * (df["ProfitMargin"] / 100)
```
Then evaluated how much profit each company generates per unit of energy consumed, to measure energy-based operational efficiency.

### 5. ESG Score per Dollar of Market Cap
Calculated ESG efficiency by dividing average ESG score by average market capitalization per industry. This reveals which sectors deliver high ESG value for their size.

---

## Tools and Technologies

- Python  
- Pandas (data processing)  
- Jupyter Notebook (interactive analysis)  
- Matplotlib / Seaborn (for visualizations, if needed)

---

## How to Run the Analysis

1. Clone or download the repository.
2. Open `company_esg_financial_dataset.ipynb` in Jupyter Notebook.
3. Install dependencies if needed:
```bash
pip install pandas matplotlib seaborn
```
4. Run the notebook to reproduce the analysis and results.

---

## Applications

- ESG-aligned investment research  
- Corporate sustainability benchmarking  
- Operational and energy efficiency reporting  
- Strategic advisory for ESG transformation  

---

## Author

**Ediomo Usoro Etesin**  
Data Analyst
Email: Ediomoetesin40@gmail.com  
LinkedIn: [Ediomo Etesin](https://www.linkedin.com/in/ediomo-etesin)  
