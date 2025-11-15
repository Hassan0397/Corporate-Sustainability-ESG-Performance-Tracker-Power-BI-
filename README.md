# 🌍 Corporate Sustainability & ESG Performance Tracker (Power BI)

A professional **ESG (Environmental, Social, Governance) Performance Tracking Dashboard** built in **Power BI** for multinational corporations.  
This dashboard provides executives with clear insights into **carbon emissions**, **diversity**, **governance compliance**, and overall **ESG Index Scores**.

The project demonstrates strong capabilities in:  
**Data Modeling → Power Query → DAX Measures → ESG KPIs → Executive Dashboard Design**

---

## 🚀 Project Overview
This ESG dashboard enables organizations to:
- Track sustainability performance over time  
- Compare ESG progress across regions  
- Analyze carbon emissions & renewable energy usage  
- Monitor diversity, training hours, and governance incidents  
- Provide executives a single view of overall ESG score  

---

## 📦 Project Workflow

### 🟦 1. Data Preparation
Created realistic ESG datasets (CSV format):
- `fact_Environmental.csv` → CO₂ emissions, energy usage, waste data  
- `fact_Social.csv` → diversity %, training hours, community investment  
- `fact_Governance.csv` → compliance incidents, board gender diversity  
- `dim_Date.csv` → calendar table  
- `dim_Region.csv` → region & country mapping  

Data prep included:
- Clean naming conventions  
- Removing duplicates  
- Ensuring numeric accuracy  
- Converting percentages to decimal formats  

---

### 🟩 2. Data Load
Imported all CSV files using **Power BI Desktop → Get Data → CSV**.

Verified data types:
- Emissions/Waste → Decimal  
- Energy (MWh) → Decimal  
- % Fields → Decimal/Percentage  
- Date → Date  
- IDs → Whole Number  

---

### 🟨 3. Data Modeling
Built a **Star Schema** with segregated ESG fact tables.

**Fact Tables**
- `fact_Environmental`  
- `fact_Social`  
- `fact_Governance`

**Dimension Tables**
- `dim_Date`  
- `dim_Region`

Relationships:
- Each fact table → `dim_Date[Date]`  
- Each fact table → `dim_Region[RegionID]`  

Marked `dim_Date` as the **official Date Table**.

---

### 🟧 4. Transformations (Power Query)
Performed data cleaning and structure alignment:
- Renamed columns → business-friendly names  
- Standardized casing (Region, Category)  
- Replaced nulls with zeros or defaults  
- Ensured data type accuracy  
- Created calculated columns for ESG categories  

---

### 🟥 5. Core DAX Measures

#### 🌿 Environmental KPIs
- Total CO₂ Emissions (Tons)  
- Renewable Energy Usage %  
- Waste Recycled %  
- Energy Consumption (MWh)  

#### 🧑‍🤝‍🧑 Social KPIs
- Diversity %  
- Avg Training Hours per Employee  
- Total Community Investment ($)  

#### 🏛 Governance KPIs
- Total Compliance Incidents  
- Board Diversity %  
- Governance Score  

#### ⭐ ESG Score (Composite Index)
- ESG Index Score = Weighted Avg of (Environmental + Social + Governance) metrics  

All measures formatted (%, Decimal, Currency) with clear naming conventions.

---

## 🖥️ Executive ESG Overview Dashboard

### 📸 ESG Dashboard Screenshot

[ESG Overview](https://github.com/Hassan0397/Corporate-Sustainability-ESG-Performance-Tracker-Power-BI-/blob/main/Corporate%20Sustainability%20Executive%20Overview.png)  


### Dashboard Components
- **KPI Cards:**  
  - ESG Index Score  
  - Total CO₂ Emissions  
  - Diversity %  
  - Compliance Incidents  

- **Slicers:** Year, Region, ESG Category  

- **Visuals:**  
  - **Line Chart:** CO₂ & Renewable Energy Trend  
  - **Bar Chart:** Diversity & Training Hours Comparison  
  - **Map:** Global CO₂ emissions / ESG score by region  
  - **Table:** Governance incidents with severity indicators  

## 🛠 Tools Used
- **Microsoft Power BI Desktop**  
- **Power Query**  
- **DAX (Data Analysis Expressions)**  
- **CSV Data Files**  

---

## ✅ Outcome
With this ESG dashboard, executives can:
- Monitor sustainability progress  
- Compare environmental impact across regions  
- Track diversity, inclusion, and training investments  
- Evaluate governance health through compliance metrics  
- View annual ESG Index scores  
- Make data-driven decisions on long-term sustainability strategy 



