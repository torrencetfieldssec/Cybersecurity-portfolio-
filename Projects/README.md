# Situation Awareness Report Generator for NGOs (AI for Social Good domain)
---
## Project Overview

The Report Generator is a Python based, AI-powered tool designed to automate the creation of multilingual situation awareness reports for humanitarian organizations operating in conflict zones. Non Governmental Organizations (NGOs) need to track conflict and humanitarian data across multiple sources, however analysts often spend days manually compiling reports, which delays critical response planning. This application automates data aggregation and generates comprehensive reports with verified citations in 6 minutes. By leveraging hybrid retrieval-augmented generation (RAG) and citation verification, the system reduces errors, saves analysts time, and enables faster humanitarian response.

**Keywords**: Humanitarian AI, Hybrid RAG, Citation Verification, Multilingual Reports

---

## Data Sources

The platform integrates multiple reputable humanitarian open source datasets:

- **ACLED** – Armed Conflict Location and Event Data Project 
- **GDELT** – Global Database of Events, Language and Tone
- **ReliefWeb** – Humanitarian Information service by the Office for the coordination of Humanitarian Affairs (OCHA)
- **World Bank** – International financial institution providing global economic indicators and development data 

---

## System Architecture

The system uses a **unified, monolithic architecture** running within Google Colab to simplify deployment and collaboration.

### Architecture Components
- Data ingestion and preprocessing
- Vector embedding and similarity search
- Retrieval-augmented generation (RAG)
- Visualization and report output

![System Architecture](screenshots/system-architecture.png)

---

## Frontend

- **Gradio**  
  Provides a simple, interactive user interface that runs directly inside Google Colab, which enabled fast iteration and usability testing without a full web stack.

- **Plotly**  
  Used to generate interactive charts and graphs, allowing users to explore trends and patterns in humanitarian and risk data.

---

## Backend

- **Google Colab**  
  Hosts the entire codebase, which improved accessibility and made colaboration simple across team members.

- **LangChain**  
  Structures the hybrid retrieval-augmented generation (RAG) pipeline, managing document chunking, retrieval flow, and prompt formatting.

- **FAISS**  
  Serves as the vector database for fast and efficient similarity search across embedded documents.

- **HuggingFace Models**  
  - **Embeddings**: `sentence-transformers/all-mpnet-base-v2`
  - **LLM**: LLaMA 3.2 3B Instruct  
  Selected for strong performance while remaining efficient in Colab’s GPU-accelerated environment.

---

## Sample Outputs

### Interactive Graph
This example shows an interactive graph generated from aggregated humanitarian and risk data.

![Sample Graph](screenshots/sample-graph.png)

---

### Generated Situational Report
This sample demonstrates an automatically generated report created using retrieved documents.

![Sample Report](screenshots/sample-report.png)

---

## Key Features

- Multi-source data aggregation
- Retrieval-augmented report generation
- Interactive visual analytics
- Robust Citation Verification System
- Rapid prototyping and collaboration via Colab

---

## Skills Demonstrated

- Python data processing and analysis
- NLP and vector embeddings
- LLM integration and prompt engineering
- Hybrid Retrieval-Augmented Generation 
- Data visualization and UI design
- Ethical data handling and reporting
- Collaborative development workflows (Jira)

---

## Use Cases

- Humanitarian situational awareness
- Conflict and risk monitoring
- Early warning and trend analysis
- Research support for NGOs and analysts
- Automated briefing and reporting

---

## Contributors

- **Torrence Fields**
- **Rahul Krishna**
- **Madeline Scogin**
- **Daniel Pulido**
- **Leandro Cabezas**

##
- Disclamer: The secrets needed to run this project are not included for security reasons, but the repository fully demonstrates the project’s design, data pipeline, and reporting capabilities.

