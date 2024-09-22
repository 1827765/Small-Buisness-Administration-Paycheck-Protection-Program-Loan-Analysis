# PPP Loan Analysis Project

This project analyzes the publicly available Paycheck Protection Program (PPP) loan data sourced from the U.S. Small Business Administration (SBA). The goal of this analysis is to extract key insights about loan distribution, forgiveness, and trends across industries and demographics during the COVID-19 pandemic.

## Project Overview

This repository contains SQL queries and Python code used for data cleaning, exploration, and analysis of the SBA’s PPP loan dataset and related industry data. The key components of the project include:

- **Data Cleaning:** Preparation and cleaning of the PPP loan dataset, including handling missing data and correcting industry sector information.
- **Exploratory Data Analysis (EDA):** Visualizing loan approvals, loan amounts, and forgiveness patterns across sectors, loan rounds, borrower demographics, and lender details.
- **Correlation Analysis:** Investigating relationships between key variables such as loan amounts and forgiveness ratios using statistical methods.
- **Comparative Analysis:** Year-over-year comparison of loan approvals, amounts, forgiveness, and originating lenders for 2020 and 2021.
- **NAICS Codes Analysis:** Classifying loan data by industry sector using NAICS codes and matching with the SBA’s table of size standards.

## Data Sources

1. [PPP FOIA Dataset](https://data.sba.gov/dataset/ppp-foia) - Publicly available dataset with PPP loan information.
2. [Table of Size Standards](https://www.sba.gov/document/support-table-size-standards) - Dataset containing size standards for small businesses based on NAICS codes.

## Files

- `ppp_analysis.sql`: SQL queries for analyzing loan approvals, forgiveness, and industry trends.
- `ppp_data_cleaning.py`: Python script for cleaning the PPP loan dataset and industry data from the SBA.
- `eda_analysis.py`: Python code for Exploratory Data Analysis (EDA) using pandas, matplotlib, and seaborn.
- `clean_sba_codes_noindex.csv`: Cleaned NAICS codes and industry sector data for analysis.
  
## Key Insights

- The majority of PPP loans in 2020 and 2021 were fully forgiven, with 97% of loans forgiven in 2020 and 94% in 2021.
- April 2020 and January 2021 were the months with the highest loan approvals.
- Certain industry sectors, such as Healthcare and Social Assistance, received a higher proportion of loans, both in terms of total loan amount and number of loans approved.
- Demographic analysis shows disparities in loan distribution across gender and ethnicity categories.

## Prerequisites

- **Python 3.x**
- **pandas, numpy, matplotlib, seaborn** for EDA
- **SQL Server or any other database supporting SQL** for SQL analysis
- **Jupyter Notebook** (optional for running Python scripts interactively)

## Usage

### SQL Queries
To run the SQL queries, load the `ppp_analysis.sql` file into your preferred SQL environment, ensuring that the PPP dataset is correctly imported and indexed for optimal performance.

### Python Scripts
Run the Python scripts in the following order:
1. `ppp_data_cleaning.py` - Clean the raw data and output CSVs for further analysis.
2. `eda_analysis.py` - Perform exploratory data analysis and visualize trends in the dataset.

```bash
# Example command to run the EDA script
python eda_analysis.py
## Tableau Dashboard

A visual representation of the analysis can be found in the following Tableau dashboard: [PPP Summary Dashboard](https://public.tableau.com/app/profile/adekunle.omotayo/viz/PPPSUMMARYDASHBOARD/Dashboard2?publish=yes).
