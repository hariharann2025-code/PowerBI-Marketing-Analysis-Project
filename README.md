# 📊 Marketing Campaign Analysis

## 📌 Project Overview

The **Marketing Campaign Analysis** project analyzes marketing campaign performance using data analytics and visualization techniques.

The goal of this project is to understand **campaign effectiveness, customer engagement, regional performance, conversion rates, and overall marketing ROI**. The analysis helps identify which campaigns and regions are performing well and where improvements are required.

---

## 🎯 Objectives

* Analyze overall marketing campaign performance.
* Compare the performance of different campaigns.
* Identify high-performing and low-performing regions.
* Analyze customer engagement and conversion rates.
* Measure campaign ROI and revenue generated.
* Identify trends and patterns in marketing performance.
* Provide actionable insights to improve future campaigns.

---

## 🗂️ Dataset

The project uses the following datasets:

### 1. Marketing Campaign Details

Contains information about individual marketing campaigns.

**Key columns may include:**

* Campaign ID
* Campaign Name
* Campaign Type
* Start Date
* End Date
* Target Audience
* Marketing Channel
* Budget

### 2. Marketing Campaign Performance

Contains performance-related metrics for each campaign.

**Key columns may include:**

* Campaign ID
* Impressions
* Clicks
* Leads
* Conversions
* Revenue
* Cost
* Engagement

### 3. Region Performance

Contains marketing performance information based on geographical regions.

**Key columns may include:**

* Region
* Campaign ID
* Leads
* Conversions
* Revenue
* Cost

---

## 🛠️ Tools & Technologies

* **Power BI** – Data visualization and dashboard development
* **Power Query** – Data cleaning and transformation
* **DAX** – Calculated measures and KPIs
* **Excel / CSV** – Data sources
* **SQL** – Data analysis and querying
* **Python** – Data analysis and preprocessing

---

## 🔄 Project Workflow

```text
Raw Data
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
Data Modeling
   ↓
DAX Measures
   ↓
Data Visualization
   ↓
Marketing Insights
   ↓
Business Recommendations
```

---

## 🧹 Data Cleaning & Transformation

The following data preprocessing steps were performed using **Power Query**:

* Removed duplicate records.
* Handled missing values.
* Corrected data types.
* Renamed columns where required.
* Standardized categorical values.
* Created calculated columns where required.
* Merged and transformed datasets.
* Validated relationships between tables.

---

## 🧩 Data Model

The datasets were connected using common fields such as **Campaign ID** and **Region**.

A suitable relational/data-modeling approach was used to establish relationships between:

```text
Marketing Campaign Details
          │
          │ Campaign ID
          ↓
Marketing Campaign Performance
          │
          │ Region
          ↓
    Region Performance
```

---

## 📐 Key KPIs

The dashboard focuses on important marketing KPIs such as:

### Total Campaign Cost

```DAX
Total Cost = SUM(Marketing_Campaign_Performance[Cost])
```

### Total Revenue

```DAX
Total Revenue = SUM(Marketing_Campaign_Performance[Revenue])
```

### Total Leads

```DAX
Total Leads = SUM(Marketing_Campaign_Performance[Leads])
```

### Total Conversions

```DAX
Total Conversions = SUM(Marketing_Campaign_Performance[Conversions])
```

### Conversion Rate

```DAX
Conversion Rate =
DIVIDE(
    [Total Conversions],
    [Total Leads],
    0
) * 100
```

### ROI

```DAX
ROI =
DIVIDE(
    [Total Revenue] - [Total Cost],
    [Total Cost],
    0
) * 100
```

---

## 📊 Dashboard

The Power BI dashboard provides interactive visualizations for:

* 📌 Total Revenue
* 📌 Total Marketing Cost
* 📌 Total Leads
* 📌 Total Conversions
* 📌 Conversion Rate
* 📌 ROI
* 📌 Campaign-wise performance
* 📌 Region-wise performance
* 📌 Marketing channel performance
* 📌 Revenue and conversion trends

Users can interact with the dashboard using filters and slicers such as:

* Campaign
* Region
* Marketing Channel
* Campaign Type
* Date

---

## 🔍 Key Analysis Areas

### Campaign Analysis

Compare different campaigns based on:

* Cost
* Revenue
* Leads
* Conversions
* Conversion Rate
* ROI

### Regional Analysis

Analyze how different regions contribute to:

* Revenue
* Leads
* Conversions
* Campaign effectiveness

### Channel Analysis

Evaluate marketing channels based on their ability to generate:

* Customer engagement
* Leads
* Conversions
* Revenue

---

## 💡 Business Insights

The analysis can help businesses:

* Identify campaigns generating higher returns.
* Understand which regions have stronger customer engagement.
* Identify underperforming campaigns.
* Compare marketing channels.
* Optimize marketing budgets.
* Improve customer conversion rates.
* Make data-driven marketing decisions.

---

## 📁 Project Structure

```text
Marketing-Campaign-Analysis/
│
├── Dataset/
│   ├── Marketing_Campaign_Details.csv
│   ├── Marketing_Campaign_Performance.csv
│   └── Region_Performance.csv
│
├── PowerBI/
│   └── Marketing_Campaign_Analysis.pbix
│
├── Screenshots/
│   └── Dashboard.png
│
└── README.md

