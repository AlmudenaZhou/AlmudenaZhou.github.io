---
title: "GitHub Archive: ETL Pipeline"
short_title: gharchive_etl
tags: [python, git, pyspark, spark, google-cloud, terraform, mage-orchestrator, docker, docker-compose, venv, sql]
category: engineering
---

A **robust data pipeline** to **analyze GitHub's top contributors** and activity types, providing actionable insights into user behavior on the platform through **data engineering skills**.

**Highlights:**
- **Data Extraction and Transformation:** Utilized **Mage as an ETL orchestrator** and **PySpark for data structuring**, with structured data ingested into **BigQuery**, organizing events by time and activity type.
- **Infrastructure Automation:** Automated deployment using **Terraform on Google Cloud**, integrating **Cloud Run** for Mage hosting, **GCS** as a data lake, and **BigQuery** as the data warehouse.
- **Batch and Stream Processing:** Supported **historical batch** data **and** near real-time streaming with an **hourly trigger** for continuous updates.
- **Data Visualization:** Created a detailed **Looker Studio dashboard** to display insights on GitHub contributors, event categories, and non-commit actions for in-depth analysis.

**Impact:** Enabled detailed analysis of GitHub user actions through a **scalable and automated pipeline**, supporting data-driven decisions for platform activity insights.

<img src="assets/images/gharchive_fig.png?raw=true"/>

<u><b>Tools</b></u>: **Python**, **Git**, **Pyspark/Apache Spark 3**, **Google Cloud**(Cloud Run, Google Cloud Storage, Google BigQuery), **Terraform**, **Mage Orchestrator**, **venv**, **Looker Studio**

<Strong>[Repository link](https://github.com/AlmudenaZhou/data-engineer-gharchive)</strong>
