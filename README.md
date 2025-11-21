End-to-End Data Project using Microsoft Fabric For NYC Yellow Taxi Data

A complete analytics workflow for data analysts and BI engineers

📘 Overview

This repository implements an end-to-end data analytics project using Microsoft Fabric. Starting with raw data ingestion, we move through transformation, modelling and reporting — providing actionable insights for decision-making.

The use case: NYC taxi data (or whichever dataset you choose) — demonstrate data engineering, modelling and visualization in one unified platform.

🚀 Project Workflow

<img width="1221" height="392" alt="image" src="https://github.com/user-attachments/assets/7db70552-4740-4c6b-ba9c-f14988c0f53f" />


Here’s what the project covers:

Data Ingestion

Load raw data (e.g., taxi trip records) into a lakehouse or data lake within Microsoft Fabric.

<img width="1243" height="192" alt="image" src="https://github.com/user-attachments/assets/4c2f8ffa-70f5-477d-b741-3fa90207331a" />

<img width="558" height="195" alt="image" src="https://github.com/user-attachments/assets/b203fb4f-56ac-4f55-86e0-7a4f782dc945" />



Use Dataflows / Pipelines for ingestion.

<img width="992" height="213" alt="image" src="https://github.com/user-attachments/assets/6bf3f1fa-fa67-402a-bc94-0e1831f03f31" />

Data Transformation & Storage

Clean and prepare data: apply filters, derive new features (trip duration, distance, passenger count analysis).

Store as Delta tables / relational tables.

<img width="517" height="183" alt="image" src="https://github.com/user-attachments/assets/1f13543a-865e-491f-93e9-a685c56b698a" />


Modelling

Build a semantic model / dimensional model (facts + dimensions).



Optimize for reporting (star schema, aggregated tables).

Reporting & Visualization

Use Power BI (or Fabric’s built-in reporting) to create dashboards: trip volumes, revenue by zone, time-series analysis.

Embed insights / allow self-service exploration.

Governance & Sharing

Leverage Fabric’s workspace, OneLake, catalog for metadata & sharing.

Secure data access, maintain data lineage.

📁 Repository Structure
/data/
  raw/            # original datasets
  processed/      # cleaned/transformed data
/scripts/
  ingestion.py    # code or notebook for ingestion
  transform.ipynb # transformation notebook
/models/
  semantic_model.sql
  star_schema_design.md
/reports/
  dashboard.pbix   # Power BI file
docs/
  architecture_diagram.png
README.md


Feel free to adapt to your project’s actual files.

🛠 Technologies & Tools

Microsoft Fabric (Lakehouse, Dataflows, Pipelines)

Delta Lake / OneLake storage

SQL / Synapse SQL

Power BI for reporting

(Optional) PySpark / Notebooks for advanced transformation

Metadata & governance using Fabric Catalog

<img width="1032" height="647" alt="image" src="https://github.com/user-attachments/assets/89f14fea-0dbf-4ab5-b940-30b0bf384c9c" />


✅ Setup & Running the Project

Clone the repo:

git clone https://github.com/yourusername/your-repo.git


In Fabric workspace:

Create a Lakehouse (link to docs)

Upload raw data to /data/raw

Run ingestion script / notebook to load data into Lakehouse.

Execute transformation notebook to derive processed tables into /data/processed.

Deploy semantic model (SQL script) to build your modelling layer.

Open dashboard.pbix in Power BI → connect to the semantic model → publish to service.

<img width="2310" height="1292" alt="image" src="https://github.com/user-attachments/assets/ea93be1d-3c3b-4290-96e9-f243c197d713" />


Configure sharing & access via Fabric workspace, assign roles/groups.

🔍 Key Insights / Features

Trip duration & distance analysis by taxi zone.

Peak hour vs off-peak comparison.

Revenue by zone and passenger count trends.

Self-service dashboard enabling ad-hoc slice & dice.

Unified platform approach: ingestion → modelling → reporting in one place.

🧩 How to Extend

Add streaming data (real-time taxi data) and leverage Real-Time Intelligence in Fabric.

Incorporate predictive analytics (e.g., trip duration prediction using ML).

Extend semantic model with more dimensions (weather, events, holidays).

Automate refresh pipelines and set up alerts for anomalies.

