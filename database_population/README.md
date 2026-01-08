# Database Population & ETL

## 🎯 Objective
This stage focused on data engineering. I moved from simply querying data to cleaning and injecting new data into a PostgreSQL database. The goal was to take raw SAT results and integrate them into the existing relational schema.

## 🛠️ Data Engineering Process
- **Data Auditing:** Inspected the raw SAT dataset to identify relational keys (DBN) and separate useful metrics from synthetic or "dirty" data.
- **Cleaning & Validation:**
    - Filtered SAT scores to ensure they fell within the valid range (200–800).
    - Handled inconsistent formatting (e.g., removing '%' signs and converting to numeric types).
    - Removed duplicates and handled null values to maintain database integrity.
- **Database Injection:** Developed a Python script using `sqlalchemy` to append the cleaned data into a custom table (`kamdem-nyafeu_sat_results`).

## 📁 Outputs
- `cleaned_sat_results.csv`: The final, processed dataset ready for production use.
- `sat_modeling.ipynb`: The notebook documenting the logic for cleaning, transformation, and the final database commit.

## ⚙️ Technical Stack
- **Languages:** Python
- **Libraries:** Pandas, SQLAlchemy, Psycopg2
- **Database:** PostgreSQL
