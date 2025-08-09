---
layout: page
permalink: /projects/
title: Projects
---

<details>
<summary>AI/ML/MLOps</summary>
<br>
<div id="projects">
  <div class="project-item">
    <h3>Sample ML model API following the Open Inference Protocol</h3>
    <p>
      <li>Designed following the Open Inference Protocol — a growing industry standard for standardized, observable, and interoperable machine learning inference</li>
    </p>
    <p><b>Tech: scikit-learn, FastAPI, pytest, pre-commit, Docker, Github Actions, Pydantic</b></p>
    <a href="https://github.com/divakaivan/model-api-oip" target="_blank">View Project</a>
  </div>
  
  <div class="project-item">
    <h3>MLOps 101 Project for a mini-course I teach</h3>
    <p>
      <li>After learning a tonne from great online teachers, and projects I decided to transfer my knowledge onto undergraduate students who are curious about the life of a model outside the Jupyter notebook</li>
      <li>An end-to-end ML system that processes taxi data, stores models in a model registry, exposes them via an API, and deploys this API to Google Cloud, and keeps logs for observability</li>
    </p>
    <p><b>Tech: scikit-learn, EvidentlyAI, FastAPI, MLFlow, Docker, Github Actions, Terraform, Google Cloud (GCS, Logging, Compute Engine, Artifact Registry, Kubernetes Engine)</b></p>
    <a href="https://github.com/divakaivan/mlops-101" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>MLOps Architecture for Real-Time Fraud Detection</h3>
    <p>
      <li>An AI-driven solution for real-time credit card fraud detection using MLOps techniques</li>
      <li>Fully orchestrated pipelines, including data ingestion, model training, and real-time prediction and monitoring</li>
      <li>High fraud case detection through Graph Convolutional Network, XGBoost, and CatBoost models</li>
    </p>
    <p><b>Tech: Neo4j graph DB, Sklearn, PyG, Mlflow, Kafka, Grafana, Mage orchestration, Docker, Streamlit</b></p>
    <a href="https://github.com/divakaivan/kb_project" target="_blank">View Project</a>
  </div>

  <div class="project-item">
    <h3>Voice-to-Voice Personal Finance Assistant</h3>
    <p>
      <li>Talk, Learn and Analyse your spending habits with your Personal Finance Assistant AI Agent. Communicate through speech</li>
      <li>Frontend + Backend communicating via a websocket</li>
      <li>Ask follow-up questions (the language model can see the chat history)</li>
      <li>Detailed observability of live and historical connections to the server via Pydantic Logfire</li>
    </p>
    <p><b>Tech: Webhooks, FastAPI, PydanticAI, Logfire, SQLite, OpenAI, Ollama, PostgreSQL, React</b></p>
    <a href="https://github.com/divakaivan/voice2voice-banking-assistant" target="_blank">View on GitHub</a>
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

  <h3>Other AI/ML</h3>
  <div class="project-item">
    <h4><a href="https://www.kaggle.com/divakaivan12/code" target="_blank">Notebook Expert on Kaggle</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://www.kaggle.com/code/divakaivan12/the-full-story-behind-multicollinearity" target="_blank">Diving into the full story behind multicollinearity</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/LingoMate" target="_blank">LingoMate - hackathon project for language learners</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://www.kaggle.com/code/divakaivan12/neural-network-epoch-by-hand" target="_blank">Doing a neural network epoch+math by hand</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/text2chart" target="_blank">text2chart - transforming natural language to charts</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/pdf-rag-from-scratch" target="_blank">PDF RAG from scratch</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/taxi-demand-video-models-paper" target="_blank">Using Video Generation Models for Taxi OD Demand Matrix Predictions</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/db2chat" target="_blank">db2chat - chat with your (SQLite) database</a></h4>
  </div>
</div>
</details>

---

<details>
<summary>Data Eng</summary>
<br>
<div class="project-item">
    <h3>Esports Voice Data Pipeline (Zach Wilson's DE bootcamp capstone)</h3>
    <p>
      <li>Esports team communication data is normally kept private, but for the first time a team is sharing their full voice communication records so with this I am showing a prototype of a pipeline that utilises audio data to extract communication patterns</li>
      <li>In addition, I developed visualizations that uncover communication patterns and dynamics, providing the underlying team with actionable insights to enhance their gameplay</li>
    </p>
    <p><b>Tech: Airflow, dbt, Google BigQuery, Google Cloud Storage, Streamlit, Terraform, Github Actions, Astronomer</b></p>
    <a href="https://github.com/divakaivan/lolesports-voice-analytics" target="_blank">View Project</a>
  </div>

<div class="project-item">
    <h3>Write-Audit-Publish exercise YT video</h3>
    <p>
      <li>Recorded a youtube tutorial on how to follow the WAP DQ practice using popular tech</li>
    </p>
    <p><b>Tech: Dremio, Apache Iceberg, Nessie, MinIO</b></p>
    <a href="https://www.youtube.com/watch?v=CzkBkwv1Llc&ab_channel=istudythings" target="_blank">View Project</a>
  </div>

<div class="project-item">
    <h3>EU AI Act Graph Modelling</h3>
    <p>
      <li>Scraped the EU AI Act website and created a conceptual, logical and a physical data model, improving my understanding of the Act’s requirements</li>
      <li>Separated entities into Articles, Recitals, Annexes, Chapters, Versions, Summaries and implemented the physical model using a graph database</li>
    </p>
    <p><b>Tech: Python, Neo4j, BeautifulSoup</b></p>
    <a href="https://github.com/divakaivan/eu-ai-act-graph-modelling" target="_blank">View Project</a>
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
</details>

---

<details>
<summary>Web/API/Other</summary>
<br>
<div class="project-item">
    <h3>RSS Aggregator API</h3>
    <p>
      <li>Developed an API that allows users to authenticate, scrape RSS feeds, follow feeds of their choice, and view posts from those feeds</li>
      <li>The API is fully tested, dockerized, and available on Docker Hub</li>
      <li>Deployed the API in a local Kubernetes setup with dashboards for monitoring both Kubernetes and the API</li>
    </p>
    <p><b>Tech: Go, PostgreSQL, GitHub Actions, Docker, Kubernetes, Prometheus, Grafana</b></p>
    <a href="https://github.com/divakaivan/rssagg" target="_blank">View Project</a>
  </div>

<div class="project-item">
    <h3>Platform Engineering with Backstage</h3>
    <p>
      <li>Built and deployed a Python API, created CI/CD pipelines with GitHub Actions, Helm, and ArgoCD for streamlined Kubernetes deployments</li>
      <li>Registered components in Backstage’s software catalog, managed team ownership, published TechDocs, and deployed Backstage in production using Docker & Kubernetes</li>
    </p>
    <p><b>Tech: GitHub Actions, Docker, Kubernetes, ArgoCD, Helm, Backstage</b></p>
    <a href="https://www.youtube.com/watch?v=i4cQzjRNz4M" target="_blank">View Video</a>
  </div>  

  <div class="project-item">
    <h3>Sample ML model API following the Open Inference Protocol</h3>
    <p>
      <li>Designed following the Open Inference Protocol — a growing industry standard for standardized, observable, and interoperable machine learning inference</li>
    </p>
    <p><b>Tech: scikit-learn, FastAPI, pytest, pre-commit, Docker, Github Actions, Pydantic</b></p>
    <a href="https://github.com/divakaivan/model-api-oip" target="_blank">View Project</a>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/politics.news" target="_blank">politics.news - TUI for reading political news from the terminal using Go</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/classify_hangul" target="_blank">Webapp for classifying hand-written Hangul characters</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/psql-express-yelp-api" target="_blank">RESTful Node.js/Express backend for a restaurant review application</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/hanja-game" target="_blank">Webapp to Practice Hanja Characters for Hanja Exam</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://korean-quiz-game-ian6qmcm2-divakaivan.vercel.app/" target="_blank">Created a quiz webapp with custom questiones on general topics</a></h4>
  </div>
  <div class="project-item">
    <h4><a href="https://github.com/divakaivan/team-comms-discord-bot" target="_blank">Discord bot for audio transcriptions</a></h4>
  </div>
</details>
