# AdWiseAI – Agile Project Plan

## Project Summary

**AdWiseAI** is an end-to-end LLMOps system designed to automate digital advertising analysis and optimization. It ingests campaign data, generates insights using large language models (LLMs), rewrites ad copy, captures feedback, and supports monitoring and retraining pipelines. The system is built using Databricks, Azure services, and modern MLOps best practices.

**Methodology**: Agile  
**Timeline**: 6 Weeks  
**Sprints**: 1-week sprints with clear deliverables  
**Final Deliverable**: Public GitHub repository with a working API, example data, and documentation

---

## Epics Overview

| Epic # | Name                     | Description                                                |
| ------ | ------------------------ | ---------------------------------------------------------- |
| 1      | Data Ingestion & Storage | Ingest and prepare ad campaign data for analysis           |
| 2      | LLM Modules              | Build insight generator, copy rewriter, and Q&A components |
| 3      | Backend API              | Serve LLM functionality via FastAPI endpoints              |
| 4      | Feedback Logging         | Collect user feedback on generated outputs                 |
| 5      | Monitoring & Retraining  | Track usage, capture logs, and build retraining triggers   |
| 6      | Deployment & CI/CD       | Automate deployment to Azure via GitHub Actions            |
| 7      | Optional UI (Streamlit)  | Build a simple interactive interface for testing           |

---

## Timeline Overview

| Week | Sprint Name               | Focus                                     |
| ---- | ------------------------- | ----------------------------------------- |
| 1    | Sprint 1: Foundations     | Set up environment, repo, and ingest data |
| 2    | Sprint 2: Clean + Store   | Clean and structure data in Delta format  |
| 3    | Sprint 3: LLM Modules     | Insight generator and copy rewriter       |
| 4    | Sprint 4: API + Feedback  | Backend endpoints and feedback capture    |
| 5    | Sprint 5: Monitoring      | Logging, tracking, optional retraining    |
| 6    | Sprint 6: Deploy & Polish | Finalize, deploy, document, and ship      |

---

## Sprint Backlog

### Sprint 1: Foundations

**Timeframe**: Week 1

**Goals**:

- Create GitHub repo with structure
- Set up Databricks environment
- Connect Azure Blob or Table Storage
- Select or download advertising dataset
- Build ingestion script

**Deliverables**:

- GitHub repo scaffold
- Raw ad data loaded into Databricks
- Azure storage connection functional

---

### Sprint 2: Data Cleaning and Storage

**Timeframe**: Week 2

**Goals**:

- Clean raw ad data
- Engineer key metrics (CTR, CPC, ROI)
- Save processed dataset in Delta format

**Deliverables**:

- Processed ad dataset
- Reusable Databricks notebook for transformation
- Stored data in Blob or Delta Table

---

### Sprint 3: LLM Modules

**Timeframe**: Week 3

**Goals**:

- Use Azure OpenAI to generate insights
- Rewrite ad copy using prompt templates
- Test prompt quality with sample data

**Deliverables**:

- Python functions for insight and rewriting
- Prompt templates saved and versioned
- Output stored with original input and metadata

---

### Sprint 4: API and Feedback

**Timeframe**: Week 4

**Goals**:

- Build FastAPI endpoints: `/insights`, `/rewrite`, `/ask`
- Add `/feedback` endpoint for collecting ratings
- Log inputs and outputs to Delta or CosmosDB

**Deliverables**:

- FastAPI app with working routes
- Feedback schema and write path
- Manual testing via Swagger or Postman

---

### Sprint 5: Monitoring and Retraining

**Timeframe**: Week 5

**Goals**:

- Track usage stats (latency, token cost, feedback score)
- Set up Azure Monitor and Application Insights
- Write retraining script using MLflow or Azure ML

**Deliverables**:

- Basic dashboard for logs
- MLflow tracking in Databricks
- Placeholder retraining pipeline (manual)

---

### Sprint 6: Deployment and Polish

**Timeframe**: Week 6

**Goals**:

- Dockerize and deploy FastAPI to Azure App Service
- Set up CI/CD via GitHub Actions
- Finalize README and examples
- (Optional) Build Streamlit demo interface

**Deliverables**:

- Live deployed API
- GitHub Actions pipeline
- Documented project with screenshots, example inputs/outputs

---

## Final Deliverables

- End-to-end system hosted on Azure
- All code and notebooks tracked in GitHub
- CI/CD pipeline for auto-deploying the backend
- Feedback loop and monitoring included
- Prompt engineering artifacts (templates + output samples)
- Optional Streamlit UI for demo/testing
- Polished README with usage and setup
