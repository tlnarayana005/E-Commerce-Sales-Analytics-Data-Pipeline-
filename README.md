# E-Commerce Sales Analytics & Data Pipeline (`ecommerce-sales-analytics`)

**Automated data extraction, SQL database ingestion, and business intelligence analytics on Brazilian e-commerce market trends.**

---

## 📌 Project Overview
An end-to-end data analytics and engineering pipeline designed to derive actionable business insights from a large-scale Brazilian e-commerce dataset containing over 100,000 orders (2016–2018). The workflow covers data extraction, schema creation, data cleaning, automated ingestion into MySQL, and comprehensive analytical querying with visualizations.

---

## 🚀 Key Features

- **Automated Data Pipeline (`CSV_to_SQL.py`):** Automatically maps pandas datatypes to SQL schemas, handles missing/null records, and loads multi-relational CSV tables directly into MySQL.
- **In-Depth SQL Analytics (`Problem Queries.txt`):** Includes basic, intermediate, and advanced queries covering revenue distribution, customer retention rates, cohort behaviors, and year-over-year growth.
- **Exploratory Data Analysis & Visualizations (`python+sql_ecommerce project.ipynb`):** Interactive notebook demonstrating trends, seller revenue rankings, moving averages, and market distribution using Seaborn and Matplotlib.

---

## 🛠️ Tech Stack

- **Language:** Python 3.x
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, MySQL Connector
- **Database:** MySQL
- **Environment:** Jupyter Notebook

---

## 📂 Project Structure

```text
ecommerce-sales-analytics/
├── CSV_to_SQL.py                          # Data ingestion script from CSVs to MySQL
├── Problem Queries.txt                    # Business intelligence SQL queries (Basic, Intermediate, Advanced)
├── python+sql_ecommerce project.ipynb     # Jupyter notebook containing EDA & Visualizations
├── dataset_link.txt                       # Reference link to dataset files
├── .gitignore                             # Git ignore rules
└── README.md                              # Project documentation
```

---

## ⚙️ Setup & Execution

1. **Clone the repository:**
   ```bash
   git clone https://github.com/tlnarayana005/E-Commerce-Sales-Analytics-Data-Pipeline-.git
   cd E-Commerce-Sales-Analytics-Data-Pipeline-
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas mysql-connector-python matplotlib seaborn jupyter
   ```

3. **Configure Database Connection:**
   Update your database credentials in `CSV_to_SQL.py`:
   ```python
   conn = mysql.connector.connect(
       host='localhost',
       user='your_username',
       password='your_password',
       database='your_database'
   )
   ```

4. **Run the Ingestion Pipeline:**
   ```bash
   python CSV_to_SQL.py
   ```

5. **Launch Jupyter Notebook for Analysis:**
   ```bash
   jupyter notebook "python+sql_ecommerce project.ipynb"
   ```
