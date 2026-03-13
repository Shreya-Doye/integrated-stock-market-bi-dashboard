# Stock Market Business Intelligence Dashboard (Power BI)

## Overview

This project presents an **Integrated Business Intelligence Dashboard** developed using **Power BI** to analyze historical stock market performance over a **10-year period (2014–2023)**.

The dashboard combines two datasets to provide insights into **stock performance, sector-wise market capitalization, and trading volume trends**. It enables users to explore market behavior, identify sector dominance, and evaluate long-term performance of major companies.

This solution demonstrates how raw financial data can be transformed into **interactive visual insights for data-driven investment analysis**.

---

## Datasets Used

### 1. Historical Stock Price Dataset

* Source: Kaggle (Anita Rostami)
* Contains daily stock trading data for major companies
* Time Period: **January 2014 – December 2023**

**Key Columns**

* Date
* Open
* High
* Low
* Close
* Adjusted Close
* Volume
* Ticker

**Tickers Included**
AAPL, MSFT, JPM, GS, AMZN, PG, KO, JNJ, XOM, CAT

---

### 2. S&P 500 Company Metadata

* Source: Kaggle (Andrew Marquez)
* Provides company-level metadata

**Key Columns**

* Company Name
* Ticker
* Sector
* Industry
* Market Capitalization

This dataset is used to **map companies to sectors and analyze sector-level market dominance**.

---

## Dashboard Features

The Power BI dashboard provides the following analytical capabilities:

* 📈 **Stock Price Trend Analysis**
  Visualize historical stock performance across 10 years.

* 🏢 **Sector-wise Market Capitalization**
  Compare sectors such as Technology, Financial Services, Healthcare, Energy, and Consumer Goods.

* 📊 **Trading Volume Analysis**
  Identify trading activity patterns across companies and years.

* 📅 **Year-based Filtering**
  Analyze specific years (e.g., 2023) using slicers and filters.

* 🔍 **Interactive Drilldowns**
  Explore deeper insights through tooltips and interactive visuals.

---

## Key Metrics

The dashboard computes several KPIs using **DAX measures**:

* **Total Close Value:** 2.97M
* **Total Market Capitalization:** 56T
* **Total Trading Volume:** 796B

Example DAX Measures:

```DAX
Total Close = SUM(StockData[Close])

Total Market Cap = SUM(SP500[Market Cap])

Total Volume = SUM(StockData[Volume])
```

---

## Tools & Technologies

* **Power BI Desktop** – Dashboard development and visualization
* **Power Query** – Data cleaning and transformation
* **DAX (Data Analysis Expressions)** – KPI calculations
* **CSV Datasets** – Data sources
* **GitHub** – Project hosting and documentation

---

## Dashboard Preview

### Main Dashboard

![Dashboard Overview](images/dashboard_overview.png)

### Sector Market Analysis

![Sector Analysis](images/sector_analysis.png)

### Stock Trend Visualization

![Stock Trend](images/stock_trend.png)

### Trading Volume Insights

![Volume Analysis](images/volume_analysis.png)

---

## Business Impact

This dashboard enables **portfolio managers, financial analysts, and investment researchers** to:

* Track long-term performance of major stocks
* Identify dominant sectors in the market
* Analyze trading activity patterns
* Discover potential investment opportunities
* Make **data-driven financial decisions**

---

## How to Use

1. Clone or download this repository
2. Open the `.pbix` file using **Power BI Desktop**
3. If prompted, load the datasets located in the `data/` folder
4. Interact with slicers and filters to explore the dashboard

---

## Future Improvements

Planned enhancements include:

* Integration of **real-time financial APIs** (Yahoo Finance / Alpha Vantage)
* Implementation of **predictive analytics models** such as ARIMA and LSTM for stock forecasting
* Expansion to include more stocks from NASDAQ and NYSE
* Automated alerts for price thresholds
* Mobile-optimized Power BI dashboard

---

## Conclusion

This project demonstrates how **business intelligence tools can transform raw financial data into actionable insights**.

By combining historical stock data with company metadata, the dashboard provides a comprehensive view of **market performance, sector trends, and trading patterns**, helping stakeholders better understand financial markets and make informed investment decisions.

---

## Author

**Shreya Doye**
Computer Science Student | Data Analytics Enthusiast
