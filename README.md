# 📊 Sales Data Analysis

> An end-to-end exploratory data analysis (EDA) of a retail sales dataset covering 9,800 transactions — featuring data cleaning, feature engineering, business insights, and rich visualizations.

![Python](https://img.shields.io/badge/Python-3.13-3776AB?style=flat-square&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-2.x-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.x-013243?style=flat-square&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-11557C?style=flat-square)
![Status](https://img.shields.io/badge/status-completed-brightgreen?style=flat-square)

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Tech Stack](#-tech-stack)
- [Project Workflow](#-project-workflow)
- [Analysis Highlights](#-analysis-highlights)
- [Key Insights](#-key-insights)
- [Visualizations](#-visualizations)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Results Summary](#-results-summary)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 🔍 Overview

This project explores a retail sales dataset to uncover patterns across **categories, regions, products, and time**. It demonstrates a complete data analysis pipeline — from raw data to actionable business insights — using Python and Jupyter Notebook.

The analysis is designed to answer questions like:

- Which product categories and regions drive the most revenue?
- How has sales performance changed year over year?
- Which products and months perform best?
- Where is the data quality lacking, and how do we handle it?

---

## 📁 Dataset

**Location:** `data/sales_data.csv`

- **Rows:** 9,800
- **Columns:** 18
- **Time Range:** 2015 – 2018
- **Regions Covered:** West, East, Central, South

| Column | Description |
|---|---|
| Row ID | Unique row identifier |
| Order ID | Order identifier |
| Order Date | Date the order was placed |
| Ship Date | Date the order was shipped |
| Ship Mode | Shipping method |
| Customer ID | Unique customer identifier |
| Customer Name | Name of the customer |
| Segment | Customer segment |
| Country | Country of the customer |
| City | City of the customer |
| State | State of the customer |
| Postal Code | Postal code |
| Region | Sales region |
| Product ID | Unique product identifier |
| Category | Product category |
| Sub-Category | Product sub-category |
| Product Name | Name of the product |
| Sales | Sales amount |

---

## 🛠 Tech Stack

| Tool | Purpose |
|---|---|
| **Python 3** | Core programming language |
| **pandas** | Data loading, cleaning, and transformation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Jupyter Notebook** | Interactive analysis environment |

---

## 🔄 Project Workflow

### 1. Data Loading & Inspection
- Loaded the CSV into a pandas DataFrame
- Inspected shape, columns, data types, and summary statistics

### 2. Data Cleaning
- Checked for missing values and duplicates
- Converted `Order Date` and `Ship Date` to `datetime`
- Converted `Postal Code` to nullable integer type
- Preserved 11 missing postal codes (no known value for Burlington, Vermont)

### 3. Feature Engineering
- Extracted `Year` and `Month` from `Order Date`
- Created a `Date` column for monthly time-series analysis

### 4. Analysis
- Sales by **Category**
- Sales by **Region**
- Top **Products** by sales
- **Monthly** and **Yearly** sales trends
- **Year-over-Year** growth

### 5. Visualization
- Bar charts, horizontal bar charts, and line charts using Matplotlib

---

## 📈 Analysis Highlights

| Analysis | Description |
|---|---|
| **Category Sales** | Revenue breakdown by product category |
| **Region Sales** | Revenue breakdown by region |
| **Top Products** | Top 10 products by total sales |
| **Monthly Trend** | Sales movement month by month |
| **Peak & Low Months** | Best and worst performing months |
| **Yearly Sales** | Annual sales totals |
| **YoY Growth** | Percentage growth year over year |

---

## 💡 Key Insights

- 📌 **Technology** generated the highest total sales across all categories.
- 📌 The **West region** led in total sales, followed by the **East region**.
- 📌 Sales **dipped by 4.26%** in 2016 compared with 2015.
- 📌 Sales **rebounded by 30.64%** in 2017 and grew a further **20.30%** in 2018.
- 📌 **November 2018** recorded the highest monthly sales in the dataset.
- 📌 The **Canon imageCLASS 2200 Advanced Copier** was the top-selling product.
- 📌 Eleven `Postal Code` values were missing and preserved as missing due to no known postal code for Burlington, Vermont.

---

## 📊 Visualizations

The notebook produces the following charts:

| Chart | Type |
|---|---|
| Total Sales by Category | Bar |
| Total Sales by Region | Bar |
| Top 10 Products by Sales | Horizontal Bar |
| Monthly Sales Trend | Line |
| Yearly Sales | Bar |

> 💡 *Screenshots can be added under a `screenshots/` folder for visual reference.*

---

## 📂 Project Structure

```
sales-data-analysis/
│
├── data/
│   └── sales_data.csv        # Raw dataset
│
├── sales_analysis.ipynb      # Main analysis notebook
│
├── README.md                 # Project documentation
│
└── screenshots/              # (Optional) Charts & outputs
```

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/sales-data-analysis.git
cd sales-data-analysis
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib
```

### 3. Add the dataset

Place `sales_data.csv` inside the `data/` folder.

### 4. Launch the notebook

```bash
jupyter notebook sales_analysis.ipynb
```

### 5. Run all cells

Execute cells top to bottom to reproduce the analysis and charts.

---

## 📌 Results Summary

| Metric | Value |
|---|---|
| Total Transactions | **9,800** |
| Top Category | **Technology** |
| Top Region | **West** |
| Best Year (Sales) | **2018** |
| Best Month | **November 2018** |
| Top Product | **Canon imageCLASS 2200 Advanced Copier** |
| YoY Growth (2017) | **+30.64%** |
| YoY Growth (2018) | **+20.30%** |

---

## 🚀 Future Improvements

- [ ] Add interactive dashboards using **Plotly** or **Streamlit**
- [ ] Perform **customer segmentation** using RFM analysis
- [ ] Build a **sales forecasting** model with time-series techniques
- [ ] Add **profit and discount analysis** if data becomes available
- [ ] Automate reporting with **scheduled scripts**

---

## 👤 Author

**Amrit Rai**

- 🔗 LinkedIn: [linkedin.com/in/amrit-rai-data-analyst](https://www.linkedin.com/in/amrit-rai-data-analyst/)
- 📧 Email: amritrai1061@gmail.com
- 💼 Open to Data Analyst / Business Analyst roles

---

## 📝 License

This project is open for **learning and portfolio purposes**. Feel free to fork, explore, and build upon it.

---

⭐ *If you found this project helpful, consider giving it a star!*
