# ✅Indian Used Car Sales Analysis

**Author:** Drisya D  
**Date:** February 2026  
**Mentor:** Lakshmi Nayana  

Comprehensive Exploratory Data Analysis (EDA) on 5,975 Indian used cars priced 44K–1.6Cr from India's ₹567Cr used car market. Covers data cleaning, feature engineering (Age, PriceperCC, LuxuryScore, RegionalPremium), and business insights for automotive sales/e-commerce.

## 📊 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Key Results](#key-results)
- [Business Insights](#business-insights)
- [Visualizations](#visualizations)
- [Future Work](#future-work)

## ✅Overview
Analyzes real Indian used car sales data from major cities (Mumbai, Pune, Chennai, Coimbatore).  
Complete pipeline: raw data → cleaning → 19 engineered features → actionable insights.  
Ideal for data analyst portfolios—production-grade EDA with visualizations and pricing strategies

## ✅Dataset
- **Source:** Indian used car sales data from GitHub repo.  
- **Size:** 5,975 rows × 14 columns.  
- **Key Columns:** Name, Manufacturer, Location, Year, KilometersDriven, FuelType, Transmission, OwnerType, Engine_CC, Power, Seats, Mileage_Km/L, Price.  
- **Scope:** Captures market dynamics; prices ₹0.44L–₹160L; avg age 12.6 years.

## ✅Project Structure

├── data/

│   ├── indian-auto.csv          # Raw data

│   ├── cleancarsalesindia.csv   # Cleaned data

│   └── advancedcarsales.csv     # With engineered features

├── notebooks/

│   ├── 01_data_cleaning.ipynb   # Cleaning & outliers

│   └── 02_eda.ipynb             # Full EDA & visuals 

├── requirements.txt

└── README.md

## ✅Key Results
**Data Quality:** Removed Seats=0, imputed Mileage median (18 km/L), capped KM outliers (max 131K km).

**Features Engineered (19 total):** Age (avg 12.6 yrs), PriceperCC (₹5.2K), KMperYear, LuxuryScore, RegionalPremium, Q12026Value, PowertoWeight, etc.

**Stats**: Avg price ₹9.5L (median ₹5.65L), Maruti 20% market share, Diesel +15% premium.

Metric	Value
Rows after cleaning	5,974
Avg Age	12.6 years
Top Brand	Maruti (1,197 listings)
Top Location Price	Coimbatore (₹10.67L)
Strongest Price Corr	Power (r=0.85)

## ✅Business Insights

**Pricing:** Mumbai/Coimbatore +15–22% premium vs Chennai bargains (₹6.5L). Arbitrage: Buy low in Chennai, sell high in Mumbai.

**Depreciation:** 40–60% value loss in first 5 years; sweet spot 4–6yr cars.

**Segments:** Diesel manuals (volume), luxury autos (margins); target 1st-owner low-KM.

**Strategy:** 60% diesel inventory, regional dynamic pricing → 2x revenue in 6 months.[file:36]

## ✅Visualizations

Key plots from EDA 


**Price vs Age:** Exponential decay; newer cars hold 70% value.


**Correlation Heatmap:** Power/EngineCC strongest price drivers.


**Price by Fuel & Transmission:** Diesel + Auto premiums clear.

## ✅Future Work
ML price prediction (XGBoost, 85% accuracy target).

Interactive dashboard (Plotly Dash/Power BI).

Choropleth maps for regional pricing.

Time-series forecasting (Q1 2026 values).

