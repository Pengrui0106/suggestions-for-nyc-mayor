NYC Government Liability & Claim Settlement Analysis
📌 Project Overview
This project provides a data-driven analysis of New York City’s government liability claims using data from the NYC Open Data portal. The primary goal is to identify patterns in claim frequency and severity to suggest cost-saving reforms. By reducing fiscal waste in legal payouts, the city could potentially reallocate funds toward initiatives such as free public transportation.


🔍 Key Business Questions
Geography: Which boroughs generate the most claims and why? 
Departmental Impact: Which agencies (e.g., NYPD, Health + Hospitals) are responsible for the highest payouts? 
Claim Characteristics: What are the most common claim types, and which ones represent "long-tail" risks? 
Efficiency: How do report lags and settlement durations affect the final payout amounts? 

🛠️ Tech Stack
Data Processing: SQL (Data cleaning, standardization, and feature engineering) 
Visualization: Tableau (Trend analysis, risk quadrants, and geospatial mapping) 
Data Source: NYC Open Data - Office of the Comptroller 

🧮 Data Engineering & Cleaning
The raw dataset was processed using a series of SQL transformations to ensure consistency and extract meaningful metrics:
Borough Standardization: Grouped variations of borough names into five clean categories .
Date Metrics: Calculated report_lag_days (incident to filing) and settlement_days (filing to closing) .
Agency & Type Simplification: Categorized hundreds of sub-agencies and claim descriptions into high-level groups like "Law Enforcement," "Vehicle Accident," and "Medical Malpractice".
PI Classification: Extracted "Personal Injury" (PI) indicators to analyze high-severity payouts.

📊 Key Insights
1. The Cost of Liability

Total Payouts: The analyzed claims account for a total of $4,800.77M ($4.8 Billion) in settlements.
Top Agency: The NYPD is the #1 department for claim payouts, totaling $1,872.01M.
Borough Leaders: Brooklyn has the highest total payout amount at $1,499.39M , while the Bronx has the highest case count due to correction facilities on Rikers Island.

2. Risk Profiles
Medical Malpractice: Kings County Hospital is a significant driver of Brooklyn's high average payouts.
Civil Rights: These represent "long-tail risks," with some cases dating back to police misconduct in the 1980s and 90s. They are characterized by high frequency and high severity.
Personal Injury (PI): PI cases consistently lead to higher payouts. Unlike other claims, their cost is driven by the severity of the injury rather than the duration of the legal process.

3. Efficiency Gaps
Claims involving the Health and Education departments are particularly slow, often taking 3.5 years to settle.

💡 Policy Recommendations for the Mayor

Driver Training: Enhance training for NYC government vehicle drivers, specifically in Brooklyn and Manhattan, to reduce the high volume of vehicle accidents.
Healthcare Staffing: Address staff shortages at Kings County Hospital to reduce medical malpractice claims.
Correction & Police Reform: Increase the use of cameras and digital evidence storage to prevent "evidence decay" and defend against speculative claims .
Early Mediation: Establish early mediation programs for high-severity PI cases where liability is clear to avoid mounting legal fees and statutory interest.
