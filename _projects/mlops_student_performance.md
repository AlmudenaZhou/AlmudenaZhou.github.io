---
title: "Student Performance: MLOps Pipeline"
short_title: mlops_student_performance
tags: [python, git, aws, terraform, mlflow, mage-orchestrator, docker, docker-compose, grafana, sklearn, ci-cd, venv, sql]
category: mlops-ds
---

A comprehensive **MLOps pipeline** for **predicting student grades**, exemplifying a scalable and effective approach to **deploying and maintaining machine learning models** in production.

**Highlights:**

- **Data Preprocessing and Model Training:** Utilized **Mage orchestrator** for robust data handling and model development.
- **Experiment Tracking and Model Registry:** Implemented **MLflow** to streamline **experiment tracking and manage models**, with artifacts securely stored in **AWS S3**.
- **Inference Pipeline:** Enabled **real-time model serving** using **AWS Lambda and Kinesis** for streaming predictions.
- **Monitoring:** Integrated **Evidently and Grafana** to **monitor** model performance and detect data drift, with **alerts sent via SES** for proactive response.
- **Infrastructure Management:** Leveraged **Terraform** to ensure consistent and scalable infrastructure provisioning.
- **Development Practices:** Ensured **high code quality** with **pre-commit hooks**, automated workflows using a **Makefile**, and adherence to best practices.
- **CI/CD Pipeline:** **Automated testing and deployment** processes to ensure seamless and reliable updates.

**Impact:** Demonstrated the **end-to-end development of a production-ready MLOps pipeline**, enabling accurate and scalable predictions while ensuring reliability, maintainability, and efficient infrastructure management.

<img src="assets/images/student_performance_fig.png?raw=true"/>


<u><b>Tools</b></u>: **Python**, **Shell Script**, **Git**, **GitHub Actions**, **MLflow**, **AWS** (Lambda with ECR, Kinesis, S3, IAM, CloudWatch), **Terraform**, **Mage**, **Docker**, **docker-compose**, **Evidently**, **Grafana**, **LocalStack**, **Makefile**, **black**, **pytest**, **isort**, **pylint**, **sklearn**, **pandas**, **numpy**, **pyproject.toml**, **Pre-commit**, **venv**

<Strong>[Repository link](https://github.com/AlmudenaZhou/mlops-student-performance)</strong>
