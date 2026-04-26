# Vendor Risk Analysis

## Overview
This project analyzes procurement data to identify vendor risk, spending concentration, and opportunities for improvement. The solution combines data preparation, risk classification, and data visualization to support better decision-making.

## Tools Used
- KNIME (data cleaning, transformation, and risk classification)
- Tableau (data visualization and dashboard development)

## Data
The analysis uses procurement data from 2024 and 2025, including vendor information, transaction amounts, and purchasing activity.

## Key Insights
- Top 14 vendors account for approximately 60% of total spend, indicating strong vendor concentration
- A small number of vendors drive the majority of procurement activity
- Approximately 18% of total spend goes to SWAM vendors, highlighting an opportunity to improve supplier diversity

## Solution Components

### 1. Vendor Risk Classification
- Cleaned and standardized vendor data
- Aggregated total spend at the vendor level
- Applied rules to classify vendors into high, medium, and low risk

### 2. Pareto Analysis (Spend Concentration)
- Analyzed how spending accumulates across vendors
- Identified concentration of spend among a small group of vendors

### 3. SWAM vs Non-SWAM Analysis
- Compared spending between SWAM and non-SWAM vendors
- Highlighted gaps in supplier diversity

### 4. Dashboard
- Combined all insights into a single Tableau dashboard
- Provides a clear view of vendor risk, spending concentration, and diversity opportunities

## Files
- `Vendor_Risk_Analysis.knwf` – KNIME workflow used for data preparation and modeling
- `vendor_risk.csv` – Processed dataset used for analysis and visualization
- `dashboard_preview.png` – Screenshot of the final dashboard

## Business Impact
- Identifies vendor dependency risk
- Supports data-driven procurement decisions
- Highlights opportunities to improve supplier diversity
