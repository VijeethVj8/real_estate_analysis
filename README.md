# 🏡 U.S. Real Estate Market Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)  
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20|%20Matplotlib%20|%20Seaborn%20|%20NumPy-orange.svg)  
![Status](https://img.shields.io/badge/Status-Completed-green.svg)

---

## 📌 Overview  
This project analyzes a **large Realtor dataset (~2.2M property listings)** to explore housing market patterns across the United States.  
The goal is to uncover **price trends, geographic insights, and volatility** using data cleaning, exploratory analysis, and visualization.  

---

## 🗂️ Dataset  
- **File**: `realtor-data.csv`  
- **Shape**: ~2.2M rows × 12 columns  
- **Key columns**:
  - `price` – Listing price of the property  
  - `bed`, `bath` – Number of bedrooms and bathrooms  
  - `house_size` – Size of the property (sq ft)  
  - `acre_lot` – Lot size in acres  
  - `status` – For Sale, Sold, Ready to Build  
  - `city`, `state`, `zip_code` – Location info  
  - `brokered_by` – Brokerage/agent ID  
  - `prev_sold_date` – Previous sale date  

---

## 🔎 Analysis Workflow  

### 1. Data Cleaning  
- Fixed datatypes (zip codes as strings, dates as datetime)  
- Handled missing values  
- Removed outliers (e.g., price > $10M, 400+ bedrooms)  

### 2. Exploratory Data Analysis (EDA)  
- Summary statistics for numeric & categorical fields  
- Missing value heatmaps and distributions  

### 3. Geographic Insights  
- **State-level medians** (price, beds, baths, size, lot size)  
- **City-level analysis** with $/sqft comparisons  
- Identified undervalued and overvalued markets  

### 4. Time-Series Trends  
- National & state-level **median price trends**  
- **Monthly rolling medians** for seasonality  
- **Year-over-Year (YoY) growth rates**  
- Heatmap of **state × year growth**  
- Volatility analysis (Top/Bottom states by YoY growth)  

### 5. Visualizations  
- Bar charts: top states/cities by median price  
- Dual-axis plots: price vs size vs lot size  
- Line charts: national & state price trends  
- Heatmap: YoY growth by state  
- Volatility lines: most boom/bust states vs U.S. baseline  

---

## ⚙️ Tech Stack  
- **Programming**: Python 3.8+  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Statsmodels  
- **Notebook**: Jupyter Notebook  

---

## 📊 Key Insights  
- **California, New York, Hawaii, and D.C.** are consistently the most expensive markets.  
- **Hawaii** has high prices despite smaller house sizes → premium land market.  
- **Utah & Colorado** show strong growth with relatively affordable $/sqft.  
- National housing market shows **boom–bust cycles** with clear volatility by state.  

---

## 🚀 How to Run  

### 1. Clone the Repository  
```bash
git clone https://github.com/yourusername/realtor-analysis.git
cd realtor-analysis
