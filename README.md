# 🛒 Maven Market Retail Analytics Dashboard — Power BI Project  
### **By: Mohammad Kaif Firoz**

An end-to-end Power BI analytics solution built using the **Maven Market retail dataset**.  
This project transforms raw retail transactions into a complete business intelligence dashboard for executives, regional managers, and product teams.

---

## 📂 Project Files Included

| File Name | Description |
|----------|-------------|
| **Maven Market Project KAIF FIROZ.pbix** | Power BI dashboard (full report) |
| **FULL INTERVIEW for Maven Market.docx** | Complete interview Q&A for project explanation |
| **MavenMarket_Calendar.csv** | Date table with time intelligence columns |
| **MavenMarket_Customers.csv** | Customer dimension table |
| **MavenMarket_Products.csv** | Product & pricing master data |
| **MavenMarket_Regions.csv** | Region mapping table |
| **MavenMarket_Returns_1997-1998.csv** | Returns fact table |
| **MavenMarket_Stores.csv** | Store master data |
| **MavenMarket_Transactions_1997.csv** | 1997 transaction data |
| **MavenMarket_Transactions_1998.csv** | 1998 transaction data |
| **PART 1 Connecting & Shaping the Data.docx** | Power Query transformation steps |
| **PART 2 Creating the Data Model.docx** | Data modeling documentation |
| **PART 3 Adding DAX Measures.docx** | DAX formulas used in the dashboard |
| **PART 4 Building the Report.docx** | Dashboard layout & visuals explanation |

---

## 📌 1. Business Requirement

The Maven Market leadership team needed a centralized dashboard that provides:

- KPIs for transactions, profit, returns, and revenue vs target  
- Product brand performance across profit, margin, volume, and return rate  
- Store, region, and country-level performance insights  
- Weekly revenue trend analysis  
- Return behavior and its impact on profit  
- A geographic view of customer/store performance  

The dashboard solves visibility gaps and enables **data-driven retail decision-making** across sales, operations, and product teams.

---

## 🎯 2. Analytical Goals

- Identify high-performing brands and weak performers  
- Compare regions (USA, Mexico, Canada) by revenue and profit  
- Track profit margin trends and return rate  
- Analyze transactions across stores & cities  
- Study weekly revenue seasonality  
- Evaluate revenue performance against targets  
- Provide executive-level KPIs with MoM indicators  

---

## 🧹 3. Data Preparation & Modeling

Dataset includes **7 CSV files + 2 years of transactions**.

### ETL Steps Performed:

- Promoted headers & corrected data types  
- Cleaned nulls and standardized text fields  
- Created new columns: `full_name`, `birth_year`, `price_tier`, `full_address`, `area_code`  
- Built a **Calendar table** with:
  - Year, Quarter, Month  
  - Week Number  
  - Weekend Flag  
- Combined 1997 & 1998 data into a single **Transaction_Data** fact table  
- Created a dedicated **_Measure Table** for DAX calculations  
- Built a clean **Star Schema**

### Final Data Model

**Fact Tables:**
- Transaction_Data  
- Return_Data  

**Dimension Tables:**
- Calendar  
- Products  
- Customers  
- Stores  
- Regions  

All relationships: **one-to-many, single-direction filtering (standard star schema)**.

---

## 📊 4. Dashboard Pages & Visuals

### 🏠 Executive Overview Dashboard  
*(Main dashboard screenshot shown at top of repository)*

#### KPIs:
- **Current Month Transactions**  
- **Current Month Profit**  
- **Current Month Returns**  
- With MoM % change & goals  

#### Visuals:
- Brand Performance Matrix (transactions, profit, margin, return rate)  
- Geographic Map of store activity  
- Treemap visual for country → region breakdown  
- Weekly Revenue Trend chart  
- Revenue vs Target Gauge  
- Slicers for country & region selection  

---

## 🛍 Product & Brand Analytics

Shows:

- Top-selling brands  
- High & low profit margin products  
- Products with high return rate  
- Conditional formatting highlights (good vs poor performers)  

---

## 🌎 Region & Store Analytics

Includes:

- Region-level revenue comparison  
- City-level performance (Portland, Chicago, Seattle, etc.)  
- Store-level bubble map  
- Filters for country selection (USA, Mexico, Canada)  

---

## 🔁 Returns Analysis

Analyzes:

- Quantity returned  
- Return rate by brand  
- Profit impact due to returns  
- Return trends across years  

Return rate maintained below **1%**, indicating strong product satisfaction.

---

## 🧠 5. Key Insights

- 🇺🇸 **USA** dominates revenue and total transactions  
- 💰 Profit margin remains consistently high at **~59–60%**  
- 🏙 **Portland exceeded 1,000 transactions in December**  
- 📅 Weekend transactions represent **~28% of traffic**  
- 🔁 Return Rate stays below **1%**, indicating strong product quality  
- 🛍 Top brands: **Hermano, Ebony, Tell Tale**  
- 🔍 Some brands show above-average return rates requiring investigation  

---

## ⚙️ 6. Tools & Techniques Used

- Power BI  
- Power Query  
- Star Schema Modeling  
- 20+ DAX Measures  
- Time Intelligence  
- Map Visuals (Geo-Spatial)  
- Bookmarks & UX Enhancements  
- Performance Optimization  

---
## 🧮 7. Major DAX Measures Created

- **Total Revenue**  
- **Total Cost**  
- **Total Profit**  
- **Profit Margin**  
- **Quantity Returned**  
- **Return Rate**  
- **YTD Revenue**  
- **60-Day Rolling Revenue**  
- **MoM KPIs (Transactions, Profit, Returns)**  
- **All Transactions / All Returns (ignore filters)**  

---

## 📂 8. Folder Structure 

📁 Maven-Market-Retail-Analysis  
│── README.md  
│── FULL INTERVIEW for Maven Market.docx  
│── PART 1 Connecting & Shaping the Data.docx  
│── PART 2 Creating the Data Model.docx  
│── PART 3 Adding DAX Measures.docx  
│── PART 4 Building the Report.docx  
│── Maven Market Project KAIF FIROZ.pbix  
│── MavenMarket_Calendar.csv  
│── MavenMarket_Customers.csv  
│── MavenMarket_Products.csv  
│── MavenMarket_Regions.csv  
│── MavenMarket_Stores.csv  
│── MavenMarket_Returns_1997-1998.csv  
│── MavenMarket_Transactions_1997.csv  
│── MavenMarket_Transactions_1998.csv  
│── Dashboard Screenshot.png  

---

## 📸 9. Dashboard Preview

https://github.com/kaiffirox/Maven-Market-Power-BI-Analytics-Dashboard/blob/main/Meven%20Market%20Dashboard%20Screenshot.png

---

## 👨‍💻 10. Author

**Mohammad Kaif Firoz**  
Data Analyst — SQL | Power BI | Excel | Tableau | Python  

📧 Email: **kaifsidd2003@gmail.com**  
🔗 LinkedIn: **https://www.linkedin.com/in/kaiffiroz/**  

---

⭐ *If you found this project useful, please consider giving the repository a star!* ⭐

