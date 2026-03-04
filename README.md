# Real Estate Sales & Price per m² Dashboard — Python (Jupyter) + Power BI/Visualization

This project focuses on cleaning and analyzing real estate sales data and building visuals to understand 
**pricing patterns** and **price per m²** across different segments such as bedroom count, area type, and location.

---

## Project Goals
- Prepare a clean, analysis-ready dataset using **Python (JupyterLab)**
- Calculate and analyze **Price per m²**
- Explore pricing differences by **Bedrooms**, **Area Type**, and **Location**
- Build clear visuals/dashboards to highlight key insights and trends

---

## Dataset Overview
Key columns used in the analysis:
- `area_type`, `location`, `society`
- `Bedroom`, `bath`, `balcony`
- `Sahe` (Area), `price_azn`
- (Derived) `price_per_m2`

---

## Data Cleaning (JupyterLab / Python)
All cleaning steps were performed in **JupyterLab**:
- Filled **missing (null)** values using appropriate strategies (mean/mode/business logic)
- Corrected **invalid / incorrect** entries (e.g., inconsistent text values like `UNKNOWN`, wrong data types)
- Standardized **column formats** (numeric, categorical, text normalization)
- Removed **duplicates**
- Detected and removed **outliers** (to reduce distortion in price analysis)

---

## Feature Engineering
- Created `price_per_m2` to normalize price by area:
  - `price_per_m2 = price_azn / Sahe`

---

## Visualizations / Dashboard
Visual analysis includes:
- KPI cards (Total revenue, Homes sold, Avg price per m²)
- Avg price per m² by **Bedrooms**
- Sales share by **Area Type**
- Top locations by average price per m²
- Homes sold by bedroom distribution
- Bedroom vs Bathroom cross-tab (heatmap / matrix style)

---

## Key Insights (Example)
- Price per m² varies significantly by **bedroom count** and **area type**
- Certain locations consistently appear in the **top price-per-m²** list
- Outliers had a noticeable impact on average prices before cleaning

