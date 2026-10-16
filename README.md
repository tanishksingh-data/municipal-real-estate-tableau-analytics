# Municipal Real Estate Insights & Valuation Dashboard (2011–2022)

An end-to-end interactive Tableau analytics project designed for municipal planning boards, tax assessors, and zoning committees to evaluate historical property sales trends, monitor assessment-to-market ratio health, and guide regional housing policy.

---

## 📌 Project Overview
* **Domain:** Municipal Real Estate & Urban Planning[cite: 13]
* **Dataset Scope:** 526,000+ real estate transaction records spanning 2011–2022 across multiple municipalities[cite: 1, 13]
* **Primary Tools:** Tableau Desktop / Tableau Public, Data Modeling, Geospatial Geocoding[cite: 13, 14]
* **Live Interactive Link:** [View on Tableau Public](YOUR_TABLEAU_PUBLIC_PROFILE_URL_HERE)

---

## 🎯 Key Objectives
1. **Audit Data Quality:** Flag invalid sales, isolate zero-dollar transactions, handle data anomalies, and rectify sales ratio drift[cite: 1, 13, 14].
2. **Track Market Trajectory:** Identify seasonal spikes and macroeconomic trends across residential, commercial, and vacant land sectors[cite: 13, 14].
3. **Analyze Assessment Equity:** Measure divergences between government Assessed Values and actual Market Sale Prices (`Sales Ratio = Assessed Value / Sale Amount`)[cite: 1, 13, 14].
4. **Interactive Exploration:** Provide dynamic dashboard filters, metric switching parameters, and drill-down capabilities for decision-makers[cite: 13, 14].

---

## 🛠️ Data Preparation & Feature Engineering
* **Derived Metrics & Calculations:**
  * `Sale Category`: Dynamic pricing bands (`Low`: < $250k | `Medium`: $250k–$750k | `High`: > $750k).
  * `Zero/Invalid Sale Flag`: Isolates zero-dollar and non-arm's length transfers to preserve aggregate integrity[cite: 1].
  * `Calculated Sales Ratio`: Independent floating-point precision verification against source ratios (`[Assessed Value] / [Sale Amount]`)[cite: 1].
* **Dynamic Metric Switching:** Integrated parameter control enabling one-click dashboard toggling between **Sale Amount** and **Assessed Value**[cite: 14].

---

## 📊 Visualizations & Dashboard Architecture
* **Geographic Sales Map:** Bubble density and color gradient tracking municipal transaction volume and average sales ratios[cite: 7, 14].
* **Dynamic Municipal Ranking:** Descending bar chart ranking top municipal sales hubs (e.g., Hot Springs, Asheville)[cite: 4, 14].
* **Time-Series Analysis:** Monthly and annual sales trends highlighting the 2021 market surge and category shifts[cite: 5, 9, 14].
* **Asset Class Breakdown:** Treemap and Pie charts detailing market distribution (Single-Family ~90%+)[cite: 6, 14].
* **Interactive Actions:**
  * **Filter Action:** Click any town/bubble to re-aggregate all metrics across the dashboard[cite: 14].
  * **Highlight Action:** Hover over property sectors to track representation across charts[cite: 14].
  * **Dynamic URL Action:** Hyperlink in tooltips directly routing to Wikipedia/municipal pages for selected towns[cite: 14].

---

## 💡 Key Strategic Findings
1. **The 2021 Market Surge:** Transaction volume and valuations peaked in late 2021 before entering a correction phase in 2022[cite: 5, 9].
2. **Sales Ratio Drift:** Several high-velocity municipalities exhibit sales ratios drifting well below 0.50, demonstrating that government assessments have lagged behind rapid market appreciation[cite: 1, 13].
3. **Single-Family Concentration:** Over 90% of regional market volume is concentrated in single-family residential properties, signaling limited multi-family inventory[cite: 6, 13].

---

## 📁 Repository Contents
* `Municipal_Real_Estate_Analysis.twbx` — Packaged Tableau workbook containing all worksheets, dashboards, and stories[cite: 14].
* `data/` — Dataset schema and dictionary[cite: 13, 14].

---
