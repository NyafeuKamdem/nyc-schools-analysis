# Database Queries & Data Auditing

## 🎯 Objective
Integrated Python with a PostgreSQL database to perform advanced data retrieval. The goal was to join demographic data with school directories to identify support levels for English Language Learners (ELL) and Special Education students.

## 🛠️ Process
- **Database Connection:** Established a secure connection using `psycopg2` and `sqlalchemy` to query the `nyc_schools` database.
- **SQL Integration:** Used `pandas.read_sql()` to pull relational data directly into dataframes for analysis.
- **Join Logic:** Attempted to merge `school_demographics` and `high_school_directory` to map specific needs by borough.

## 📈 Key Findings
- **School Distribution:** Brooklyn (121) and the Bronx (118) lead in school count, while Staten Island (10) has the fewest.
- **Manhattan ELL Trends:** English Language Learner percentages in Manhattan showed a steady increase over time, rising from 5.68% (05-06) to 11.96% (11-12).

## ⚠️ Critical Data Audit (Anomalies)
- **Data Gap:** A major limitation was discovered—the `school_demographics` table only contains records for **Manhattan**. 
- **Impact:** Analysis for Brooklyn, Bronx, Queens, and Staten Island regarding ELL and Special Education percentages was impossible due to this missing data.
- **Recommendation:** The project requires a more complete demographic dataset for the four missing boroughs to draw city-wide conclusions.
