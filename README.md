# ☀️ Solar Battery Investment Analysis
### Energy Modelling | Battery Storage Simulation | 20-Year Financial Investment Appraisal

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge" />
</p>

<p align="center">
  <strong>Data-driven evaluation of the financial value of residential solar battery storage.</strong>
</p>

**Author:** Wycliffe Adek  
**Project:** Data Analyst Assessment – 2026  
**Analysis Period:** January–December 2020  
**Investment Period:** 2022–2041

---

## 1. Executive Summary

This project evaluates whether installing a **12.5 kWh battery storage system**, at an initial cost of **$7,000**, can generate sufficient long-term electricity savings to justify the investment.

Using 8,760 hourly observations of solar generation and household electricity consumption, I developed a Python-based model to simulate battery charging, discharging and grid electricity purchases.

The analysis compares the household's existing solar arrangement against a proposed battery-supported system. It then evaluates the investment over 20 years under two electricity price inflation scenarios.

**The objective:** translate historical energy data into measurable operational savings and a forward-looking investment appraisal.

## 2. Key Findings

<details>
<summary><strong>Energy performance – model outputs</strong></summary>

| Performance Measure | Result |
|---|---:|
| Hourly observations analysed | 8,760 |
| Grid purchases without battery | 15,639.36 kWh |
| Grid purchases with battery | 12,137.10 kWh |
| Electricity saved through storage | **3,502.26 kWh** |
| Annual electricity cost savings | **$595.38** |

The model indicates that battery storage reduces grid electricity purchases by approximately 3,502 kWh over the historical analysis year.

</details>

**Investment evaluation:** Two 20-year electricity price inflation scenarios were assessed using a 6% discount rate, Net Present Value (NPV) and Internal Rate of Return (IRR). The financial outcomes should be interpreted alongside the model assumptions and verified against the final notebook calculations.

## 3. Business Problem

Solar generation and household electricity demand do not always occur at the same time.

Under the existing arrangement:
- Solar electricity is consumed immediately when available.
- Excess generation is not stored for later use.
- Electricity shortfalls are purchased from the provider.

The proposed battery system provides an opportunity to store excess solar energy and use it when generation is insufficient.

The analysis addresses one central question:

**Does the additional electricity saved through battery storage justify the initial investment over the system's expected 20-year lifetime?**

## 4. Analytical Approach

The project follows a structured analytical workflow:

| Stage | Analytical Activity |
|---|---|
| 01 – Data Preparation | Load, inspect and validate hourly energy records. |
| 02 – Exploratory Analysis | Examine hourly and monthly solar generation and electricity consumption. |
| 03 – Baseline Modelling | Calculate grid purchases without battery storage. |
| 04 – Battery Simulation | Model hourly battery charging and discharging within capacity limits. |
| 05 – Energy Comparison | Quantify changes in grid purchases and electricity savings. |
| 06 – Financial Modelling | Forecast savings over 20 years under two inflation scenarios. |
| 07 – Investment Appraisal | Evaluate NPV at 6% and calculate IRR. |
| 08 – Validation | Perform energy, battery and financial reasonableness checks. |

## 5. Investment Assumptions

| Parameter | Model Assumption |
|---|---:|
| Initial battery investment | $7,000 |
| Battery capacity | 12.5 kWh |
| Expected working life | 20 years |
| Initial electricity price | $0.17/kWh |
| Scenario 1 inflation | 4% annually |
| Scenario 2 inflation | Starts at 4%, increases by 0.25 percentage points annually |
| Discount rate | 6% annually |
| Installation date | 1 January 2022 |

The financial model evaluates both inflation scenarios independently. The projections are assumption-based and depend on the historical energy profile used in the simulation.

## 6. Project Visualisations

### 6.1 Hourly Solar Generation vs Electricity Usage

![Average hourly solar generation vs electricity usage](outputs/figures/01_average_hourly_solar_vs_usage.png)

### 6.2 Monthly Grid Electricity Purchases

![Monthly grid purchases comparison](outputs/figures/02_monthly_grid_purchases_comparison.png)

### 6.3 Monthly Solar Generation vs Electricity Usage

![Monthly solar generation vs electricity usage](outputs/figures/03_monthly_solar_generation_vs_usage.png)

### 6.4 Twenty-Year Annual Savings Projection

![20-year annual savings projection](outputs/figures/04_20_year_annual_savings_projection.png)

### 6.5 Investment Appraisal Comparison

![Investment appraisal comparison](outputs/figures/05_investment_appraisal_comparison.png)

## 7. Technology Stack

| Tool | Application |
|---|---|
| 🐍 Python | Core analytical programming |
| 📓 Jupyter Notebook | Model development and documentation |
| 🐼 Pandas | Data preparation, transformation and aggregation |
| 🔢 NumPy | Numerical calculations and simulation |
| 📊 Matplotlib | Analytical visualisations |
| 🎨 Seaborn | Statistical and comparative visualisation |

## 8. Repository Deliverables

| Folder / File | Description |
|---|---|
| Jupyter Notebook | Executable Python analysis and modelling workflow |
| Technical Documentation | Detailed methodology, assumptions and calculations |
| `outputs/figures/` | Five project charts |
| `outputs/tables/` | Monthly energy summary and validation results |
| `outputs/financial_results/` | Financial projections and investment appraisal outputs |
| `requirements.txt` | Python package dependencies |

### Supporting Analysis

- [Monthly Energy Summary](outputs/tables/monthly_energy_summary_2020.csv)
- [Model Validation Summary](outputs/tables/model_validation_summary.csv)
- [20-Year Savings Projection](outputs/financial_results/20_year_savings_projection_2022_2041.csv)
- [Investment Appraisal Comparison](outputs/financial_results/investment_appraisal_comparison.csv)

## 9. Skills Demonstrated

- Data cleaning, validation and exploratory analysis.
- Python programming and numerical modelling.
- Time-series and hourly energy analysis.
- Battery charging and discharging simulation.
- Data visualisation and analytical reporting.
- Financial forecasting and scenario analysis.
- Net Present Value (NPV) and Internal Rate of Return (IRR).
- Model validation and business decision support.

## 10. Conclusion

This project demonstrates how historical operational data can be transformed into an analytical model that supports investment decision-making.

By combining hourly energy modelling, battery storage simulation and long-term financial appraisal, the analysis provides a structured basis for understanding the potential financial value of battery storage.

The model also demonstrates the importance of validating assumptions, testing scenarios and evaluating investment decisions using both operational and financial measures.

---

<p align="center">
  <strong>Developed by Wycliffe Adek</strong><br/>
  Data Analyst | Business Intelligence | Financial Analytics
</p>

<p align="center">
  <sub>Data Analyst Assessment · 2026</sub>
</p>
<p align="center">
  <img src="assets/wycliffe-adek.jpg" alt="Wycliffe Adek - Data Analyst" width="170" />
</p>

<h1 align="center">Wycliffe Adek</h1>

<p align="center">
  <strong>Data Analyst | Business Intelligence | Financial Analytics</strong>
</p>

<p align="center">
  <em>Turning Data into Insights. Supporting Better Business Decisions.</em>
</p>

---

