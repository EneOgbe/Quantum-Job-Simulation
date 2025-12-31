# Quantum-Job-Simulation
# Quantium Job Simulation – Data Analysis Project

## Project Overview
This project forms part of the Quantium Virtual Job Simulation on Forage.  
The objective of the analysis is to examine transaction and customer data to
identify key drivers of sales, understand customer purchasing behaviour, and
provide data-driven recommendations to support business decision-making.

The analysis focuses on data quality checks, customer segmentation, sales
drivers, and actionable insights for stakeholder reporting.

---

## Datasets
The analysis uses two datasets:

- **Transaction data** (`QVI_transaction_data.xlsx`)
  - Contains detailed records of chip purchases including date, product,
    quantity, and total sales.
- **Customer data** (`QVI_purchase_behaviour.csv`)
  - Contains customer demographic information such as lifestage and premium
    customer classification.

Raw datasets are stored locally and are not modified directly. Cleaned and
analysis-ready datasets are saved as CSV files in the `output/` directory.

---

## Analysis Workflow

### 1. Data Quality Checks
- Inspected transaction and customer datasets for missing values, incorrect
  data types, and duplicate records.
- Identified and removed extreme transaction outliers that were not
  representative of typical household purchasing behaviour.
- Verified uniqueness of customer loyalty card numbers to ensure valid merging.

### 2. Data Preparation
- Converted transaction date fields into datetime format.
- Merged cleaned transaction and customer datasets using a left join to retain
  all transaction records.
- Saved cleaned and merged datasets for reproducibility.

### 3. Sales and Customer Analysis
- Defined key metrics including total sales, transaction count, and customer
  count.
- Analysed total sales by customer lifestage and premium category.
- Investigated drivers of sales by comparing transaction frequency and spend
  per transaction.
- Examined packet size preferences across customer segments.

### 4. Visualisation and Reporting
- Created and saved charts to support insights and stakeholder reporting.
- Summarised findings in a clear, business-focused narrative.

---

## Key Findings
- Average spend per transaction is consistent across customer segments.
- Packet size preferences show minimal variation by lifestage.
- Differences in total sales are primarily driven by transaction frequency.
- High-performing segments generate sales through frequent purchasing rather
  than higher spend per visit.

---

## Tools Used
- Python
- pandas
- matplotlib
- Jupyter Notebook (GitHub Codespaces)

---

## Author
Prepared by Ene Ogbe as part of the Quantium Virtual Job Simulation to demonstrate data
analysis, problem-solving, and business insight development.

