# Global Life Expectancy Analysis: Health, Socioeconomic, and Education Factors (2000–2015)

## Project Overview
This project examines the key health indicators, socioeconomic factors, and education-related variables that influence **global life expectancy** across countries. Using a comprehensive dataset spanning **193 countries from 2000 to 2015**, we applied statistical modeling techniques to identify significant determinants of life expectancy and quantify their impact.

The analysis was conducted as part of an **Applied Statistics in Biomedical Informatics** course and emphasizes real-world public health implications and policy relevance.

---

## Research Questions
1. **What health and socioeconomic factors significantly influence life expectancy across countries?**
2. **Does education level (schooling) significantly impact life expectancy after controlling for economic and health factors?**

---

## Dataset
- **Source:** WHO Global Health Observatory (via Kaggle)
- **Time Period:** 2000–2015
- **Countries:** 193
- **Observations:** 2,938 (reduced to 1,853 after cleaning)
- **Variables:** 22 total (mortality, immunization, economic, and social indicators)

Key variables include:
- Adult Mortality, Infant Deaths, Under-Five Deaths
- HIV/AIDS prevalence
- Immunization coverage (Hepatitis B, Diphtheria, Polio)
- GDP, Health Expenditure
- Income Composition of Resources
- Schooling (education level)

---

## Data Preparation
- Removed rows with missing values
- Cleaned column names
- Identified and capped outliers using the **IQR method**
- Assessed variable distributions and normality using:
  - Boxplots
  - Q–Q plots

---

## Exploratory Data Analysis
- Summary statistics for all variables
- Scatter plots to examine linear relationships with life expectancy
- Spearman correlation heatmap to identify association patterns

Key observations:
- Strong **negative correlations** with mortality indicators
- Strong **positive correlations** with schooling, income composition, and GDP

---

## Statistical Modeling
- **Multiple Linear Regression**
- Stepwise model refinement to retain only significant predictors
- Model diagnostics included:
  - Residual plots
  - Q–Q plots
  - Histogram of residuals

### Final Model Performance
- **Adjusted R²:** 0.8319  
- Explains ~83% of variability in life expectancy

---

## Key Findings
- Higher **adult mortality**, **under-five deaths**, and **HIV/AIDS prevalence** significantly reduce life expectancy
- **Education (schooling)** has a strong, independent positive effect on life expectancy
- **Income composition of resources** is one of the strongest positive predictors
- Health expenditure and immunization coverage play meaningful roles in improving population longevity

---

## Tools & Technologies
- **R**
- Linear Regression
- Exploratory Data Analysis (EDA)
- Data Visualization
- Statistical Diagnostics

---

## Project Files
- **Presentation:** `presentation/global_life_expectancy_analysis_presentation.pdf`
- **Full Report:** `report/global_life_expectancy_analysis_report.pdf`
- **R Code:** `code/life_expectancy_analysis.Rmd`

---

## Key Takeaway
This project demonstrates how statistical modeling can uncover actionable insights into global health disparities, highlighting the critical roles of **education, economic stability, and healthcare access** in improving life expectancy outcomes.

---
