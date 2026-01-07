# SOC Lakehouse using Azure Databricks & Power BI

## 📌 Project Overview
This project implements a **Security Operations Center (SOC) Lakehouse architecture** using **Azure Databricks, Azure Data Lake Storage Gen2 (ADLS), and Power BI** to ingest, process, and visualize security authentication logs.

The goal is to demonstrate how raw security logs can be transformed into **actionable security insights** using a modern **Medallion Architecture (Bronze → Silver → Gold)** and visualized through an interactive Power BI dashboard.

---

## 🏗️ Architecture Overview
The solution follows a **Lakehouse + Medallion Architecture**:

- **Bronze (Raw Layer)**  
  Ingest raw authentication / login logs into ADLS

- **Silver (Cleaned Layer)**  
  Clean, normalize, and enrich logs using Databricks notebooks

- **Gold (Analytics Layer)**  
  Create aggregated security metrics such as:
  - Failed logins by user
  - High-risk users
  - Event severity distribution

Gold tables are stored in **Delta format** and consumed by Power BI for analytics.

📁 Architecture diagrams and screenshots are available in the `architecture/` folder.

---

## 🛠️ Tech Stack
- **Azure Databricks** – Data processing & transformations  
- **Azure Data Lake Storage Gen2 (ADLS)** – Central data storage  
- **Delta Lake** – Reliable, query-optimized data format  
- **Power BI** – Security analytics dashboard & reporting  
- **Python / PySpark** – Data engineering logic  
- **GitHub** – Version control & documentation

---

## 📊 Power BI Dashboard
The Power BI dashboard provides:
- Failed login attempts by user
- Identification of high-risk users
- Security risk summary narrative
- Clear visuals suitable for SOC monitoring

Dashboard files and documentation are available in the `powerbi/` folder, with screenshots in `screenshots/`.

---

## 🔍 Key Learnings
- Implemented Medallion Architecture in a real SOC-style use case  
- Connected Databricks Delta tables to Power BI via ADLS Gen2  
- Built security-focused analytics instead of generic dashboards  
- Applied cloud data engineering best practices

---

## 🚀 Future Enhancements
- Integrate streaming logs (Event Hub / Kafka)
- Add anomaly detection using ML
- Automate pipelines using Databricks Jobs
- Publish Power BI report to Power BI Service with scheduled refresh

---
## 👩‍💻 Author
**Pooja Borade**  
Master’s Student – Information Technology  
Focus Areas: Cloud, Data Engineering, Security Analytics

---

⭐ If you found this project useful, feel free to explore the repository
