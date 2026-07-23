# 📊 Sales Data Cleaning, Exploration & Analysis Project

This repository contains a comprehensive Excel-based data analysis project covering end-to-end data processing—from raw data cleaning and normalization to statistical analysis and business intelligence reporting using Pivot Tables.

---

## 📌 Project Overview

The objective of this project is to clean, transform, and analyze a raw sales dataset to evaluate employee performance, product popularity, discount strategies, and demographic purchase patterns.

---

## 🛠️ Data Processing Lifecycle

### 1. Data Cleaning & Normalization
* **Text & Name Normalization**: Trimmed white spaces across text fields (`Sales Person`, `Customer Name`) and standardized naming conventions.
* **Percentage Formatting Fix**: Adjusted percentage representations (e.g., converting scaled integers like `3600%` to standard decimal values `0.36` / `36%`).
* **Calculated Fields**:
  * $$\text{Revenue} = \text{Quantity} \times \text{Price}$$
  * $$\text{Net Revenue} = \text{Revenue} - \text{Discount}$$
  * $$\% \text{ Discount} = \frac{\text{Discount}}{\text{Revenue}}$$

---

### 2. Descriptive Statistical Analysis

Descriptive statistics were computed across the dataset for **Discount** and **Net Revenue**:

| Statistic | Discount Value ($) | Net Revenue ($) |
| :--- | :---: | :---: |
| **Mean** | $30.35 | $263.37 |
| **Median** | $8.00 | $142.50 |
| **Mode** | $0.00 | $800.00 |
| **Standard Deviation** | $66.57 | $267.83 |
| **Total Sum** | **$3,186.25** | **$27,653.75** |

---

### 3. Key Business Insights & Mining Questions

Six Pivot Tables were built to answer core business questions:

1. **Sales Value by Customer**:
   * Top-performing customer accounts: `rami kareem` (**$7,817.50**) and `sami saeed` (**$6,950.50**).
2. **Top Selling Products (by Quantity)**:
   * **Headset**: 77 units
   * **Mouse**: 68 units
   * **Monitor**: 58 units
   * **Keyboard**: 58 units
   * **Laptop**: 15 units  
   *(Total Units Sold: 276)*
3. **Sales Percentage by Gender**:
   * **Male**: 90.94%
   * **Female**: 9.06%
4. **Discount Value by Discount Bracket**:
   * Identified that the lowest discount tier (`0.0001 - 0.2001`) accounted for the highest cumulative discount volume (**$1,762.25**).
5. **Sales Value by Month**:
   * Mapped monthly revenue distribution to evaluate seasonal sales trends.
6. **Quantity Sold by Employee per Product**:
   * Cross-tabulation of itemized performance per sales agent across product categories.
   * 📂 Project File: The complete dataset and working Excel file can be downloaded directly via Data analysis.xlsx.

---

## 📁 Repository Structure

```text
├── Data analysis.xlsx       # Primary Excel workbook containing raw data, cleaned tables, and Pivot Tables
└── README.md                # Project documentation and summary report
