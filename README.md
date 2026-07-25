<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Montserrat&weight=800&size=30&pause=1000&color=E87722&center=true&vCenter=true&width=900&lines=Retail+Sales+Business+Intelligence;1997%E2%80%931998+Data+Analysis;3+Dashboards+%C2%B7+7+Regions+%C2%B7+25%2B+Stores" alt="Typing SVG" />

<br/>

![Excel](https://img.shields.io/badge/Excel-Power%20Query%20%7C%20Power%20Pivot%20%7C%20DAX-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)
![Data Period](https://img.shields.io/badge/Data%20Period-1997–1998-0A1628?style=for-the-badge&logo=clockify&logoColor=E87722)
![Transactions](https://img.shields.io/badge/Transactions-269%2C711-2E75B6?style=for-the-badge&logo=databricks&logoColor=white)
![Profit Margin](https://img.shields.io/badge/Profit%20Margin-59.67%25-00897B?style=for-the-badge&logo=chartdotjs&logoColor=white)

<br/>

> **Turning Raw Data into Business Decisions** — A full-stack BI solution analyzing retail performance across 7 regions, 25+ stores, and 2 fiscal years using Microsoft Excel's complete analytics stack.

</div>

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Dataset Summary](#-dataset-summary)
- [Tech Stack](#-tech-stack)
- [Dashboard 1 — Executive Overview](#-dashboard-1--executive-overview)
- [Dashboard 2 — Sales Performance](#-dashboard-2--sales-performance)
- [Dashboard 3 — Product Analytics](#-dashboard-3--product-analytics)
- [Key Findings](#-key-findings)
- [Strategic Recommendations](#-strategic-recommendations)
- [Color System](#-color-system)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)

---

## 🧭 Project Overview

This project delivers a three-dashboard Business Intelligence solution built entirely in Microsoft Excel. It covers the complete BI workflow: raw data ingestion via Power Query, relational modeling in Power Pivot, DAX measure development, and interactive PivotChart dashboards — all presented via a 17-slide Canva deck aligned to the dashboard color system.

| Attribute | Detail |
|---|---|
| **Data Period** | 1997 – 1998 (2 fiscal years) |
| **Total Transactions** | 269,711 |
| **Regions Analyzed** | 7 |
| **Stores Covered** | 25+ |
| **Dashboards Built** | 3 interactive |
| **Slides Produced** | 17 (Canva 16:9) |
| **Objective** | Identify revenue growth opportunities, reduce return rate below 2%, and improve store profitability |

---

## 📦 Dataset Summary

<details>
<summary><b>Click to expand — Data Sources & Schema</b></summary>

<br/>

| Table | Key Fields | Role in Model |
|---|---|---|
| **Sales** | OrderID, StoreID, ProductID, CustomerID, Revenue, Date | Fact table — central hub |
| **Customers** | CustomerID, Segment, AcquisitionYear | Customer dimension |
| **Products** | ProductID, ProductName, Brand, Category | Product dimension |
| **Stores** | StoreID, StoreName, Region | Store/geography dimension |
| **Region** | RegionID, RegionName | Region rollup dimension |
| **Returns** | OrderID, ReturnDate, Reason | Return analysis dimension |

All tables are loaded via **Power Query**, related in **Power Pivot (Data Model)**, and queried through **DAX** measures.

</details>

---

## 🛠 Tech Stack

```
Microsoft Excel
├── Power Query        → ETL: load, clean, transform all 6 tables
├── Power Pivot        → Relational data model (star schema)
├── DAX                → KPI measures: Revenue, Margin %, YoY Growth, AOV, Churn
├── PivotTables        → Aggregations driving all chart data
├── PivotCharts        → Bar, combo, column, and line visuals
└── Slicers            → Interactive filters: Year, Region, Store

Canva (16:9 Presentation)
└── 17 slides aligned to dashboard design system
```

---

## 📊 Dashboard 1 — Executive Overview

### KPIs at a Glance

| Metric | Value | Signal |
|---|---|---|
| 💰 Total Revenue | **$1,764,494.87** | Full period 1997–1998 |
| 📈 Gross Profit | **$1,052,789.03** | — |
| 📊 Profit Margin % | **59.67%** | ✅ Strong — 2× industry average |
| 🛒 Total Orders | **269,711** | — |
| ↩️ Return Rate | **2.63%** | ⚠️ Monitor — target < 2% |
| 🆕 New Customers | **3,261** | Acquired during period |
| 💔 Lost Customers | **782** | Churned — action needed |

<details>
<summary><b>Visuals in this dashboard</b></summary>

<br/>

**Monthly Revenue & Profit Margin Trend (Combo Chart)**
- Blue clustered bars = monthly revenue (Apr 1997 → Sep 1998)
- Orange line overlay = profit margin % (right axis)
- Revenue grew consistently into 1998; margin held above 59% throughout

**Revenue by Region (Horizontal Bar)**
- 7 regions ranked by total revenue
- North West leads at ~$870K; Central West is lowest priority turnaround region
- Top 2 regions generate 52% of all revenue

</details>

---

## 📈 Dashboard 2 — Sales Performance

### Period KPIs

| Metric | Value |
|---|---|
| 📅 Revenue 1997 | **$565,233.03** |
| 📅 Revenue 1998 | **$1,199,261.84** |
| 📆 Revenue MTD | **$120,160.84** |
| 📊 Revenue QTD | **$326,369.10** |
| 🛍️ Avg Order Value | **$6.54** |

**Year-over-Year Growth: +112%** — $634K incremental revenue in a single year.

<details>
<summary><b>Visuals in this dashboard</b></summary>

<br/>

**Top 10 vs Bottom 10 Stores (Dual Horizontal Bar)**

| Rank | Top Store | Revenue | | Bottom Store | Revenue |
|---|---|---|---|---|---|
| 1 | Store 13 | ~$170K | | Store 1 | ~$35K |
| 2 | Store 17 | — | | Store 4 | — |
| 3 | Store 15 | — | | Store 23 | — |

> Store 13 generates **4.9× more** than Store 1 — same company, same period.

**Revenue by Day of Week (Column Chart)**
- Sunday through Saturday column chart showing weekly revenue variation (~$210K–$265K range)
- Identifies staffing optimization opportunities

**Customer Segment Table**

| Segment | Customers | Revenue | Avg per Customer |
|---|---|---|---|
| **High Value** | 2 | $4,356.74 | $2,178 |
| **Mid Value** | 829 | $673,067.20 | $812 |
| **Low Value** | 8,011 | $1,087,070.93 | $135 |

> 90.6% of the customer base is Low Value. Segment migration = biggest revenue lever.

</details>

---

## 📦 Dashboard 3 — Product Analytics

### Customer Health KPIs

| Metric | Value | Signal |
|---|---|---|
| 👥 Active Customers | **269,711** | Full period |
| 💰 Revenue per Customer | **$199.56** | Avg lifetime value |
| 🔄 Retained Customers | **8,842** | Bought in both years |
| 🆕 New Customers | **3,261** | First-time buyers |
| 💔 Churned Customers | **782** | Did not return ⚠️ |

**Retention Rate: 91.9% · Churn Rate: 8.1%**

<details>
<summary><b>Visuals in this dashboard</b></summary>

<br/>

**Top 10 Products by Revenue**

| Rank | Product | Revenue |
|---|---|---|
| 1 | Hermanos Green Pepper | ~$2,550 |
| 2 | Hilltop Mint Mouthwash | — |
| 3 | Carlton Head Cheese | — |
| 4 | Great Pumpernickel Bread | — |
| 5 | Fabulous Strawberry Drink | — |

Revenue range is tight ($2,200–$2,550) — healthy SKU distribution, no over-reliance.

**Top 10 Products by Profit Margin**

| Rank | Product | Margin |
|---|---|---|
| 1 | Landslide Sesame Oil | **70.8%** |
| 2 | Sunset Scented Tissue | ~70.5% |
| 3 | Skinner Cream Soda | ~70.3% |
| 4 | High Quality Glass Cleaner | ~70.1% |
| 5 | Club Chocolate Milk | ~70.0% |

Products appearing in **both** top-10 lists (revenue + margin) are star performers requiring investment protection.

**Brand Revenue vs Profit Margin (Combo Chart)**
- Blue bars = brand revenue | Orange line = margin % (right axis)
- Brands: Best Choice · Ebony · Fast · Fort West · Hermanos · High Top · Horatio · Nationeel · Tell Tale · Tri-State
- Hermanos leads revenue at ~$55K; margin line oscillates 56.5%–61.5%

</details>

---

## 💡 Key Findings

<table>
<tr>
<td width="48px" align="center"><b>01</b></td>
<td><b>Exceptional Margins</b><br/>Total revenue of $1.76M at a 59.67% profit margin — roughly 2× the typical retail benchmark of 25–35%.</td>
</tr>
<tr>
<td align="center"><b>02</b></td>
<td><b>Explosive YoY Growth</b><br/>1998 revenue ($1.19M) was <b>112% higher</b> than 1997 ($565K), driven by consistent monthly growth — not seasonal spikes.</td>
</tr>
<tr>
<td align="center"><b>03</b></td>
<td><b>Regional Concentration Risk</b><br/>North West generates $870K — <b>3.5× more</b> than Central West. Top 2 regions account for 52% of all revenue.</td>
</tr>
<tr>
<td align="center"><b>04</b></td>
<td><b>Store Performance Gap</b><br/>Store 13 generates <b>4.9× more revenue</b> than Store 1 ($170K vs $35K) within the same organization — suggesting significant operational variance.</td>
</tr>
<tr>
<td align="center"><b>05</b></td>
<td><b>Recoverable Churn Revenue</b><br/>782 churned customers × $199.56 avg value = <b>$156K in recoverable annual revenue</b> from a targeted win-back campaign.</td>
</tr>
</table>

---

## 🎯 Strategic Recommendations

| Priority | Recommendation | Owner | Timeline | Expected Impact |
|---|---|---|---|---|
| 🔴 HIGH | Audit bottom 10 stores — operational review to close the 4.9× gap with Store 13 | Ops Team | 30 days | +$200K potential |
| 🔴 HIGH | Win-back 782 churned customers via targeted re-engagement campaign | Marketing | 21 days | $156K recovery |
| 🔴 HIGH | Accelerate North West investment — already leads at $870K, highest ROI region | Sales VP | Immediate | +15% region target |
| 🟡 MED | Reduce return rate from 2.63% → 2% target — identify top-returned products | Quality Team | 60 days | ~$46K saved annually |
| 🟡 MED | Convert 200 Mid Value customers to High Value via upsell program ($135 → $2,178 avg) | CRM Team | 90 days | +$400K LTV potential |

> **Combined estimated impact: $800K – $1.1M** if all 5 recommendations are fully implemented.

---



---

## 🚀 How to Use

**1. Open the Excel Workbook**
```
File → Enable Editing → Enable Content (required for Power Pivot and DAX)
```

**2. Refresh Data**
```
Data tab → Refresh All → Power Query refreshes all 6 source tables
```

**3. Interact with Dashboards**
```
Use Year, Region, and Store slicers to filter all charts simultaneously.
Each dashboard is self-contained with its own slicer set.
```

**4. Reproduce a Metric**
```
All KPI values are DAX measures. Open Power Pivot → Measures
to inspect or modify any calculation.
```

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Lato&style=italic&size=16&pause=1000&color=6699AA&center=true&vCenter=true&width=700&lines=Data+without+action+is+just+numbers.+These+insights+demand+decisions." alt="Tagline" />

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-MohammedAhmed--01-0A1628?style=for-the-badge&logo=github&logoColor=white)](https://github.com/MohammedAhmed-01)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-mohammed--01--salah-2E75B6?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/mohammed-01-salah)


</div>
