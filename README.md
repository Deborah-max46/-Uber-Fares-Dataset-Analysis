# 🚖 Uber Fare Behavior Analysis

This project analyzes Uber ride fare patterns using a cleaned and feature-enhanced dataset enriched with simulated weather data. It combines Python-based data processing with Power BI dashboarding to uncover deep insights into ride behavior, temporal trends, and pricing anomalies.

---

## 📘 Project Overview

Urban mobility platforms like Uber generate massive volumes of transactional data. However, fare variability is often misunderstood due to hidden behavioral and contextual factors. This project explores these questions:

- How do time-based patterns influence fare amounts?
- What non-obvious trends emerge in off-peak hours?
- Can simulated weather data help reveal pricing behavior?
- How can data visualization guide decision-making for pricing and operations?

---

## 🧪 Methodology

### 🗃️ Data Sources
- Raw ride data (`uber.csv`) with timestamps and fare amounts.
- Enhanced dataset (`enhanced_uber.csv`) with extracted time features.
- Simulated weather data (`weather`, `temperature_C`) generated with Python.

### 🛠️ Tools & Techniques
- **Python** (Pandas, Seaborn): Data cleaning, EDA, and feature engineering.
- **Power BI Desktop**: Dashboard creation with filters, drilldowns, and custom visuals.

### ✨ Engineered Features
- `hour`, `day`, `month`, `weekday`, `day_name`
- `time_category`: Peak / Off-Peak label
- `weather`: Simulated (Sunny, Rainy, Cloudy, etc.)
- `temperature_C`: Synthetic realistic values

---

## 📊 Analysis Highlights

### 📌 Fare Distribution
- Fares are right-skewed, with most under $20 and occasional spikes over $60.
- Tuesdays showed the most consistent pricing; Fridays had extreme outliers.

### ⏱️ Temporal Patterns
- **Peak demand** occurs 7–9 AM and 5–7 PM.
- **Unexpected fare spikes** between 1–3 AM hint at event-driven demand.

### 🌦️ Weather Impact
- Rainy and stormy conditions showed **15–22% fare increases**.
- Fares were more volatile in poor weather.

### 🗓️ Seasonal Behavior
- Fares followed a **U-shaped trend**, peaking in July and December.

---

## 📈 Key Results

- Late-night Sunday and early-Friday evening slots show stress points in pricing and demand.
- Slight correlation between **colder temperatures** and **higher fares**, suggesting weather sensitivity.
- Weekday × Hour matrix revealed clear patterns useful for driver allocation.

---

## 🧾 Dashboard Features (Power BI)

- Histograms and box plots for fare distribution
- Line charts for fare and ride trends over time
- Interactive filters: `weather`, `day_name`, `time_category`
- Drill-downs by `month → day` for time-series depth
- Optional geographic visualization (if coordinates are available)

---

## ✅ Recommendations

- **Dynamic pricing models** should factor in weather forecasts, especially for stormy and rainy days.
- Implement **event-aware micro-surge pricing** for unusual late-night demand spikes.
- Use temporal matrices to guide **predictive driver positioning**.
- Launch **midweek promotions** to increase usage on low-demand days.

---

## 📂 Files in This Repo

| File | Description |
|------|-------------|
| `uber.csv` | Original dataset |
| `enhanced_uber.csv` | Cleaned dataset with engineered features |
| `uber_with_weather.csv` | Final dataset with simulated weather |
| `uber_fare_analysis.pbix` | Power BI dashboard file |
| `main.py` | Python script for cleaning, feature engineering, and weather simulation |

---

## 📌 Credits

Developed by **Uwase Ketsia Deborah**  
Tools used: Python, Pandas, Seaborn, Power BI

---

## 📄 License

This project is for academic and demonstration purposes only. Simulated data (weather, temperature) was generated for illustrative analysis.

