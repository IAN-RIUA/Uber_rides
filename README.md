# Uber Rides Project
# 🚖 NCR Uber Ride Bookings — End-to-End Analytics & ML

![Python](https://img.shields.io/badge/Python-3.14-blue) ![License](https://img.shields.io/badge/license-MIT-green) ![Status](https://img.shields.io/badge/status-complete-brightgreen)

An end-to-end data analytics and machine learning project analysing **150,000 Uber ride bookings** across the NCR region (Jan–Dec 2024). The project covers data cleaning, exploratory analysis, demand forecasting, and cancellation prediction — with an interactive HTML dashboard.

---

## 📁 Project Structure

```
Uber_rides/
├── index.ipynb               # Main analysis notebook
├── uber_ncr_dashboard.html   # Interactive analytics dashboard
├── ncr_ride_bookings.csv     # Dataset (150,000 rides)
├── README.md
└── *.png                     # Chart exports from notebook
```

---

## 📊 Project Overview

| Section | Description |
|---|---|
| Data Cleaning | Datetime parsing, null handling, feature engineering |
| EDA | Demand patterns, revenue trends, payment methods |
| Business Insights | Cancellation analysis, VTAT wait times, ratings |
| Demand Forecasting | Gradient Boosting Regressor — R² = 0.83 |
| Cancellation Prediction | Random Forest Classifier — ROC-AUC = 0.64 |

---

## 💡 Key Findings

- **32% problem rate** — 57,000 rides were cancelled, incomplete, or unmatched
- **Driver cancellations dominate** — 18% of all rides vs 7% by customers (2.6× higher)
- **Evening peak (18:00–20:00)** is the highest demand window across all days
- **VTAT is the #1 cancellation predictor** — longer wait times drive most problems
- **Annual revenue ≈ ₹51.8M** with consistent month-to-month performance

---

## 🤖 ML Models

**Demand Forecasting (Gradient Boosting Regressor)**
- Features: hour, weekday, month, peak flags
- R² Score: `0.83` | MAE: `3.15 rides/hour`

**Cancellation Prediction (Random Forest Classifier)**
- Features: hour, vehicle type, pickup location, VTAT
- ROC-AUC: `0.64`

---

## 🛠️ Tech Stack

`Python` `pandas` `NumPy` `scikit-learn` `Matplotlib` `Seaborn` `Chart.js`

---

## 🚀 Getting Started

```bash
git clone https://github.com/IAN-RIUA/Uber_rides.git
cd Uber_rides
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook index.ipynb
```

To view the dashboard, open `uber_ncr_dashboard.html` in any browser.

---

## 👤 Author

**Ian** — Data Systems Analyst | [GitHub](https://github.com/IAN-RIUA)
