# Exploratory Data Analysis on UN Refugee Data

This project explores **global refugee data** collected by the United Nations High Commissioner for Refugees (UNHCR).  
The goal is to walk through the **Exploratory Data Analysis (EDA)** process, from cleaning and transformation to visualization and insight generation, while understanding global displacement patterns and host-country impacts.

---

## Dataset Overview

**Source:** [UNHCR Refugee Data - UN Data Portal](https://data.un.org/Data.aspx?q=refugee&d=UNHCR&f=indID%3aType-Ref)  
**File:** `UN_refugee_data.xlsx`

The dataset provides **annual statistics on refugees and refugee-like populations**, including information on:
- **Country of origin** and **country of asylum/residence**
- **Number of refugees**
- **Refugees assisted by UNHCR**
- **Administrative costs** for host countries

It serves as a valuable resource for analyzing humanitarian aid distribution, policy efficiency, and global refugee trends.

---

## Feature Description

| Feature | Description |
|----------|-------------|
| `country_asylum` | Country where refugees sought asylum or residence |
| `country_origin` | Country refugees fled from |
| `year` | Reporting year |
| `num_refugees` | Total recognized refugees |
| `refugees_assisted_by_UNHCR` | Refugees directly or indirectly supported by UNHCR |
| `total_refugees` | Total number of refugees and people in refugee-like situations |
| `total_refugees_asylum` | Refugees and refugee-like individuals in asylum countries |
| `host_country_administration_cost` | Estimated administrative cost for the host country |

---

## EDA Objectives
The main aim of this EDA is to:
1. Identify top refugee-hosting countries  
2. Examine the relationship between total refugees and those assisted by UNHCR  
3. Highlight major countries of origin  
4. Compare administrative costs among host countries  
5. Explore efficiency in refugee assistance  
6. Understand how refugee numbers have evolved over time  

---

## Data Cleaning Steps Involved

- Dropped irrelevant columns (`Unnamed:0`)  
- Fixed inconsistent column naming  
- Converted `Year` to datetime format  
- Handled missing and non-numeric values in numeric columns  
- Standardized datatypes for numerical consistency  

---

## Key Explorations

- **Univariate Analysis**: Distribution of asylum applications and refugee origins  
- **Bivariate Analysis**: Correlation between refugee count, assistance, and administrative cost  
- **Geospatial Visualization**: Global refugee distribution using choropleth maps  
- **Comparative Analysis**: Top host countries by cost and assistance efficiency  

---

## Insights

- **Turkey** and **Uganda** host some of the largest refugee populations — and shoulder significant administrative costs.  
- **Canada** recorded one of the **highest costs per assisted refugee**, suggesting comprehensive but expensive support systems.  
- Strong **positive correlation** exists between the number of refugees and administrative cost — higher refugee volumes generally mean higher expenses.  
- However, **cost-efficiency varies**: some countries manage large refugee populations with relatively lower costs, possibly due to efficient systems or external support.  

---

## Recommendations

### 1. Policy Support & Resource Allocation
- High-burden countries like **Turkey** and **Uganda** may need additional international financial assistance.  
- Countries with high costs (e.g., **Canada**) could explore process optimization without compromising service quality.

### 2. Future Research Opportunities
- Extend data beyond 2021 to observe **long-term trends** and effects of major conflicts.  
- Analyze **cost per refugee vs GDP or unemployment rate** for fairer country comparisons.  
- Apply **PCA or feature selection** to reduce redundancy among correlated variables.  
- Conduct **time-series forecasting** to predict future refugee movements and funding needs.

### 3. Efficiency Focus
- Efficiency isn’t about spending less — it’s about spending **wisely per refugee**.  
- Insights like **cost per assisted refugee** can guide fairer humanitarian budgeting and strategic support.

---

## Tools Used

- **Python**
  - `pandas`, `numpy` for data wrangling  
  - `matplotlib`, `seaborn`, `plotly` for visualizations  
- **Jupyter Notebook** for EDA documentation and reproducibility
- NB: Libraries can be install using the requirement.txt file.

---

## Example Visuals

- Top 10 Refugee-Hosting Countries  
- Refugees vs Refugees Assisted by UNHCR  
- Global Refugee Distribution (Choropleth Map)  
- Host Country Administration Costs  

---

## Conclusion

This analysis highlights how **refugee management varies widely across nations**,shaped by economic strength, international aid, and administrative efficiency.  
Data-driven insights like these can help policymakers, NGOs, and researchers **allocate resources more equitably** and design **sustainable humanitarian strategies**.

---

*Author: Eunice Gyau*  
*Data Analyst | Aspiring AI Engineer*
