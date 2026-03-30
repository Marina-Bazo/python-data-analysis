# Project 3 — World Tourism Statistics Analysis

**ReDI School of Digital Integration — AI Certificate Program 2026**
Week 03 | Introduction to Statistics

---

## Problem

How has global tourism changed over 25 years?
Which countries receive the most tourists?
What was the impact of COVID-19 on global tourism arrivals?

This project uses statistical analysis and visualisation to answer these questions using real-world data.

---

## Dataset

- **Source:** Kaggle — Tourism and Economic Impact
- **Link:** https://www.kaggle.com/datasets/bushraqurban/tourism-and-economic-impact
- **Coverage:** 266 countries, 1999-2023
- **Key columns:** `country`, `year`, `tourism_arrivals`, `tourism_receipts`

> Dataset not included due to file size. Download directly from Kaggle.

---

## Approach

1. Loaded and inspected the dataset
2. Calculated measures of central tendency (mean, median, mode)
3. Calculated measures of spread (min, max, range, variance, std deviation, IQR)
4. Created a decade column for grouped analysis
5. Developed four visualisations to explore trends
6. Filtered top 10 countries by total arrivals

---

## Key Concepts Applied

- `pandas` — DataFrame loading, groupby, filtering, column creation
- `matplotlib` — Histogram, box plot, line chart, bar chart
- Statistical analysis — central tendency, spread, distribution shape
- Data exploration — identifying patterns and outliers

---

## Visualisations

1. **Histogram** — Distribution of tourism arrivals across all countries
2. **Box Plot** — Tourism receipts by decade
3. **Line Chart** — Global tourism arrivals over time (1999-2023)
4. **Bar Chart** — Top 10 most visited countries (1999-2023)

---

## Key Insights

- The mean (62.6M arrivals) is much higher than the median (2.5M), showing a right-skewed distribution — a few large countries dominate global tourism
- Tourism grew consistently every year from 1999 to 2019
- COVID-19 caused the biggest drop in global tourism in 25 years (2020)
- France leads global tourism due to its culture and infrastructure
- Recovery after COVID has been gradual

---

## Files

| File | Description |
|------|-------------|
| `tourism_analysis.ipynb` | Individual assignment: statistical analysis and visualisation of global tourism data |
