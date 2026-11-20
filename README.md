# 🚗 Vehicle Sales Analysis | Power BI Dashboard

An interactive Power BI dashboard that analyzes **22 years (2002–2023)** of monthly new and used vehicle sales, covering both **sales volume** (units) and **sales revenue** ($).

---

## 🎯 Objective

Understand how vehicle sales changed over time by answering questions such as:

- How many vehicles are sold each year, and how is the market split between new and used?
- Is revenue growing because more cars are sold, or because prices are rising?
- How did economic shocks (the 2008–09 downturn, COVID-19) affect new vs. used sales?
- Which months and quarters are the strongest for sales?

---

## 🛠️ Tools & Skills

| Area | Details |
|---|---|
| **BI Tool** | Power BI Desktop |
| **Data Modeling** | Date dimension table (`DimDate`) related to the sales data, separate tables for Volume and Sales measures |
| **DAX** | Totals, ratios, percentages, YoY growth, Year-to-Date, Quarter-to-Date, Same Period Last Year |
| **Data Preparation** | Power Query |
| **Visualization** | KPI cards, line charts, donut charts, clustered bar charts, slicers, custom page navigation |

---

## 📂 Dataset
- **Period:** January 2002 – December 2023 (264 monthly records)
- **Columns:**

| Column | Description |
|---|---|
| `Year`, `Month` | Reporting period |
| `New`, `Used` | Number of new and used vehicles sold |
| `Total Sales New`, `Total Sales Used` | Sales revenue for new and used vehicles |

---

## 📊 Dashboard Pages

### 1. Volume
- KPI cards: **Total**, **New**, and **Used** vehicles sold, plus the **New-to-Used ratio**
- Total vehicles sold by year (line chart)
- New vs. used share of units (donut chart)
- New vs. used sales by month (clustered bar chart)
- Total vehicles sold vs. previous year (KPI visual) and **Used / New YoY %**
- Slicers: Year, Quarter, Month

### 2. Sales
- KPI cards: **Total**, **New**, and **Used** sales revenue
- Year-to-Date and Quarter-to-Date sales
- New vs. used share of revenue (donut chart)
- Total sales vs. same period last year (KPI visual)
- Total sales by year (line chart) and new vs. used sales by month (bar chart)
- Slicers: Year, Quarter, Month

---

## 🧮 DAX Measures

**Volume Measures:** Total Vehicle Sold, New Vehicle Sold, Used Vehicle Sold, New Vehicle Sold %, Used Vehicle Sold %, New To Used Ratio, Total Sales Previous Year, New YoY %, Used YoY %

**Sales Measures:** Total Vehicle Sales, New Total Sales, Used Total Sales, New Sales %, Used Sales %, Sales Same Period Last Year, Sales Total Quarter To Date, Sales Total Year To Date
---

## 💡 Key Insights

1. **Used cars dominate units, new cars dominate revenue.** Used vehicles are about **66%** of all units sold, but new vehicles bring in about **61%** of total revenue (average price ≈ **$30.9K** new vs. **$10.1K** used).
2. **Fewer cars, more revenue.** From 2002 to 2023, units sold fell by about **18%**, yet annual revenue grew by about **60%**, from **$14.5B to a record $23.2B**. The average price of a new vehicle rose by about **93%** over the same period.
3. **Used cars are more resilient in downturns.** Between 2005 and 2009, new-vehicle sales dropped about **41%**, while used-vehicle sales dropped only about **13%**.
4. **COVID-19 impact and rebound.** In 2020, units fell **17.3%** and revenue fell **12.2%**. Revenue then jumped **19.3%** in 2021, largely driven by higher prices, with the average used-car price about **40% higher** in 2023 than in 2019.
5. **Clear seasonality.** Sales are strongest from **March to August**, and **Q2 and Q3 together account for about 53%** of annual units. February, November, and December are the weakest months.

---

## 📁 Repository Structure

```
vehicle-sales-analysis/
├── README.md
├── VehicleSalesAnalysis.pbix
├── MVA_Vehicle_Sales_Counts_by_Month_for_Calendar_Year_2002_through_December_2023.csv 
└── volume-page.png
└── sales-page.png
  
```

## ▶️ How to Use

1. Download `VehicleSalesAnalysis.pbix`.
2. Open it with **Power BI Desktop** (free).
3. If prompted, update the data source path to point to the CSV file in the `data/` folder.

---

## 👤 Author

**Muhammed Mokhtar** — Data Analyst
📍 Alexandria, Egypt
🔗 [LinkedIn](https://linkedin.com/in/mohammed-mokhtar-3126a1167)
