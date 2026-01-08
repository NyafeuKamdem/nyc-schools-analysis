# School Incident Analysis

## 🎯 Objective
Explored the NYC School Safety dataset to identify incident patterns, perform data cleaning, and investigate data integrity.

## 🛠️ Process
- Data cleaning: Standardized column names to lowercase, replaced spaces with underscores, and removed special characters.
- Analysis: Calculated incident distributions across boroughs and identified frequent incident types using Google Sheets.
- **[Click here to access the Google Sheet](YOUR_LINK_HERE)**

## 📈 Key Findings
- **Total Records:** 6,310 rows across 1,890 unique schools.
- **Most Frequent Incident:** “NoCrim N”.
- **Geographic Focus:** 28.24% of all incidents occurred in the Bronx.

## 🔍 Insights & Anomalies
- **The "Safety in Numbers" Insight:** Initial analysis suggests that the number of schools in a building correlates with incident rates—interestingly, buildings with more schools tended to report fewer incidents.
- **Metadata Mismatch:** Found a discrepancy between the metadata (23 columns) and the actual dataset (34 columns).
- **Categorization Ambiguity:** While metadata lists 3 crime categories, the dataset contains 5 columns related to crime types, creating potential confusion for frequency reporting.
