---
title: GH Archive ETL
short_title: gharchive_etl
tags: [python, git, pyspark, spark, google-cloud, terraform, mage-orchestrator, docker, docker-compose, venv]
category: engineering
---
Through leveraging data from GH Archive, I've developed an Extract, Transform, Load (**ETL**) pipeline to clean raw data, insert it into a centralized **data lake**, and process it into a structured **data warehouse** for analysis. The pipeline handles both **batch processing** for historical data and **real-time hourly updates**. By implementing this pipeline, I aimed to provide improved **insights into GitHub activity** while ensuring **data reliability** and facilitating future advanced **analytics**. 

<img src="assets/images/gharchive_fig.png?raw=true"/>

<u><b>Tools</b></u>: **Python**, **Git**, **Pyspark/Apache Spark 3**, **Google Cloud**(Cloud Run, Google Cloud Storage, Google BigQuery), **Terraform**, **Mage Orchestrator**, **venv**, **Looker Studio**

<Strong>[Repository link](https://github.com/AlmudenaZhou/data-engineer-gharchive)</strong>
