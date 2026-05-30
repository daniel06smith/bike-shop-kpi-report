# Bike Shop 2-Year KPI Analysis

A Power BI dashboard analysing two years (2021–2022) of bike shop performance data,
with a focus on revenue, ridership, and profitability trends across time and season.
Data was sourced via SQL Server Management Studio (SSMS) and imported directly into
Power BI through a live database connection.

---

## Overview

This dashboard provides a high-level summary of key commercial metrics for a bike shop
operation, enabling analysis of rider demographics, seasonal revenue patterns, and
hourly performance across weekdays.

---

## Preview

<img width="1189" height="665" alt="image" src="https://github.com/user-attachments/assets/36ccf387-f518-4973-b0d7-f49781acf80b" />

---

## Data Source

- **Database:** SQL Server
- **Connection Tool:** SQL Server Management Studio (SSMS)
- **Method:** Direct database connection to Power BI via SSMS data import

---

## KPI Summary (Header)

| Metric | Value |
|---|---|
| **Profit Margin** | 0.45 |
| **Riders** | 3M |
| **Sum of Profit** | 10.45M |
| **Sum of Revenue** | $15M |

A **year slicer** allows filtering between Year 0 (2021) and Year 1 (2022).

---

## Visuals

### 1. Average Revenue | Weekday - Hour (Matrix + Bar Chart)
Displays average revenue segmented by **weekday (0–6)** and **hour of day (8–20)**.
The bar chart summarises average revenue by weekday, while the matrix beneath it
provides a granular hourly breakdown for each day, supporting operational scheduling
decisions.

---

### 2. Average Revenue | Season (Bar Chart)
Horizontal bar chart comparing average revenue across four seasons:
Summer, Spring, Fall, and Winter. Summer consistently shows the highest average
revenue, informing inventory and staffing strategies by season.

---

### 3. Rider Type Demographics (Donut Chart)
Breaks down the rider base by type:

- **Registered riders** — 3M (81.17%)
- **Casual riders** — 1M (18.83%)

Highlights the dominance of the registered rider segment in overall volume.

---

### 4. Number of Riders, Average Revenue, and Average Profit | Year - Month (Line + Column Chart)
A dual-axis chart tracking monthly trends across 2021 and 2022.

- **Columns** — sum of riders per month
- **Lines** — average profit and average revenue overlaid on a secondary axis

Enables identification of seasonal peaks and year-over-year growth patterns.

---

## Setup & Usage

1. Open the `.pbix` file in **Power BI Desktop**
2. Ensure a connection to the SQL Server database is available
3. Refresh the dataset to pull the latest data via SSMS
4. Use the **year slicer** (top right) to filter between 2021 and 2022

---

## Requirements

- Power BI Desktop (latest recommended)
- SQL Server Management Studio (SSMS)
- Access to the underlying SQL Server database
