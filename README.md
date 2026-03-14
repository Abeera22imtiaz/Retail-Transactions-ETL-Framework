# Retail Transactions ETL Framework 🚀

An end-to-end Data Engineering pipeline built with **PySpark** on **Azure Databricks**. This project demonstrates a modular ETL (Extract, Transform, Load) architecture to process retail sales data and generate business-critical insights using **Delta Lake**.

##  Architecture Overview
The framework is designed with modularity in mind, separating each stage of the ETL process into dedicated notebooks for scalability and maintainability.

* **Data Lakehouse:** Utilizing **Delta Lake** for ACID transactions and unified batch processing.
* **Storage:** Data is managed via **Databricks Volumes** (Raw, Bronze, and Gold layers).
* **Processing Engine:** Apache Spark (PySpark) on Databricks.

## 📁 Project Structure & Modules
- `extractor`: Connects to data sources and ingests raw transaction and customer datasets.
- `transform`: Implements business logic, including complex joins and filtering (e.g., Apple iPhone and AirPods transaction analysis).
- `loader`: Handles the loading of processed data into optimized **Delta Tables**.
- `reader_factory` & `loader_sink`: Reusable utility modules for consistent data I/O.
- `Apple_analysis`: Analytical notebook providing final business metrics and visualizations.

## 🛠️ Tech Stack
* **Language:** Python (PySpark)
* **Platform:** Azure Databricks / Databricks Community Edition
* **Format:** Delta Lake, Parquet
* **Orchestration:** Databricks Workflows

## 💡 Key Features
* **Modular Pipeline:** Easy to debug and extend by adding new transformation modules.
* **Schema Enforcement:** Leverages Delta Lake to ensure data quality.
* **Efficient Joining:** Optimized Spark logic for handling multi-source retail data.
* **Production Ready:** Designed to be easily integrated into automated Databricks Jobs.

---
*Developed by [Abeera Imtiaz](https://github.com/Abeera22imtiaz)* *Computer Systems Engineer | Machine Learning & Data Engineering Enthusiast*
