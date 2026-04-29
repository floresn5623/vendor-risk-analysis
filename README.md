<div align="center">

<img src="https://img.shields.io/badge/NYTU%20Analytics-Vendor%20Risk%20Solution-1B3A6B?style=for-the-badge&logo=databricks&logoColor=white" alt="NYTU Analytics"/>

# Vendor Risk Analysis & Procurement Insights Dashboard

**INFO-465-002 · Projects in Information Systems · Spring 2026**

[![KNIME](https://img.shields.io/badge/KNIME-Data%20Processing-FFA500?style=flat-square&logo=knime&logoColor=white)](https://www.knime.com/)
[![Tableau](https://img.shields.io/badge/Tableau-Visualization-E97627?style=flat-square&logo=tableau&logoColor=white)](https://www.tableau.com/)
[![GitHub](https://img.shields.io/badge/GitHub-Version%20Control-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/)
[![Status](https://img.shields.io/badge/Status-Complete-2E75B6?style=flat-square)](.)

</div>

---

## 📌 Overview

This project transforms raw procurement data into **clear, actionable insights** on vendor risk, spending concentration, and supplier diversity. Built for real-world procurement decision-making, the solution integrates **KNIME** for automated data engineering and **Tableau** for interactive visualization — creating a complete end-to-end analytics pipeline.

> _"Bridging the gap between raw procurement data and strategic decision-making."_

---

## 🚨 The Problem

Organizations managing large procurement portfolios often operate with limited visibility into:

| Challenge | Impact |
|-----------|--------|
| Vendor dependency & risk exposure | Operational disruptions when key vendors fail |
| High spending concentration | Financial vulnerability from over-reliance on few suppliers |
| Limited supplier diversity | Missed opportunities for SWAM vendor participation |
| Lack of structured analysis | Reactive, inefficient procurement decisions |

---

## ✅ Our Solution

We built a data-driven analytics system that:

- 🧹 **Cleans & standardizes** raw procurement data from 2024–2025
- 📊 **Aggregates** vendor-level spending using automated KNIME workflows
- 🔴 **Classifies** vendors into High / Medium / Low risk tiers
- 📈 **Visualizes** all insights through an interactive Tableau dashboard
- 🤝 **Analyzes SWAM participation** to support supplier diversity goals

---

## 🏗️ Architecture
Raw Procurement Data (2024–2025 CSV Files)
│
▼
┌─────────────────────────┐
│   KNIME Data Pipeline   │
│  ┌───────────────────┐  │
│  │  Data Cleaning    │  │   → Standardize vendor names
│  │  & Preparation    │  │   → Format numeric fields
│  └────────┬──────────┘  │   → Merge yearly datasets
│           │             │
│  ┌────────▼──────────┐  │
│  │ Vendor-Level      │  │   → GroupBy aggregation
│  │ Aggregation       │  │   → Total spend, count, avg price
│  └────────┬──────────┘  │
│           │             │
│  ┌────────▼──────────┐  │
│  │ Risk Classification│  │   → High / Medium / Low
│  │ Model             │  │   → Rule-based spend thresholds
│  └────────┬──────────┘  │
└───────────┼─────────────┘
│
▼
vendor_risk_output.csv

Pareto analysis outputs
│
▼
┌─────────────────────────┐
│  Tableau Dashboard      │
│  • Vendor risk KPIs     │
│  • Pareto spend chart   │
│  • SWAM vs Non-SWAM     │
└─────────────────────────┘
│
▼
Business Insights & Strategic Recommendations


---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **KNIME** | Data cleaning, transformation, aggregation & risk classification |
| **Tableau** | Interactive dashboard development & visualization |
| **GitHub** | Version control, collaboration & project documentation |
| **CSV / Excel** | Raw data input format (2024 & 2025 procurement records) |

---

## ✨ Key Features

- 🔴 **Vendor Risk Classification** — Automated High / Medium / Low risk scoring
- 📊 **Pareto Analysis** — Identify the vendors driving spending concentration
- 💰 **Procurement Spend KPI** — Total spend summary at a glance
- 🤝 **SWAM Analysis** — SWAM vs. Non-SWAM vendor spend comparison *(subset-based)*
- 🔁 **Scalable Workflow** — Reusable KNIME pipeline for future datasets
- 📋 **Interactive Dashboard** — Decision-ready Tableau visualization

---

## 📊 Key Insights

> **60%** of total procurement spend is concentrated among just **14 vendors**

- A small number of vendors account for the majority of organizational spend
- Several high-spend vendors carry **High Risk** classifications due to dependency
- SWAM vendors represent a smaller share of total spend — indicating room for improvement
- Diversification opportunities exist across both spend and supplier categories

---

## 💼 Business Impact

| Value Driver | Description |
|---|---|
| 📉 **Risk Reduction** | Reduces operational exposure from vendor concentration |
| 🎯 **Better Decisions** | Data-driven procurement strategy backed by evidence |
| 🤝 **Supplier Diversity** | Identifies SWAM vendor gaps and opportunities |
| 📈 **Scalability** | KNIME workflow reusable for any future procurement dataset |

---

## 📁 Project Structure
vendor-risk-analysis/
│
├── data/
│   ├── raw/
│   │   ├── procurement_2024.csv
│   │   └── procurement_2025.csv
│   └── processed/
│       ├── vendor_risk_output.csv
│       └── pareto_output.csv
│
├── knime/
│   └── vendor_risk_workflow.knwf
│
├── tableau/
│   └── vendor_risk_dashboard.twb
│
├── docs/
│   ├── Business_Proposal.docx
│   └── Architecture_Document.docx
│
└── README.md

---

## ⚙️ How to Run

### KNIME Workflow

1. Open **KNIME Analytics Platform**
2. Import `knime/vendor_risk_workflow.knwf`
3. Update the file path nodes to point to your local `data/raw/` directory
4. Execute the full workflow
5. Output will be saved to `data/processed/vendor_risk_output.csv`

### Tableau Dashboard

1. Open **Tableau Desktop**
2. Open `tableau/vendor_risk_dashboard.twb`
3. If prompted, reconnect the data source to `data/processed/vendor_risk_output.csv`
4. The dashboard will populate automatically

> **Note:** The Tableau file (`.twb`) is provided separately due to file size. SWAM analysis is based on the subset of data where classification was available.

---

## 📈 Scalability

The KNIME workflow is designed for **reusability**:

- Drop in new yearly procurement CSV files
- Re-execute the workflow — no redesign needed
- Tableau dashboard refreshes automatically with updated data
- Risk classification thresholds can be adjusted as organizational needs evolve

This means **continuous vendor risk monitoring** with minimal ongoing effort.

---

## 👥 Team

<div align="center">

**NYTU Analytics** · INFO-465-002 · Spring 2026

| | Name |
|---|---|
| 👤 | **Natalia Flores** |
| 👤 | **Umaiza Farooque** |
| 👤 | **Yasmien Jemaledin** |
| 👤 | **Taylor Winston** |

</div>

---

## 📄 Deliverables

- [x] Business Proposal (`docs/Business_Proposal.docx`)
- [x] Architecture Document (`docs/Architecture_Document.docx`)
- [x] KNIME Workflow (`knime/vendor_risk_workflow.knwf`)
- [x] Tableau Dashboard (`tableau/vendor_risk_dashboard.twb`)
- [x] Processed Dataset (`data/processed/vendor_risk_output.csv`)
- [x] GitHub Repository with commit history

---

## 🎯 Final Takeaway

This project demonstrates how **data analytics can transform raw procurement records into strategic intelligence** — identifying vendor risk, surfacing spending concentration, and uncovering opportunities to improve supplier diversity.

Built with scalability in mind, the solution is ready for real-world deployment and continuous monitoring.

---

<div align="center">

_NYTU Analytics · INFO-465-002 · Spring 2026_

</div>
