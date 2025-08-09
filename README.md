
# Startup Funding Analysis

## 📌 Overview

This project analyzes **Indian startup funding data** to clean, preprocess, and extract key insights such as top-funded sectors, cities, startups, and investors. It also visualizes funding trends over time using **Matplotlib** and **Seaborn**.

The script performs:

* Data cleaning and preprocessing
* Handling of missing values
* Standardization of text fields
* Analysis of funding trends by year, month, sector, city, startup, investor, and investment type
* Visualization of results

---

## 📂 Dataset

The script expects a dataset in CSV format named `startup_funding.csv` with the following columns:

* `Sr No`
* `Date dd/mm/yyyy`
* `Startup Name`
* `Industry Vertical`
* `SubVertical`
* `City  Location`
* `Investors Name`
* `InvestmentnType`
* `Amount in USD`
* `Remarks` *(optional)*

---

## ⚙️ Requirements

Install the required Python libraries:

```bash
pip install pandas matplotlib seaborn
```

---

## 🚀 How to Run

1. Place `startup_funding.csv` in the `/content/` directory or update the path in `main.py`.
2. Run the script:

```bash
python main.py
```

3. The script will:

   * Display cleaned dataset information
   * Show funding trends and top rankings
   * Generate visualizations for trends and comparisons

---

## 🔍 Key Steps in Analysis

1. **Data Cleaning**

   * Drop `Remarks` column if present
   * Fill missing values with `"Unknown"`
   * Remove commas, plus signs from `Amount in USD`
   * Convert date to proper datetime format
   * Standardize text columns (lowercase, strip spaces)

2. **Feature Engineering**

   * Extract `FundingYear` and `FundingMonth` from dates

3. **Trend Analysis**

   * Yearly and monthly funding trends
   * Sector-wise, city-wise, startup-wise, and investor-wise analysis
   * Investment type analysis

4. **Visualizations**

   * Line plots for funding trends
   * Bar charts for top 10 rankings in different categories

---

## 📊 Example Outputs

* **Yearly Funding Trends** – Total funding and number of deals over the years
* **Top Sectors by Funding**
* **Top Cities by Funding**
* **Top Startups by Funding**
* **Top Investors by Funding & Deals**
* **Top Investment Types by Funding & Deals**

---

## 🖼 Visualizations

Generated plots include:

* Funding trends over time
* Top sectors, cities, startups, and investors
* Popular investment types
---
