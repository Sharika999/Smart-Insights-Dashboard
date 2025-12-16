# Smart Insights Dashboard – E-Commerce Analytics

An **interactive analytics dashboard** designed to convert raw e-commerce data into **clear, actionable insights**.  
Built with **Python**, **Streamlit**, and **Plotly**, this project demonstrates **data storytelling**, combining KPIs, cohort analysis, and dynamic visualizations in a single interface.

---

## Project Summary

This dashboard simulates a complete analytics workflow for an e-commerce business.  
It covers **data ingestion, cleaning, analysis, and reporting**, providing insights on sales trends, customer behavior, and product performance.

The dataset used is synthetic, representing **4,000+ transactions over 2 years**, with **1,600+ customers** from multiple countries and product categories.

---

<img width="1358" height="443" alt="image" src="https://github.com/user-attachments/assets/185eecb9-1ea3-4084-a712-d1e9f1281c46" />


## Goals

1. **Transform raw data into insights:** Turn large datasets into interactive visual stories.  
2. **Provide analyst-friendly controls:** Filter by country, category, sales channel, and timeframe.  
3. **Enable data-driven decisions:** Identify top-performing products, categories, and customer segments.  
4. **Showcase advanced analytics:** Perform cohort retention and RFM analysis for customer segmentation.

---

## Metrics Tracked

| Metric | Meaning |
|--------|---------|
| **Revenue** | Total sales after discounts |
| **Profit** | Revenue minus cost |
| **Orders** | Number of individual transactions |
| **Customers** | Number of unique buyers |
| **AOV (Average Order Value)** | Average revenue per transaction |
| **Profit Margin %** | Profit ÷ Revenue |

---

## Features & Visualizations

- **KPI Overview** – Quick glance at revenue, profit, orders, and AOV  
- **Sales Trends** – Month-by-month revenue and profit charts  
- **Product & Category Insights** – Identify best-selling items and categories  
- **Channel Revenue Share** – Pie charts showing sales by channel  
- **Geographical Sales** – Country-to-city breakdowns  
- **Customer Retention Analysis** – Cohort tracking for repeat buyers  
- **RFM Segmentation** – Classify customers into groups like “Loyal”, “Active”, or “New”

---

## Tech Stack

| Component | Purpose |
|-----------|---------|
| **Python** | Data wrangling and analysis |
| **Pandas / NumPy** | Dataset manipulation and KPI computation |
| **Streamlit** | Web-based dashboard UI |
| **Plotly** | Interactive charts |
| **Scikit-Learn** | RFM modeling and segmentation |
| **Statsmodels / Prophet** | Optional forecasting for trends |
| **Great Expectations / Pandera** | Optional data validation |

---

## Quick Start

### Clone Repository
```bash
git clone https://github.com/yourusername/Smart-Insights-Dashboard.git
cd Smart-Insights-Dashboard

### Folder Structure

SmartInsightsDashboard/
├── data/
│   └── orders.csv              # Synthetic e-commerce dataset
├── app/
│   ├── app.py                  # Streamlit main dashboard
│   └── utils/
│       └── data_utils.py       # Functions for KPIs, cohort & RFM
├── requirements.txt
└── README.md



## Install Dependencies
pip install -r requirements.txt
## Run Dashboard
streamlit run app/app.py
The dashboard will open at http://localhost:8501/.

## Use Your Own Dataset
export ORDERS_CSV=/path/to/your/orders.csv
# On Windows PowerShell
$env:ORDERS_CSV="C:\path\orders.csv"

Your dataset should include:
order_id, order_date, customer_id, country, city, channel, product_id, category, subcategory, unit_price, quantity, discount, revenue, cost.
