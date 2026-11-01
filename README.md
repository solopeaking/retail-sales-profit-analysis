# Retail Sales & Profit Analysis

## Project Overview

This project focuses on analyzing retail sales data to understand business performance, identify profitable and loss-making products, evaluate category performance, and investigate the relationship between discounts and profitability.

The analysis uses Python and Pandas to clean, explore, and interpret retail transaction data, with the objective of turning raw data into meaningful business insights that can support better business decisions.

**Project Status:** In Progress

## Business Objectives

The main objectives of this project are:

- Understand overall sales and profitability.
- Identify the highest-performing and least-profitable product categories.
- Find the most profitable and loss-making products.
- Analyze the relationship between discounts and profit.
- Examine sales and profit trends over time.
- Identify potential areas where business performance can be improved.

## Dataset

The project uses a Superstore retail sales dataset stored at:

`data/raw/superstore.csv`

The dataset contains retail transaction information, including fields related to:

- Order and shipping dates
- Customer and order details
- Product names and categories
- Sales and quantity
- Discount
- Profit
- Geographical information

The working dataset contains **9,001 records** after removing fully empty rows.

The order date range covered by the current analysis is **January 3, 2015, to December 30, 2018**.

## Tools and Technologies

- **Python 3.13** — Programming and data analysis
- **Pandas** — Data cleaning, manipulation and exploratory data analysis
- **NumPy** — Numerical computing
- **Jupyter Notebook** — Interactive analysis and documentation
- **Git & GitHub** — Version control and project management

## Project Workflow

### 1. Data Loading and Exploration

- Imported the dataset using Pandas.
- Explored the dataset structure and columns.
- Inspected data types and basic statistical information.
- Identified fully empty rows and prepared the working dataset.

### 2. Data Cleaning

- Removed fully empty rows from the working dataset.
- Checked missing values.
- Checked duplicate records.
- Converted Order Date and Ship Date into datetime format.
- Validated date information before performing further analysis.

**Current data quality checks:**
- Missing values in the cleaned working dataset: 0
- Duplicate records: 0

### 3. Date and Shipping Analysis

Analyzed order dates, shipping dates and shipping delays.

Key findings:
- Order dates range from January 3, 2015, to December 30, 2018.
- Shipping dates range from January 7, 2015, to January 5, 2019.
- Average shipping delay is approximately 4 days.
- Median shipping delay is 4 days.
- Shipping delays range from 0 to 7 days.

### 4. Category-Wise Sales and Profitability Analysis

Analyzed total sales, total profit, losses and profit margins across product categories.

| Category | Total Sales | Net Profit Margin |
|---|---:|---:|
| Furniture | $659,820.84 | 2.30% |
| Office Supplies | $636,354.15 | 16.79% |
| Technology | $779,451.74 | 17.51% |

**Initial observations:**
- Technology generated the highest sales and net profit.
- Office Supplies maintained a strong profit margin.
- Furniture had the lowest profit margin, indicating an area that needs further investigation.

### 5. Product-Level Profitability Analysis

Grouped products by name and calculated their total profit.

The analysis identified:
- Top 10 most profitable products.
- Top 10 loss-making products.
- Highest profit-generating product.
- Product with the greatest accumulated loss.

**Key findings:**
- Canon imageCLASS 2200 Advanced Copier was the highest profit-generating product, with approximately $25,199.93 in profit.
- Cubify CubeX 3D Printer Double Head Print was the largest loss-making product, with approximately $8,879.97 in losses.

### 6. Discount and Profitability Analysis

Investigated how different discount levels relate to product profitability.

The analysis includes:
- Discount distribution.
- Average and maximum discount.
- Total profit by discount level.
- Average profit by discount level.
- Loss-making records at each discount level.
- Percentage of loss-making records at each discount level.

**Preliminary observations:**
- At 0% discount, no loss-making records were observed.
- At 30% discount, approximately 91.26% of records were loss-making.
- At 40% discount, approximately 88.17% were loss-making.
- At discount levels of 32%, 45%, 50%, 60%, 70%, and 80%, all observed records were loss-making.
- The 20% discount level had the highest count of loss-making records, with 454 records.

These results indicate an association between certain higher discount levels and loss-making transactions. Further analysis is required before drawing conclusions about causation or recommending pricing changes.

## Overall Business Performance

The current analysis has identified the following overall figures:

| Metric | Value |
|---|---:|
| Total Sales | $2,075,626.73 |
| Total Positive Profit | $399,949.19 |
| Total Losses | $141,431.16 |
| Net Profit | $258,518.03 |
| Net Profit Margin | 12.45% |

These figures provide an initial overview of the business's financial performance.

## Repository Structure

```text
retail-sales-profit-analysis/
│
├── data/
│   └── raw/
│       └── superstore.csv
│
├── notebooks/
│   └── sales.ipynb
│
├── reports/
├── sql/
│
├── README.md
└── .gitignore
```

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/solopeaking/retail-sales-profit-analysis.git
```

### 2. Navigate to the Project Directory

```bash
cd retail-sales-profit-analysis
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Environment (Windows PowerShell)

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

```bash
python -m pip install pandas numpy jupyter
```

### 6. Open the Jupyter Notebook

```bash
jupyter notebook notebooks/sales.ipynb
```

Run the notebook cells sequentially.

## Planned Improvements

The following work is planned to complete the project:

- Complete time-based sales and profit analysis.
- Finish discount-related analysis and business conclusions.
- Perform additional exploratory data analysis.
- Create meaningful data visualizations.
- Develop SQL queries for important business questions.
- Add final business insights and recommendations.
- Improve notebook organization and documentation.

## Project Objective

The ultimate goal is to demonstrate practical data analysis skills, including data cleaning, exploratory data analysis, aggregation, profitability analysis, SQL, visualization, and business interpretation.

This project is being developed as part of my Data Analyst learning journey and portfolio.

---

**Repository:** [Retail Sales & Profit Analysis](https://github.com/solopeaking/retail-sales-profit-analysis)

**Author:** [Your Name]