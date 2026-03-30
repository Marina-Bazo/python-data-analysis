# Project 1 — COVID-19 Global Data Analysis

**ReDI School of Digital Integration — AI Certificate Program 2026**
Week 02 | Python & Pandas

---

## Problem

How did COVID-19 affect mortality rates across different countries and years?
This project explores real-world epidemiological data to identify trends in confirmed cases and deaths globally and for Brazil specifically.

---

## Dataset

- **Source:** Google COVID-19 Open Data
- **Link:** https://storage.googleapis.com/covid19-open-data/v3/epidemiology.csv
- **Coverage:** Global, multiple countries, 2020-2022
- **Key columns:** `location_key`, `date`, `new_confirmed`, `new_deceased`, `new_recovered`, `new_tested`

> Dataset not included due to file size. Download directly from the source above.

---

## Approach

1. Loaded and inspected a large real-world dataset using Pandas
2. Filtered data by country (Denmark, India, Brazil)
3. Handled missing values and converted date columns
4. Calculated mortality rate: `new_deceased / new_confirmed`
5. Grouped data by year and calculated yearly averages
6. Visualised trends using Matplotlib

---

## Key Concepts Applied

- `pandas` — DataFrame inspection, filtering, groupby, column creation
- `matplotlib` — Line chart visualisation
- Statistical analysis — mortality rate calculation, yearly averages
- Data cleaning — handling zeros, datetime conversion
- Best practices — `.loc[]` for safe row modification

---

## Files

| File | Description |
|------|-------------|
| `Spring2025AI_Week02_IntroToPython_handsOn.ipynb` | Class exercise: global COVID-19 exploration and mortality analysis |
| `brazil_pratice.ipynb` | Individual assignment: Brazil-specific mortality rate analysis |

---

## Key Insights

- Global mortality rate was highest in 2020 and declined over the following years
- Brazil showed a distinct mortality pattern compared to the global average
- The mean was significantly higher than the median, indicating a skewed distribution driven by heavily affected countries
