## Hi there 👋

### I'm Kyrylo.

I am an aspiring Data Engineer and I am currently learning how to build scalable data architectures and transforming raw data into actionable insights. Currently focused on mastering data processing frameworks and cloud architectures.

### Technical Skills

- **Data Engineering :** Python, SQL, Apache Airflow, Soda Core, pandas
- **Infrastructure & DevOps :** Docker, CI/CD (GitHub Actions), Git, Linux, Shell/Bash
- **Stockage :** PostgreSQL, MinIO (S3)
- **Visualisation :** Metabase

### Projects

- ### [En cours] - [Pipeline ELT YouTube Cloud — Analyse des chaînes tech francophones](https://github.com/NebylytsiaKyrylo/youtube_elt_pipeline_cloud)
  **Stack**: Python, SQL (Snowflake), dbt, AWS S3, Apache Airflow 3.2 (astronomer-cosmos), Elementary, Prometheus, Grafana, Apache Superset, uv, ruff, SQLFluff, GitHub Actions.

  **Suite cloud de mon précédent pipeline ELT, migrée vers un modern data stack (Snowflake, dbt, S3).**

  Ce projet déploie un pipeline ELT cloud pour une agence marketing spécialisée dans la tech. L'objectif est d'analyser l'influence de 40 chaînes YouTube francophones via l'API YouTube v3 afin d'orienter les décisions de partenariats.

  Architecture lakehouse hybride orchestrée par Apache Airflow : stockage brut JSON immuable dans Amazon S3, puis transformations SQL déclaratives via dbt en quatre couches (Staging, Intermediate, Core, Marts) chargées dans Snowflake. Le modèle Core suit un star schema Kimball avec deux tables de faits à grain quotidien (vidéo et chaîne), permettant l'historisation des métriques sans recourir à un SCD Type 2. La qualité des données est garantie par des tests dbt bloquants et la détection d'anomalies statistiques via Elementary. L'observabilité du pipeline (latence, taux d'échec) est exposée via Prometheus et Grafana, et les 13 marts analytiques alimentent des tableaux de bord interactifs dans Superset.

- ### [Pipeline ELT YouTube — Analyse des chaînes tech francophones](https://github.com/NebylytsiaKyrylo/youtube-elt-pipeline)
  **Stack**: Python, SQL (PostgreSQL 17), Docker, Apache Airflow 3.2, MinIO (S3), Soda Core, uv, ruff, SQLFluff, GitHub Actions et Metabase.

   Ce projet déploie un pipeline ELT automatisé conçu pour une agence marketing spécialisée dans la tech. L'objectif est d'analyser l'influence de 40 chaînes YouTube francophones via l'API YouTube v3 afin d'orienter les décisions de partenariats.

  Pipeline ELT de bout en bout orchestré par Apache Airflow 3.2. L'infrastructure repose sur une séparation stricte des responsabilités : stockage brut JSON dans MinIO, puis transformation SQL structurée en trois couches (Staging, Core, Marts) dans PostgreSQL. Ce projet met l'accent sur l'idempotence, la gestion des conflits d'insertion (UPSERT) et la robustesse opérationnelle via Docker Compose et GitHub Actions. La fiabilité du pipeline est assurée par des portes de qualité (Quality Gates) intégrées à chaque étape du chargement.
      
- ### [SQL Data Warehouse Project](https://github.com/NebylytsiaKyrylo/sql_data_warehouse_project)
  **Objective:** Develop a modern data warehouse using PostgreSQL to consolidate sales data, enabling analytical reporting and informed
  decision-making.
    
    * **Data Sources**: Import data from two source systems (ERP and CRM) provided as CSV files.
    * **Data Quality**: Cleanse and resolve data quality issues prior to analysis.
    * **Integration**: Combine both sources into a single, user-friendly data model designed for analytical queries.
    * **Scope**: Focus on the latest dataset only; historization of data is not required, SCD Type 1.
    * **Documentation**: Provide clear documentation of the data model to support both business stakeholders and analytics
      teams.

- ### [EDA and Analytics Project](https://github.com/NebylytsiaKyrylo/sql_eda_and_analytics_project.git)
   **Objective:** Develop SQL-based analytics to deliver detailed insights into:

   * **Customer Behavior:** Understanding how customers interact with products.
   * **Product Performance:** Identifying top-selling items and revenue drivers.
   * **Sales Trends:** Analyzing sales growth or decline over specific periods.
 
- ### [Walmart Retail Data Pipeline](https://github.com/NebylytsiaKyrylo/retail_data_pipeline_walmart)
  **Objective:**
  Develop a Python-based ETL pipeline to deliver clean data and aggregated insights:

   - **Extract:** Connect to a local PostgreSQL database running in Docker and load a supplementary .parquet file.
   - **Transform:** Merge datasets, handle missing values via mean imputation, extract date features, enforce schemas, and filter for high-performing sales weeks.
   - **Load:** Export the cleaned dataset and a monthly aggregated sales report into structured CSV files for downstream analytics.

- ### [Clinical Data ETL Processor](https://github.com/NebylytsiaKyrylo/clinical-data-etl-processor.git)
   **Objective:**
   Create a Python-based pipeline for integrating clinical health data with supplement usage
information. Health data from wearable devices and supplement usage logs exist in separate csv files. Clinicians and data scientists
need to cross-reference these sources manually, which is cumbersome and error-prone.

   - **Extract**: Load four CSV sources (health metrics, supplement usage, user profiles, experiments)
   - **Transform**: Clean, validate, and standardize data (type conversions, missing value handling, unit normalization)
   - **Merge**: Combine datasets into a single, comprehensive view
   - **Load**: Export analysis-ready CSV for downstream analytics
 
- ### [ETL Pipeline](https://github.com/NebylytsiaKyrylo/data-engineering)
   **Objective:**
  Create a two-stage Extract-Transform-Load (ETL) pipeline for processing sales data using Python, Flask, and AVRO serialization.
  The pipeline consists of two independent jobs that work together:

   - Job1: Extracts sales data from an external API and saves it as JSON files
   - Job2: Reads the JSON files created by Job1 and transforms them into AVRO format

### Certificates:
* **Linux Essentials Certificate** - Linux Professional Institute (LPI)
* **Data Engineer Certificate** - DataCamp (Obtained in March 2026, valid until March 2028)
* **Associate Data Engineer Certificate** - DataCamp (Obtained in September 2025, valid until September 2027)
* **Hackerrank SQL** Basic, Intermediate and Advanced Certificates (11 September 2025)
  
<!-- 
## Get in Touch

* **LinkedIn:** [Link to your LinkedIn]
* **Email:** [Your Email Address]
 -->
---
> "Without data, you're just another person with an opinion." — W. Edwards Deming
