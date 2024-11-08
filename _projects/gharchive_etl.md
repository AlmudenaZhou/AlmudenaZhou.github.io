---
title: GH Archive ETL
short_title: gharchive_etl
tags: [python, git, pyspark, spark, google-cloud, terraform, mage-orchestrator, docker, docker-compose, venv, sql]
category: engineering
---


The **GitHub Archive Project** constructs a **data pipeline**, **ETL**, for **analyzing GitHub's top contributors and activity types**, providing valuable insights into user actions on the platform. Key components include:

- **Data Extraction and Transformation**: Integrated **Mage as an orchestrator for ETL**, with **PySpark managing data structuring** for ingestion into **BigQuery**, where events are organized by time and activity type.
- **Infrastructure Automation**: Employed **Terraform for deploying** the project on Google Cloud, leveraging **Cloud Run** for Mage hosting, **GCS** as the data lake, and **BigQuery** as the data warehouse.
- **Batch and Stream Processing**: Handles both **historical *batch data and near real-time streaming** with an hourly trigger to ensure continuous updates.
- **Data Visualization**: Developed a comprehensive **Looker Studio dashboard** that displays insights into GitHub contributors, event categories, and non-commit actions for deeper analysis.

<img src="assets/images/gharchive_fig.png?raw=true"/>

<u><b>Tools</b></u>: **Python**, **Git**, **Pyspark/Apache Spark 3**, **Google Cloud**(Cloud Run, Google Cloud Storage, Google BigQuery), **Terraform**, **Mage Orchestrator**, **venv**, **Looker Studio**

<Strong>[Repository link](https://github.com/AlmudenaZhou/data-engineer-gharchive)</strong>
