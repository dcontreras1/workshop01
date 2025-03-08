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

# Conclusions
1. Hiring is spread across many technologies without one standing out the most.

Some technologies, like Security, Mulesoft, and QA Manual, have a slightly higher number of hires, but the difference isn’t very big.
This means that job opportunities are fairly balanced across different areas of technology, rather than being focused on just a few.

2. Experience level doesn’t seem to be a big obstacle for getting hired.

The Hires by Experience Level chart shows that hiring is pretty even across all experience levels.
This suggests that companies are open to hiring both experienced workers and those just starting their careers.

3. The number of hires has changed over the years.

Hiring went up from 2018 to 2019, then stayed mostly steady from 2020 onward.
The drop in 2022 might not mean much because the data only covers the first half of the year.

4. Hiring patterns are different in each country.

The United States has seen a steady rise in hiring, especially in recent years.
On the other hand, Colombia and Ecuador have had fewer hires over time.
Brazil’s hiring numbers have gone up and down, possibly due to changes in the economy or shifts in what companies need.