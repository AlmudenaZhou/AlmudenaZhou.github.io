---
title: MLOps Student Performance
short_title: mlops_student_performance
tags: [python, git, aws, terraform, mlflow, mage-orchestrator, docker, docker-compose, grafana, sklearn, ci-cd, venv, sql]
category: mlops-ds
---


The Student Performance project compounds a comprehensive **MLOps pipeline** for predicting student grades, exemplifying an **effective** and **scalable** approach to **deploying** and **maintaining machine learning models** in **production**. Key components include:

- <span style="color:#6e6e6e">**Data Preprocessing and Model Training**</span>: Utilized **Mage** for robust data handling and model development.
- <span style="color:#6e6e6e">**Experiment Tracking and Model Registry**</span>: Implemented **MLflow** to streamline experiment tracking and model management, with artifacts securely stored on **AWS S3**.
- <span style="color:#6e6e6e">**Inference Pipeline**</span>: Enabled model serving via a **AWS Lambda** function and **Kinesis** for real-time streaming.
- <span style="color:#6e6e6e">**Monitoring**</span>: Integrated **Evidently** and **Grafana** for thorough tracking of model performance and data drift, with alerts sent through **SES** when drift is detected.
- <span style="color:#6e6e6e">**Infrastructure Management**</span>: Employed **Terraform** to ensure consistent and scalable infrastructure.
- <span style="color:#6e6e6e">**Development Practices**</span>: Maintained high **code quality** with tools, automated workflows using a **Makefile**, and enforced standards with **pre-commit hooks**.
- <span style="color:#6e6e6e">**CI/CD Pipeline**</span>: **Automated testing** and **deployment** for seamless updates, ensuring reliability and efficiency.


<img src="assets/images/student_performance_fig.png?raw=true"/>


<u><b>Tools</b></u>: **Python**, **Shell Script**, **Git**, **GitHub Actions**, **MLflow**, **AWS** (Lambda with ECR, Kinesis, S3, IAM, CloudWatch), **Terraform**, **Mage**, **Docker**, **docker-compose**, **Evidently**, **Grafana**, **LocalStack**, **Makefile**, **black**, **pytest**, **isort**, **pylint**, **sklearn**, **pandas**, **numpy**, **pyproject.toml**, **Pre-commit**, **venv**

<Strong>[Repository link](https://github.com/AlmudenaZhou/mlops-student-performance)</strong>
