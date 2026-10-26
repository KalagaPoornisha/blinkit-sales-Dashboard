# Blinkit Sales Analytics Power BI Dashboard

## 📌 About the Project
This project presents an end-to-end data analysis and interactive Power BI dashboard for **Blinkit** (India's Last Minute App). Quick commerce demands rapid operational clarity—this dashboard delivers actionable insights into grocery delivery performance, consumer buying behavior, store footprint efficiency, and product sales distributions across various retail formats and geographic tiers.

---

## 🎯 Project Objective
The primary goal of this project is to analyze Blinkit's retail sales data to evaluate store performance, track key operational metrics, and uncover sales trends. Specific objectives include:
* Analyzing key business KPIs (Total Revenue, Average Order Value, Total Items Sold, and Customer Satisfaction Ratings).
* Identifying regional preferences regarding product fat content, store size, and location tiers.
* Evaluating performance across different outlet types (Grocery Stores vs. Supermarkets).
* Providing dynamic filtering capabilities for stakeholders to perform granular ad-hoc analysis.

---

## 📅 Dataset
The analysis is based on the Blinkit Sales Dataset containing detailed transactional and operational attributes:
* **Item Metrics:** Item Identifier, Weight, Fat Content, Visibility, Type, MRP.
* **Outlet Metrics:** Outlet Identifier, Establishment Year, Size (Small, Medium, High), Location Type (Tier 1, Tier 2, Tier 3), Outlet Type (Grocery Store, Supermarket Type 1/2/3).
* **Sales & Metrics:** Total Sales, Item Rating.

---

## 🛠️ Tools & Technologies
* **Power BI Desktop:** Core tool for data modeling, visualization, dynamic slicers, and dashboard design.
* **Power Query Editor:** Used for ETL (Extract, Transform, Load) processes, column profiling, and data hygiene.
* **DAX (Data Analysis Expressions):** Utilized to construct calculated columns, explicit measures, dynamic aggregations, and comparative time-series KPI logic.
* **Microsoft Excel / CSV:** Source dataset format.

---

## 🧹 Data Cleaning & Transformation
Data preprocessing was performed using **Power Query** to ensure data integrity:
1. **Standardization:** Normalized variations in categorical values (e.g., standardizing `LF`, `low fat`, and `Low Fat` into a single `Low Fat` category).
2. **Missing Value Handling:** Imputed missing values for `Item Weight` using mean values based on item categories and handled missing `Outlet Size` values by cross-referencing `Outlet Type`.
3. **Data Type Correction:** Enforced explicit data types across all columns (Currency, Integers, Decimals, Text).
4. **Custom Columns:** Created derived columns for age of outlets (`Outlet Age = YEAR(TODAY()) - Outlet_Establishment_Year`).

---

## 🧮 DAX & Measures
Custom DAX formulas were created for dynamic key metrics:

* **Total Sales Revenue:**
  ```dax
  Total Sales = SUM('Blinkit Sales'[Total_Sales])
  ```
* **Average Sales Value:**
  ```dax
  Avg Sales = AVERAGE('Blinkit Sales'[Total_Sales])
  ```
* **Total Items Sold:**
  ```dax
  Total Items = COUNTROWS('Blinkit Sales')
  ```
* **Average Rating:**
  ```dax
  Avg Rating = AVERAGE('Blinkit Sales'[Rating])
  ```

---

## 📊 Dashboard Features

### 🎛️ Interactive Filters (Slicers)
* **Outlet Location Type:** Tier 1, Tier 2, Tier 3.
* **Outlet Size:** Small, Medium, High.
* **Item Type:** Fruits & Vegetables, Snack Foods, Dairy, Household, etc.
* **Fat Content:** Low Fat vs. Regular.

### ❓ Key Business Questions Answered
1. Which outlet location tier generates the highest revenue?
2. How does item fat content preference vary across store tiers?
3. What product categories contribute most to total sales volume?
4. How does store physical size correlate with revenue performance?
5. How do Supermarkets compare against local Grocery Stores in total sales and item turnover?

### 💡 Key Insights
* **Total Sales Revenue:** Reached **₹1.20M** across 8,523 total items sold with an average customer rating of **3.92 / 5**.
* **Top Selling Categories:** *Fruits & Vegetables* and *Snack Foods* lead overall sales, closely followed by *Household* goods.
* **Location Tier Distribution:** **Tier 3** locations generate the highest proportion of total sales (₹472K), demonstrating high demand in developing markets.
* **Outlet Size Impact:** **Medium-sized** outlets dominate revenue generation (₹508K), outperforming both High (₹249K) and Small (₹445K) stores.
* **Fat Content Preference:** Low Fat items account for the majority (~65%) of total sales volume across all location tiers.

---

## 📁 Project Structure
```text
Blinkit_Sales_PowerBi_Dashboard/
│
├── data/
│   └── Blinkit_Sales_Data.csv          # Raw Dataset
│
├── visuals/
│   └── dashboard_preview.png           # Visual screenshot of the dashboard
│
├── Blinkit_Sales_Dashboard.pbix         # Main Power BI File
├── README.md                            # Project documentation
└── LICENSE                              # Project License
```

---

## 🚀 How to Use
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Blinkit_Sales_PowerBi_Dashboard.git
   ```
2. **Open the Dashboard:**
   * Download and install **Microsoft Power BI Desktop**.
   * Double-click `Blinkit_Sales_Dashboard.pbix` to launch the report.
3. **Explore Interactively:**
   * Click on any visual element or use the filter pane to slice data across tiers, sizes, and item categories in real time.

---

## 💡 Skills Demonstrated
* Data Cleaning, Transformation, and ETL pipeline execution in Power Query.
* Writing optimized DAX measures and calculated columns.
* Data modeling and building relationship topologies between tables.
* UI/UX layout design, color contrast balance, and dynamic dashboard creation.
* Translating complex datasets into actionable executive summaries.

---

## 🔮 Future Improvements
* **Automated Data Refresh:** Integrate Power BI Service scheduled refresh with cloud storage (Azure Blob / SharePoint).
* **Predictive Analytics:** Implement Forecasting models using Power BI built-in AI visual extensions for sales predictions.
* **Customer Basket Analysis:** Conduct Market Basket Analysis to understand cross-selling item pairs.

---

## 🏁 Conclusion
This dashboard offers Blinkit an interactive tool to monitor sales performance, optimize inventory across store sizes, and tailor localized product offerings based on customer preferences in Tier 1, 2, and 3 cities.

---
*Developed by **AnalyticalCK** | Powered by **Power BI***