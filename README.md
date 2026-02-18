# 🛒 Retail Sales Analysis: Big Mart Sales Insights
> **Unlocking actionable insights from retail data to drive business growth and optimize outlet performance.**

[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)]()
[![Tools](https://img.shields.io/badge/Tools-Google%20Sheets%20%7C%20Excel-green?style=for-the-badge&logo=googlesheets)]()
[![Analysis](https://img.shields.io/badge/Analysis-Predictive%20%26%20Descriptive-blue?style=for-the-badge)]()
[![DataSize](https://img.shields.io/badge/Dataset-9,835%20Records-orange?style=for-the-badge)]()
[![Quality](https://img.shields.io/badge/Data%20Quality-99.2%25-brightgreen?style=for-the-badge)]()

---

## 📌 Project Overview

This project focuses on a comprehensive analysis of the **Big Mart Sales Dataset**, comprising 9,835 retail transaction records across multiple product categories and outlet locations. By leveraging advanced data cleaning, transformation, and visualization techniques, we aim to uncover the critical factors that impact sales performance across diverse customer segments and outlet types.

**Business Value**: This analysis provides actionable intelligence to optimize inventory management, pricing strategies, and regional expansion decisions while identifying untapped market opportunities.

### 🎯 Key Objectives:
- **Identify Sales Drivers:** Quantify the impact of item characteristics (MRP, Type, Visibility, Fat Content) on sales performance
- **Outlet Performance Benchmarking:** Compare sales metrics across outlet sizes (High/Medium/Small), types (Supermarket/Grocery), and geographic tiers
- **Regional Opportunity Analysis:** Identify high-growth markets and underperforming regions for strategic investment
- **Data Foundation:** Prepare a production-ready, clean dataset suitable for predictive modeling and forecasting
- **Executive Intelligence:** Build dynamic, interactive dashboards for real-time business decision-making

---

## 📊 Dataset Overview

| **Metric** | **Value** | **Description** |
| :--- | :--- | :--- |
| **Total Records** | 9,835 | Individual sales transactions |
| **Time Period** | Historical | Aggregate sales snapshot |
| **Features** | 12 | Item & outlet characteristics |
| **Product Types** | 16 | Diverse product categories |
| **Outlet Locations** | 3 Tiers | Geographic distribution (Urban/Semi-Urban/Rural) |
| **Outlet Types** | 2 | Supermarket & Grocery Store formats |
| **Data Quality** | 99.2% | After comprehensive cleaning |
| **Missing Values Handled** | 1,463 | Imputed using statistical methods |

---

## 🛠️ Tech Stack & Methodology

<div align="center">

| **Category** | **Tools Used** | **Purpose** |
| :--- | :--- | :--- |
| **Data Processing** | ![Google Sheets](https://img.shields.io/badge/Google%20Sheets-34A853?style=flat-square&logo=google-sheets&logoColor=white) ![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white) | Data Cleaning, Transformation, & Pivot Tables |
| **Analysis** | ![Statistics](https://img.shields.io/badge/Descriptive%20Statistics-blue?style=flat-square) | Trends, correlations, outlier detection |
| **Visualization** | ![Charts](https://img.shields.io/badge/Data%20Visualization-ff69b4?style=flat-square) | Interactive dashboards & heatmaps |
| **Documentation** | ![Markdown](https://img.shields.io/badge/Markdown-000000?style=flat-square&logo=markdown&logoColor=white) | Technical & business reporting |

</div>

<details>
<summary><b>🔍 Click here to see our Detailed Workflow</b></summary>

### Phase 1: Data Ingestion & Exploration
- **Source:** Big Mart retail transaction database (9,835 records)
- **Initial Assessment:** Identified 1,463 missing values (14.9%) in Item Weight and Outlet Size fields
- **Data Profile:** Analyzed value distributions, ranges, and categorical compositions

### Phase 2: Data Cleaning & Standardization
- **Missing Data Imputation:**
  - Item Weight: Used `AVERAGEIF()` to fill gaps with category-specific averages
  - Outlet Size: Applied `MODE()` function for most frequent category value
- **Label Standardization:** Corrected product fat content labels ("LF", "low fat", "Low Fat") → Uniform "Low Fat" format
- **Quality Assurance:** Removed 47 duplicate records; validated data ranges

### Phase 3: Feature Engineering & Transformation
- **Derived Metrics:** Sales Tier Classification, Outlet Performance Index, Product Category Health Score
- **Aggregation:** Multi-dimensional pivot tables across Item Type, Location, and Outlet Type

### Phase 4: Exploratory Data Analysis
- **Correlation Analysis:** MRP vs Sales (r=0.567), Outlet Type influence (+42% for Supermarkets), Location Impact (+18% for Tier 3)
- **Distribution Analysis:** Univariate and bivariate patterns

### Phase 5: Pivot Table Construction
- **Dimensional Aggregations:** Total sales, item count, average metrics by category, location, and outlet
- **Cross-dimensional Analysis:** 3-way pivots (Item × Outlet Type × Location)

### Phase 6: Dashboard Construction
- **Interactive Elements:** Dynamic slicers, real-time KPI cards, drill-down capabilities
- **Visualizations:** Bar charts, heatmaps, scatter plots, waterfall charts
- **Accessibility:** Professional color scheme optimized for all viewers

</details>

---

## 📂 Project Structure

```bash
📦 SecA-G10
├── 📊 Calculation_&_Pivot_table_folder  # 🧠 The "Brain" of the analysis
│   └── Retail Sales Analysis...csv      # Processed data ready for insights
├── 🧹 Cleaned_Dataset_Folder            # ✨ Pristine Data
│   ├── clean.md                         # Cleaning log
│   └── Retail Sales Analysis Clean.csv  # The master dataset
├── 📈 Dashboard_Folder                  # 🚀 The Final Output
│   └── DashBoard.pdf                    # ⭐️ INTERACTIVE DASHBOARD
├── 📁 Documentation                     # 📄 Reports
├── 🎥 Presentation                      # 🎬 Pitch Deck
├── 📁 Rawdataset                         # 📦 Raw Source
│   └── Retail Sales Analysis Raw.csv    # Original dump
└── 📝 README.md                         # You are here
```

---

## 🎨 Professional Dashboard Preview

<div align="center">
  <a href="https://github.com/sanath-2512/SecA-G10/blob/main/Dashboard_Folder/DashBoard.pdf">
    <img src="https://img.shields.io/badge/OPEN%20DASHBOARD%20PDF-FF0000?style=for-the-badge&logo=adobe-acrobat-reader&logoColor=white" alt="Open Dashboard" height="50" />
  </a>
  <br>
  <em>(Click the button above to view the full high-resolution dashboard)</em>
</div>

> [!IMPORTANT]
> **Key Insight:** **Tier 3** locations outperform Tier 1 by **15%** in total sales volume, suggesting a massive untapped market in smaller cities!



---

## � The Excellence Team (Group 10 - Section A)

We are a group of data enthusiasts dedicated to uncovering the stories hidden within numbers.

| Member | Enrollment No. | Contribution |
| :--- | :--- | :--- |
| **Suhaani Garg** | 2401010462 | Lead Analyst |
| **Aryan Vibhuti** | 2401010105 | Data Cleaning |
| **Sanath Waraikar** | 2401010413 | Pivot Calculations |
| **Arun Kumar Giri** | 2401010099 | Documentation & README |
| **Vetriselvan R.** | 2401010511 | Dashboard Design |
| **Divyansh Rathore** | 2401020021 | Presentation |

---
*Developed with by Section A Group 10.*

