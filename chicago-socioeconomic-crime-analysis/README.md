# Chicago Socioeconomic, Education, and Crime Data Analysis (SQL & Python)

## 📌 Project Overview
This project analyzes multi-sector open data from the City of Chicago, combining socioeconomic indicators, public school performance, and crime statistics to uncover urban patterns using Python, Pandas, and SQLite.

## 🛠️ Tech Stack & Tools
* **Python** (Pandas, SQLite3)
* **SQL** (IPython-SQL / `%sql` magic commands)
* **Database:** SQLite (`FinalDB.db`)
* **Datasets:** Chicago Census Data, Chicago Public Schools, Chicago Crime Data

## 🔍 Key Insights & Queries Solved
* Loaded and cleaned multi-source CSV files into SQLite database tables using Pandas (`df.to_sql`).
* Extracted high-poverty community areas using `ORDER BY` and `LIMIT`.
* Identified crime-prone community areas via `GROUP BY`, `COUNT(*)`, and aggregate filtering.
* Leveraged **subqueries** to link crime metrics with socio-economic hardship indices.

## 🙏 Acknowledgments
- IBM Data Science Professional Certificate — Developed as part of the Python Project for Data Science course curriculum.
