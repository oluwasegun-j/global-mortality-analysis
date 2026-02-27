📊 Global Mortality Analysis

Overview

This project analyzes mortality rates across countries and years using structured population and mortality datasets.
The objective was to calculate standardized death rates per 100,000 population to enable meaningful cross-country comparisons across major age bands.
________________________________________
Dataset

The analysis uses:
•	Mortality counts by age group and year
•	Population counts by age group and year
•	Country reference table
Age groups analyzed:
•	Under 5
•	5–19
•	20–39
•	40–59
•	60–79
•	80+
________________________________________
Methodology
1️⃣   Data Aggregation
•	Aggregated mortality counts by country and year
•	Aggregated population counts by corresponding age bands
2️⃣   Rate Standardization
Mortality rates calculated as:
(Deaths ÷ Population) × 100,000
Using per-100,000 normalization ensures comparability across countries with different population sizes.
3️⃣   Query Optimization
•	Used Common Table Expressions (CTEs)
•	Pre-aggregated mortality and population tables before joining
•	Applied COALESCE() and NULLIF() to handle missing values and prevent division errors
________________________________________
Key Insights
•	Under-5 mortality rates show significant variation across countries
•	Smaller population age bands produce more volatile rate estimates
•	Standardized rates reveal structural mortality differences across regions
________________________________________
Tools Used
•	SQL (MySQL syntax)
•	Jupyter Notebook
•	Git & GitHub
________________________________________
Repository Structure
global-mortality-analysis/
│
├── global_mortality_analysis.ipynb
└── README.md

