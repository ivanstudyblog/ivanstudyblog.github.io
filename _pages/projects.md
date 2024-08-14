---
layout: page
permalink: /projects/
title: Projects
---

<div id="projects">
  <div class="project-item">
    <h3>Your Personal Finance Voice Assistant</h3>
    <p>
      <li>Chat, Talk, Learn and Analyse your spending habits with your Personal Finance Assistant</li>
      <li>Communicate through text or speech</li>
      <li>Ask follow-up questions (the language model can see the chat history)</li>
      <li>On the dev side, see how the RAG is performing by analysing prompts and retrieved information</li>
    </p>
    <p><b>Tech: SQLite, OpenAI, HuggingFace, LlamaIndex, Azire Pheonix monitoring, Streamlit</b></p>
    <a href="https://github.com/divakaivan/personal_finance_assistant" target="_blank">View on GitHub</a>
  </div>
  
  <div class="project-item">
    <h3>MLOps Architecture for Real-Time Fraud Detection</h3>
    <p>
      <li>An AI-driven solution for real-time credit card fraud detection using MLOps techniques</li>
      <li>Fully orchestrated pipelines, including data ingestion, model training, and real-time prediction and monitoring</li>
      <li>High fraud case detection through Graph Convolutional Network, XGBoost, and CatBoost models</li>
    </p>
    <p><b>Tech: Neo4j graph DB, Sklearn, PyG, Mlflow, Kafka, Grafana, Mage orchestration, Docker, Streamlit</b></p>
    <a href="https://github.com/divakaivan/kb_project" target="_blank">View on GitHub</a>
  </div>

  <div class="project-item">
    <h3>Glaswegian Audio Dataset and ASR model</h3>
    <p>
      <li>Co-create a 120 minute open-sourced Glaswegian dataset</li>
      <li>Preprocess raw audio and transcriptions and upload to HuggingFace</li>
      <li>Research into audio AI models and fine-tune ASR and TTS models</li>
    </p>
    <p><b>Tech: HuggingFace, Python, Fine-Tuning, Audio AI</b></p>
    <a href="https://huggingface.co/datasets/divakaivan/glaswegian_audio" target="_blank">View on HuggingFace</a>
  </div>
  
  <div class="project-item">
    <h3>MLOps Architecture for Insurance Fraud Detection</h3>
    <p>
      <li>Building an end-to-end MLOps pipeline to detect car insurance fraud</li>
      <li>Pipeline orchestration covering data storage, data preprocessing (using IV and WoE), model training, deployment, and monitoring</li>
      <li>Focus on achieving high recall in fraud detection using a Balanced Random Forest Classifier</li>
    </p>
    <p><b>Tech: PostgreSQL DB, Terraform, Google Cloud Platform, Mlflow, Prefect, Grafana, Evidently, Docker, FastAPI</b></p>
    <a href="https://github.com/divakaivan/insurance-fraud-mlops-pipeline" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>Transaction Stream Data Engineering Pipeline</h3>
    <p>
      <li>Generate transaction data via Stripe's API</li>
      <li>Stream data using Apache Kafka and process it in real-time with PySpark Structured Streaming</li>
      <li>Store processed data in PostgreSQL</li>
      <li>Manage data transformations and modeling using dbt</li>
      <li>Visualize data using Grafana</li>
    </p>
    <p><b>Tech: PostgreSQL DB, Kafka, PySpark, dbt, Grafana</b></p>
    <a href="https://github.com/divakaivan/transaction-stream-data-pipeline" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>Lending Club Data Engineering Pipeline</h3>
    <p>
      <li>Build a data pipeline to process and visualize Lending Club data</li>
      <li>Extract raw data from Kaggle and load it into Google Cloud Storage</li>
      <li>Process data with dbt in BigQuery</li>
      <li>Create visualizations using Looker</li>
      <li>Manage infrastructure with Terraform</li>
      <li>Orchestrate the entire process with Mage</li>
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
    padding: 10px;
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
