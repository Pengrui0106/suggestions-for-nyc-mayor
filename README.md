# NYC Government Liability & Claim Settlement Analysis 📌

## Project Overview
This project provides a data-driven analysis of New York City’s government liability claims using data from the NYC Open Data portal. The primary goal is to identify patterns in claim frequency and severity to suggest cost-saving reforms. By reducing fiscal waste in legal payouts, the city could potentially reallocate funds toward initiatives such as free public transportation.

---

## 🔍 Key Business Questions
- **Geography:** Which boroughs generate the most claims and why?  
- **Departmental Impact:** Which agencies (e.g., NYPD, Health + Hospitals) are responsible for the highest payouts?  
- **Claim Characteristics:** What are the most common claim types, and which ones represent "long-tail" risks?  
- **Efficiency:** How do report lags and settlement durations affect the final payout amounts?  

---

## 🛠️ Tech Stack
- **Data Processing:** SQL (Data cleaning, standardization, and feature engineering)  
- **Visualization:** Tableau (Trend analysis, risk quadrants, and geospatial mapping)  
- **Data Source:** NYC Open Data - Office of the Comptroller  

---

## 🧮 Data Engineering & Cleaning
The raw dataset was processed using a series of SQL transformations to ensure consistency and extract meaningful metrics:

- **Borough Standardization:** Grouped variations of borough names into five clean categories.  
- **Date Metrics:** Calculated `report_lag_days` (incident to filing) and `settlement_days` (filing to closing).  
- **Agency & Type Simplification:** Categorized hundreds of sub-agencies and claim descriptions into high-level groups like *Law Enforcement*, *Vehicle Accident*, and *Medical Malpractice*.  
- **PI Classification:** Extracted "Personal Injury" (PI) indicators to analyze high-severity payouts.  

---

## 📊 Key Insights

### The Cost of Liability
- **Total Payouts:** $4,800.77M ($4.8B) in settlements.  
- **Top Agency:** NYPD with $1,872.01M in claim payouts.  
- **Borough Leaders:** Brooklyn has the highest total payout ($1,499.39M), while the Bronx has the highest case count due to correction facilities on Rikers Island.  

### Risk Profiles
- **Medical Malpractice:** Kings County Hospital is a significant driver of Brooklyn's high average payouts.  
- **Civil Rights:** "Long-tail risks," some cases date back to police misconduct in the 1980s and 90s; high frequency and high severity.  
- **Personal**
