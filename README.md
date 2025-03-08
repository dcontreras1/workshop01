# Hires Report: Project Description
This project implements an Extract, Transform, Load (ETL) process to analyze and visualize contracting data. The data is extracted from a CSV file, loaded into a PostgreSQL database, transformed and cleaned using PSQL queries, and then used to generate visualizations in Python and Power BI. Finally, the visualizations provide valuable insights into the processed data.

# Tools Used

Python (pandas, numpy, matplotlib, seaborn, sqlalchemy)
PostgreSQL (data storage)
Jupyter Notebook / Python Scripts (data analysis and visualization)
Git and Github (version control and documentation)
Power BI

# ETL Process Flow

Extraction: The CSV file (Contracting.csv) is loaded using Pandas.
Transformation:
Column names are cleaned.
Null values are handled (filled with median or deleted if necessary).
Duplicates are removed.
Transformations are applied to normalize data.
Load: The cleaned data is stored in a PostgreSQL database.
Analysis and Visualization:
Descriptive statistics.
Histograms of key variables.

```bash
git clone https://github.com/dcontreras1/workshop01.git
cd workshop01
```

```bash
python -m venv Workshop_env
Workshop_env\Scripts\activate
```

# Instalar dependencias
```bash
pip install -r requirements.txt
```

# Configuración a la base de datos PostgreSQL
```sql
CREATE DATABASE candidatesdb;
```
# Ejecución del proyecto
1 Ejecutar el pipeline ETL
```bash
python script/development.py
```

```bash
jupyter notebook Notebook/candidates_workshop.ipynb
```

# Hires report
Hires by Technology,
Hires by Year,
Hires by Seniority,
Hires by Country Over Years.