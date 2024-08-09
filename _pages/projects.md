---
layout: page
permalink: /projects/
title: Projects
---

<div id="projects">
  <div class="project-item">
    <h3>MLOps Architecture for Real-Time Graph Database Fraud Detection</h3>
    <p>An AI-driven solution for real-time credit card fraud detection using MLOps techniques. It involves fully orchestrated pipelines, including data ingestion, model training, and real-time prediction and monitoring. The system focuses on high fraud case detection through Graph Convolutional Network, XGBoost, and CatBoost models.
    </p>
    <p><b>Tech: Neo4j graph DB, Sklearn, PyG, Mlflow, Kafka, Grafana, Mage orchestration, Docker, Streamlit</b></p>
    <a href="https://github.com/divakaivan/kb_project" target="_blank">View on GitHub</a>
  </div>
  
  <div class="project-item">
    <h3>MLOps Architecture for Insurance Fraud Detection</h3>
    <p>This project is a capstone for DataTalksClub's MLOps Zoomcamp. It involves building an end-to-end MLOps pipeline to detect car insurance fraud. The pipeline integrates tools like Terraform, Prefect, MLflow, Docker, Grafana, and Evidently, covering aspects from data storage, data preprocessing (using IV and WoE), model training, deployment, and monitoring. The project emphasizes reproducibility, orchestration, and monitoring with a focus on achieving high recall in fraud detection using a Balanced Random Forest Classifier.
    </p>
    <p><b>Tech: PostgreSQL DB, Terraform, Google Cloud Platform, Mlflow, Prefect, Grafana, Evidently, Docker, FastAPI</b></p>
    <a href="https://github.com/divakaivan/insurance-fraud-mlops-pipeline" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>Transaction Stream Data Engineering Pipeline</h3>
    <p>This project starts by generating transaction data via Stripe's API, streams it using Apache Kafka, and processes it in real-time with PySpark Structured Streaming. The processed data is stored in PostgreSQL, managed by dbt for data transformations and modelling, and visualized using Grafana.
    </p>
    <p><b>Tech: PostgreSQL DB, Kafka, PySpark, dbt, Grafana</b></p>
    <a href="https://github.com/divakaivan/transaction-stream-data-pipeline" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>Lending Club Data Engineering Pipeline</h3>
    <p>This project involves building a data pipeline using various tools and technologies to process and visualize Lending Club data. The pipeline extracts raw data from Kaggle, loads it into Google Cloud Storage, processes it with dbt in BigQuery, and creates visualizations using Looker. Terraform is used for infrastructure management, and Mage orchestrates the entire process.
    </p>
    <p><b>Tech: Docker, Mage orchestration, Google Cloud Platform, Terraform, dbt, Looker</b></p>
    <a href="https://github.com/divakaivan/lending-club-data-pipeline" target="_blank">View Project</a>
  </div>
</div>

<style>
  #projects {
    display: block;
  }

  .project-item {
    border: 1px solid #ccc;
    padding: 20px;
    border-radius: 8px;
    width: 100%;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    margin-bottom: 20px;
  }

  .project-item h3 {
    margin-top: 0;
  }

  .project-item a {
    display: inline-block;
    margin-top: 10px;
    color: #007BFF;
    text-decoration: none;
  }

  .project-item a:hover {
    text-decoration: underline;
  }
</style>
