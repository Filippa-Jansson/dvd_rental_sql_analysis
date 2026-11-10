# DVD Rental SQL Analysis

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?logo=duckdb&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?logo=postgresql&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?logo=jupyter&logoColor=white)

SQL analysis of a DVD rental company's data, built as part of the SQL course in the Data Engineering program at STI.

The scenario: legacy data is stored in a SQLite database. The task was to migrate it to DuckDB, explore it with SQL and pandas, and present insights to the manager.

## Data

The [Sakila database](https://www.kaggle.com/datasets/atanaskanev/sqlite-sakila-sample-database), a sample database of a fictional DVD rental store with films, actors, customers, rentals and payments.

## What the notebook does

1. **Migrates** the SQLite database to DuckDB
2. **Explores** the data with SQL queries, using filtering, aggregation and joins across up to six tables
3. **Visualizes** results with matplotlib

## Key findings

- Movies range from **46 to 185 minutes**, with an average of about 115 minutes
- **Gina Degeneres** has played in the most movies (42)
- **Sports** has the most movies (74) and also brings in the most revenue ($5,314)
- **Bucket Brotherhood** is the most rented movie (34 rentals)
- **Karl Seal** is the top customer by total spend ($221.55)

## Project structure

```
├── data/
│   └── sqlite-sakila.db     # source data
├── sql/
│   └── load_sakila.sql      # migrates SQLite to DuckDB
├── sakila_analysis.ipynb    # analysis and charts
└── requirements.txt
```