# LA03-Azure-Databricks-Transform-data
# Transform Data with Apache Spark in Azure Databricks

## 📌 Project Overview

This lab focuses on data transformation using **Apache Spark** in **Azure Databricks**, a powerful analytics platform integrated into the Microsoft Azure ecosystem. Azure Databricks enables scalable data processing and analysis through Spark-based clusters and notebooks.

This hands-on exercise demonstrates key data engineering tasks such as:
- Provisioning a Databricks workspace
- Creating a Spark cluster
- Ingesting data from external sources
- Cleaning and transforming data
- Performing aggregations and filtering
- Running SQL queries over Spark DataFrames


## 🎯 Learning Objectives

By completing this lab, I learned how to:

- Set up a **Databricks Workspace** and Spark **cluster** using the Azure Portal and Cloud Shell
- Use **Apache Spark DataFrames** to manipulate data
- Clean and transform raw CSV files using PySpark
- Perform **aggregations** and **grouping** on datasets
- Filter data with conditions and extract insights
- Combine multiple transformation functions using method chaining
- Run **SQL queries** directly in Databricks notebooks
- Understand the basics of ETL (Extract, Transform, Load) pipelines in a cloud environment


## 🛠️ Technologies Used

- **Microsoft Azure Portal**
- **Azure Cloud Shell** (PowerShell)
- **Azure Databricks**
- **Apache Spark (via Databricks Runtime 13.3 LTS)**
- **PySpark (Python API for Spark)**
- **GitHub (for dataset repository)**


## 🗂️ Steps Followed

### 1. Provision Azure Databricks Workspace
- Used the provided `setup.ps1` script in Azure Cloud Shell to automatically deploy a Databricks workspace.
- Validated the resource group and Databricks service creation.

### 2. Create a Spark Cluster
- Created a single-node cluster to minimize resource usage.
- Enabled Photon acceleration for performance.
- Selected Databricks Runtime 15.4 LTS.

### 3. Create a Notebook
- Created a notebook titled **"Transform data with Spark"** and attached the newly created cluster.

### 4. Ingest External Data
- Downloaded CSV files (2019, 2020, 2021) from GitHub to the Databricks file system using shell commands.

### 5. Define Schema and Load Data
- Applied a defined schema to import data into a DataFrame.
- Displayed sample rows to verify schema accuracy.

### 6. Clean and Prepare Data
- Removed duplicate entries.
- Recalculated `Tax` column based on `UnitPrice`.
- Cast `Tax` values back to `float` to optimize performance.

### 7. Filter and Select Specific Data
- Selected customer names and emails.
- Filtered specific products using conditions.
- Counted total and unique customers.

### 8. Aggregate Data
- Summed quantities of each product using `groupBy`.
- Counted total sales per year and sorted by year.

### 9. Run SQL Queries
- Practiced using SQL syntax directly in notebook cells to query the Spark data.


## 💡 Key Takeaways

- Azure Databricks is an efficient tool for large-scale data transformation and analysis.
- Apache Spark simplifies complex data operations like filtering, aggregating, and cleaning.
- Spark DataFrames offer a flexible structure that supports both functional (PySpark) and declarative (SQL) paradigms.
- Automation through scripts makes provisioning Azure resources faster and consistent.

## Screenshots

<img width="886" alt="1" src="https://github.com/user-attachments/assets/e55d8faa-b061-4d20-959c-5d4c012c0075" />


<img width="885" alt="2" src="https://github.com/user-attachments/assets/dc3d277d-b6cd-4c4c-83a0-9fb74953cc9a" />


<img width="882" alt="3" src="https://github.com/user-attachments/assets/689ea9ab-3513-40c0-a0b0-02887244a23c" />


<img width="895" alt="4" src="https://github.com/user-attachments/assets/7c27bf69-6678-4546-b02f-acf01c970df1" />


<img width="891" alt="5" src="https://github.com/user-attachments/assets/4ba7ef1f-f9ca-490f-a0bb-5208b9e63308" />

<img width="891" alt="6" src="https://github.com/user-attachments/assets/f0265d28-b02d-413a-b1cd-c0a48117ec1b" />


