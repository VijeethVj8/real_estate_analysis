🏡 U.S. Real Estate Market Analysis
📌 Overview

This project explores U.S. housing market trends using a large Realtor dataset (~2.2M records).
The analysis provides insights into property prices, house sizes, lot sizes, geographic differences, and time-based market trends.

🗂️ Dataset

Source: Realtor housing dataset (realtor-data.csv)

Size: ~2.2M rows × 12 columns

Key fields:

price, bed, bath, house_size, acre_lot

status (For Sale, Sold, Ready to Build)

city, state, zip_code, brokered_by

prev_sold_date

🔎 Analysis Workflow

Data Cleaning

Converted datatypes (e.g., zip → string, dates → datetime)

Handled missing values

Removed outliers (e.g., unrealistic price, size, lot size)

Exploratory Data Analysis (EDA)

Summary stats & missing value report

Distribution of price, size, lot size, beds & baths

Geographic Insights

State-level medians (price, size, lot size)

Top cities by price and $/sqft value

Comparison of city vs state medians

Time-Series Trends

National & state-level median price trends

Monthly rolling averages & seasonality

Year-over-Year (YoY) % growth

Heatmap of YoY growth by state × year

Volatility analysis (Top/Bottom states by growth)

Visualizations

Bar charts: top states & cities by price

Dual-axis charts: price vs size vs lot size

Line charts: price trends & YoY growth

Heatmap: state-level YoY changes

⚙️ Tools & Libraries

Python: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Modeling/Stats: Statsmodels (for additional exploration)

📊 Key Findings

California & New York consistently rank among the most expensive states.

Hawaii shows high prices despite smaller house sizes.

Some inland states (e.g., Utah, Colorado) provide larger homes at lower $/sqft.

National YoY growth highlights boom & bust cycles, with clear volatility in certain states.
