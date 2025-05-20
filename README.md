# New_york_city_fatalities
# 🚗 NYC Traffic Fatalities Analysis

This project analyzes traffic-related fatalities in New York City using publicly available crash data. The goal is to uncover patterns across time, geography, and contributing factors that help understand where and when fatal crashes occur—and what might influence them.

---

## 📦 Dataset

- **Source**: NYC Open Data – [Motor Vehicle Collisions - Crashes](https://data.cityofnewyork.us/Transportation/Motor-Vehicle-Collisions-Crashes/h9gi-nx95)
- **File**: `Motor_Vehicle_Collisions_-_Crashes_20250220.csv`
- **Size**: 1M+ records
- **Features Used**: Crash date, time, borough, latitude, longitude, number of persons killed, street names, vehicle type, contributing factors.

---

## 🔍 Key Objectives

- Understand **when** fatal crashes occur (time of day, day of week, month, year).
- Identify **where** crashes are most deadly (borough, ZIP code, streets).
- Explore whether certain **conditions** (like night-time or borough) increase fatal crash likelihood.
- Build statistical models to test hypotheses and predict fatal crash outcomes.

---

## 📊 Analysis & Visualizations

### ✅ Data Cleaning & Transformation
- Standardized column names.
- Parsed datetime fields (`CRASH_DATE`, `CRASH_TIME`) and extracted `HOUR`, `DAY_OF_WEEK`, `YEAR`.
- Created new features: `IS_FATAL`, `TOTAL_FATALITIES`.

### 📈 Visualizations
- **Heatmap** of fatalities by hour of day and day of week.
- **Bar charts**:
  - Fatalities by borough
  - Top 10 ZIP codes and streets with most fatalities
- **Line plots**:
  - Hourly trends
  - Yearly and monthly time series
- **Pie chart**:
  - Fatalities by road user type (pedestrian, cyclist, motorist)
- **Folium maps**:
  - Cluster map of fatal crash locations
  - Weighted geographic heatmap of fatality density

### 📐 Statistical Analysis
- **T-Test**: Compared night-time vs day-time crashes.
- **Chi-Square Test**: Checked association between borough and fatality likelihood.
- **OLS Regression**:
  - Modeled fatal crashes using hour and borough with interaction terms.

---

## 💡 Key Insights

- Fatal crashes are more frequent late at night and early in the morning.
- Brooklyn and the Bronx report the highest fatality numbers.
- Weekends (especially Saturday) show increased fatal crash density.
- Certain streets and ZIP codes consistently appear as high-risk zones.

---

## 🛠️ Tools & Libraries

- Python (Pandas, NumPy)
- Matplotlib, Seaborn (for charts)
- Folium (for interactive maps)
- SciPy & StatsModels (for statistical testing)

---

## 📁 Files Included

