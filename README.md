
# Data-Warehouse-ETL-Project
A data warehousing project built using SQL Server, SSIS, and Visual Studio.

---

## 🔎 Project Tasks Breakdown

### ✅ Step 1: Dataset Selection
- Selected a custom **OLTP dataset** (not OLAP or AdventureWorks).
- Dataset includes **customer**, **order**, and **product** data.
- Covers approx. **one year** of transactions (augmented with generated meaningful records).
- Ensures support for:
  - Multiple data sources
  - Rich ETL flows
  - Hierarchies and dimensions
  - Cube aggregation
  - Report generation

📌 *ER Diagram and dataset description are included in the PDF report.*

---

### ✅ Step 2: Data Source Preparation
- Organized data into **two source types**:
  - **Customer data** in CSV/Text format
  - **Order and transactional data** in SQL tables
- Introduced additional fields such as **product categories** and **hierarchies** for enriched analysis.

📌 *Source descriptions and file formats are documented in the report.*

---

### ✅ Step 3: Solution Architecture
- Designed a high-level architecture including:
  - Source layer
  - Staging area
  - ETL pipeline
  - Data warehouse layer (fact + dimensions)
  - BI/reporting layer

📌 *Architecture diagram and component explanation provided in the report.*

---

### ✅ Step 4: Data Warehouse Design & Development
- Developed a **dimensional model** using **Star Schema**:
  - At least **two custom dimensions** (e.g., Product, Customer)
  - **Date dimension**
  - **One fact table** (e.g., Sales Fact)
  - **Slowly Changing Dimension (SCD Type 2)** handled

- Implemented schema in SQL Server using **SSMS**.

📌 *Relational diagrams and design assumptions are included in the PDF.*

---

### ✅ Step 5: ETL Process (SSIS)
- Built ETL pipeline using **SQL Server Integration Services (SSIS)**:
  - Extracted data from both CSV and SQL sources
  - Applied transformations (lookups, derived columns, data conversions)
  - Loaded data into warehouse schema

📌 *Step-by-step ETL task flow is documented in the report with screenshots.*

---

### ✅ Step 6: Accumulating Fact Table Handling
- Extended fact table with:
  - `accm_txn_create_time`
  - `accm_txn_complete_time`
  - `txn_process_time_hours`
  
- Created a **second ETL package** to:
  - Update the `accm_txn_complete_time` using a separate data source (CSV or table)
  - Calculate `txn_process_time_hours` dynamically

📌 *ETL logic, update strategy, and transformation steps are explained in the report.*

---

## 🧠 Key Features

- 📁 Multi-source data integration
- 📊 Star schema with dimensional modeling
- ⚙️ SSIS-based ETL pipelines
- 🕒 Handling of accumulating fact tables
- 🧮 Support for reporting and aggregation
- 🗃️ Type 2 SCD implementation
- 📷 Detailed documentation and screenshots

---

## 📚 Academic Context

| Field          | Details                                           |
|----------------|---------------------------------------------------|
| Module         | IT3021 – Data Warehousing and Business Intelligence |
| Program        | BSc (Hons) in Information Technology – Data Science |
| Institution    | [Your Campus Name Here]                           |
| Semester       | Semester 1, 2025                                  |

---

## 👩‍💻 Author

**Savindi Abeykoon**  
[LinkedIn](https://www.linkedin.com/in/yourprofile) | [GitHub](https://github.com/yourusername)

---

