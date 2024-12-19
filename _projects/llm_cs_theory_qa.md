---
title: Computer/Data Science Interview Assistant
short_title: cs_ds_interview_assistant
tags: [python, conda, streamlit, docker, docker-compose, grafana, llm, elastic-search, sql]
category: mlops-ds
---

The **Computer&Data Science Interview Assistant** project is a robust **RAG-based chatbot** designed to answer complex questions in computer science and data science, demonstrating an effective and scalable approach to **knowledge-based question answering**. Key components include:

- **Retrieval-Augmented Generation System**: Built with **Azure OpenAI**, **Ollama**, **Transformers** and **ElasticSearch** for embedding, retrieval, and answer generation.
- **Data Sources and Preprocessing**: Processes a Kaggle Q&A dataset and interview question book to form a unified, indexed knowledge base, with **data cleaning** and **structure checks**.
- **User Interface and Interaction**: Features a **Streamlit app** for easy user interaction, **with a feedback system** to rate response quality.
- **Performance Monitoring**: Employs **Grafana** and **PostgreSQL** to monitor costs, response times, and feedback metrics in real time.
- **Evaluation Metrics**: Implements **retrieval evaluation** using **MRR and hit rate** metrics, along with **RAG evaluation** using GPT-4 and GPT-3.5-turbo for **relevance scoring**, ensuring high answer accuracy.
- **Containerized Deployment**: Streamlined with **Docker and Docker Compose** for consistent, reliable app deployment.

<img src="assets/images/cs_theory_app.png?raw=true"/>

<u><b>Tools</b></u>: **Azure OpenAI**, **Ollama**, **SentenceTransformers**, **ElasticSearch**, **Grafana and PostGres DB**,**Streamlit**, **Python**, **Docker and docker-compose or podman**, **Conda**, **Git and Github**

<strong>[Repository link](https://github.com/AlmudenaZhou/llm-computer-science-theory-qa)</strong>