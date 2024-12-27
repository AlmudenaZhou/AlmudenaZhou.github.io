---
title: Computer & Data Science Interview Assistant
short_title: cs_ds_interview_assistant
tags: [python, conda, streamlit, docker, docker-compose, grafana, llm, elastic-search, sql]
category: genai-llm
---

A robust **RAG-based chatbot** designed to provide accurate answers to complex computer science and data science questions, utilizing a **knowledge-based question-answering** approach. The system includes **real-time evaluation and monitoring**, ensuring high accuracy, relevance, and performance.

**Highlights:**

- **Retrieval-Augmented Generation System:** Developed using Azure OpenAI, Ollama, Transformers, and ElasticSearch for embedding, retrieval, and answer generation.
- **Data Sources and Preprocessing:** Unified a Kaggle Q&A dataset and an interview question book into a clean, indexed knowledge base with thorough **data preprocessing and structure checks**.
- **User Interface:** Built a **Streamlit app with a feedback system** for users to rate response quality.
- **Performance Monitoring:** Integrated **Grafana and PostgreSQL** to track costs, response times, and feedback metrics in real time.
- **Evaluation Metrics:** Used **MRR, hit rate, and RAG evaluation** with GPT-4/GPT-3.5-turbo to ensure high answer accuracy and relevance.
- **Containerized Deployment:** Streamlined with **Docker and Docker Compose** for consistent and reliable application deployment.

**Impact:** Enhanced learning and interview preparation by providing an **intelligent, real-time assistant** capable of answering complex questions with **precision and minimal hallucinations**, while continuously **monitoring** and optimizing performance metrics to deliver reliable and relevant results.

<img src="assets/images/cs_theory_app.png?raw=true"/>

<u><b>Tools</b></u>: **Azure OpenAI**, **Ollama**, **SentenceTransformers**, **ElasticSearch**, **Grafana and PostGres DB**,**Streamlit**, **Python**, **Docker and docker-compose or podman**, **Conda**, **Git and Github**

<strong>[Repository link](https://github.com/AlmudenaZhou/llm-computer-science-theory-qa)</strong>