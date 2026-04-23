# Ankur Zalavadiya

**Senior Data Engineer · Data Platform Engineer**

5.8 years building production data platforms — lakehouse, streaming, CI/CD, and GenAI — for chemical manufacturing, e-commerce, retail, and healthcare. Currently based in India, open to remote work globally.

---

## What I'm doing now

Senior Data Engineer at **DCM Shriram Limited**, a multi-billion-dollar listed conglomerate. I own the end-to-end Data & AI (DNA) platform on Azure Databricks — real-time streaming, lakehouse, CI/CD, and production GenAI serving multiple chemical manufacturing plants.

Lead a cross-functional team of 4 (2 Data Engineers, 2 Data Scientists). Sole owner of the Azure DevOps CI/CD for the entire data engineering platform — Databricks Asset Bundle monorepo across DEV / TEST / PROD. Recent initiatives have delivered **₹10.8+ Cr (≈ $1.3M USD)** in measurable business value and cut Azure cloud spend by **54%** in under a year.

The code for this work is private, but the shape of it is described below.

---

## What I care about

A few principles that shape how I build:

- **Config-driven pipelines over one-off notebooks.** New use cases should be a configuration entry, not a new repo, dashboard, or cluster. One well-designed streaming pipeline can serve every real-time use case across multiple plants if the framework is right.
- **Business impact is the only KPI that matters.** A pipeline running clean at 99.9% uptime is worthless if nothing downstream depends on it. I orient projects around measurable outcomes — cost saved, revenue lifted, hours returned — before technical elegance.
- **Monorepos + Databricks Asset Bundles over scattered repos** for data platforms. Versioned, reviewable, promotable across environments, and one place to enforce standards.
- **RAG quality comes from retrieval, not the LLM.** Hybrid search + metadata filtering + thoughtful chunking beat switching to a bigger model almost every time.
- **Re-architecture is often cheaper than scaling.** Most "we need more infrastructure" problems are actually "our architecture is wrong" problems. A good rebuild reduces cost *and* improves reliability.

---

## Recently shipped (current role, private)

High-level summaries of platforms I've designed and delivered at DCM Shriram over the last 7 months:

- **Config-Driven Production Streaming Framework** — Single Spark Declarative streaming pipeline on Databricks serving every real-time plant use case via configuration entries, with built-in ADLS-staging-table backfill. Replaced notebook-based Structured Streaming jobs that were failing every few days, at 1/3 the infrastructure cost and zero repeated failures.

- **Consolidated CAPA RAG Platform (GenAI)** — Re-architected 4 independent Streamlit chatbots into a unified GenAI platform: single React frontend, FastAPI backend, FAISS on Azure Files, and a separate event-driven vector-embedding service on ACI triggered by ADLS blob notifications. Processes 70 GB of plant documents (PDF, DOCX, images, Excel) with hybrid search, metadata filtering, and source-document citations.

- **Fuel Mix Optimizer (End-to-End Rebuild)** — Full-stack production application: React + FastAPI + PostgreSQL, with a Pyomo nonlinear optimization model solved via IPOPT for coal procurement across 3 boilers under 15+ constraint sets. Delivered ₹3.4 Cr (≈ $400K USD) in savings in the first 2 months.

- **H2 Margin Maximizer (End-to-End Rebuild)** — Same architecture, but the engine is a Mixed-Integer Linear Program (Pyomo + GLPK) running every 4 minutes over live DCS sensor data from 253 tags. Recommends optimal hydrogen allocation across 11 consuming units. Delivered ₹7.4 Cr (≈ $786K USD) in savings over 6 months.

- **Platform Re-architecture** — Owned the redesign of the entire data engineering platform: cut Azure cloud spend by 54%, authored org-wide standards and templates for streaming, batch ingestion, and data-backfill jobs — now the default scaffold for every new project.

---

## Public projects (freelance era, 2020–2025)

Foundation projects from my freelance consulting years. Smaller in scope than the current-role work, but the code is open and the patterns still hold up.

### [E-commerce Analytics Data Pipeline](https://github.com/Anku1903/Shopify-Analytics-Data-Pipeline)
*Azure Data Factory · Databricks · Synapse Analytics · Tableau*

End-to-end pipeline processing 500K+ daily Shopify transactions through a medallion architecture on Azure Data Lake. Star-schema models on Synapse serverless SQL improved analytical query performance by 40%. Tableau dashboards for sales trends, customer lifetime value, and inventory optimization.

### [Data Warehouse with Snowflake & DBT](https://github.com/Anku1903/Datawarehouse-Snowflake-DBT-Airflow)
*Snowflake · DBT · Apache Airflow · Python*

Scalable data warehouse processing 2M+ daily records. 30+ DBT models with automated data quality tests, SCD Type 2 dimensions, and complex Airflow orchestration with dynamic scheduling and failure recovery.

### [Real-time Weather Analytics Platform](https://github.com/Anku1903/Realtime-WeatherAPI-Streaming-Pipeline)
*Azure Event Hubs · Databricks · Azure Functions · Microsoft Fabric*

Streaming pipeline processing 10K+ weather data points hourly with sub-second anomaly detection in PySpark. Automated alerting for critical weather conditions and live Power BI dashboards for pattern analysis.

---

## Tech stack

Grouped by how often I reach for each tool, not alphabetically.

**Daily driver**
Python · SQL · PySpark · Azure Databricks · Delta Lake · Unity Catalog · Databricks Asset Bundles · Kafka (Confluent) · FastAPI · Docker · Azure DevOps

**Regular**
Airflow · DBT · Snowflake · ADLS Gen2 · Azure Data Factory · Azure Synapse · Terraform · Kubernetes · PostgreSQL · React

**In rotation**
FAISS · LangChain · Azure OpenAI (GPT-5.1, text-embedding-3-large) · Pyomo (MILP / Nonlinear) · Tableau · AWS (S3, EC2, Glue, Lambda, Athena)

---

## Connect

- 📧 [alsoankur@gmail.com](mailto:alsoankur@gmail.com)
- 💼 [linkedin.com/in/helloankur](https://www.linkedin.com/in/helloankur/)
- 📄 Resume available on request or via LinkedIn

Open to senior data engineer / data platform engineer roles — remote-first, US / EU / India.
