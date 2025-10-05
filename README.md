# Web Server Log Processing with Apache Spark

## 📌 Overview
This project processes **web server access logs** using **Apache Spark**, cleans and transforms the raw data into a **structured schema**, and writes the output into **Parquet format** for efficient analytics and integration with BI tools.

The pipeline follows this flow:

<img width="783" height="189" alt="image" src="https://github.com/user-attachments/assets/770371ac-e060-4477-80f1-822c25f8c408" />


`Web Logs → Spark Transformations → Parquet`

---


## 🚀 Features
- Parse raw web log data.
- Extract fields:
  - Client IP
  - Timestamp
  - HTTP Method
  - Path (URL)
  - Protocol
  - Status Code
  - Content Size
  - Referrer
  - User Agent
- Convert timestamp to proper Spark `timestamp` type.
- Handle malformed or missing rows.
- Write output as **compressed Parquet files**.

---

## 🛠️ Tech Stack
- **Apache Spark (PySpark)** for distributed data processing  
- **Python** for data cleaning and transformations  
- **Parquet** for efficient columnar storage  
- **Power BI / Tableau** (optional) for visualization 
