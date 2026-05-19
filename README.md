# AI Governance Frameworks 🏛️

Welcome to the **AI Governance Frameworks** repository. This project represents a hands-on learning journey and an educational design exercise dedicated to exploring how abstract AI policies can be translated into structured engineering requirements. 

Using high-stakes automated HR recruitment and resume screening as a foundational anchor (inspired by historical precedents like the Amazon hiring system case study), this repository demonstrates how to break down complex global regulations into logical, auditable blueprints.

---

## 📂 Repository Architecture

This repository splits the AI risk lifecycle into two complementary, conceptual artifacts:

┌────────────────────────────────────────┐
              │ 1. AI Risk Checklist (Hiring System)   │
              │    - Diagnostic Audit Tool             │
              │    - Evaluates & Scores System Risks   │
              └───────────────────┬────────────────────┘
                                  │
                                  ▼
              ┌────────────────────────────────────────┐
              │ 2. Resume Screening Governance Matrix │
              │    - Operational Lifecycle Blueprint   │
              │    - Continuous Control Loop (NIST)    │
              └────────────────────────────────────────┘

              ### 1. [AI Risk Checklist — Hiring System](./ai-risk-checklist-hiring.md)
* **Purpose:** A diagnostic audit tool designed to turn qualitative risk evaluation into a structured, quantitative checklist. 
* **Core Logic:** Uses an objective scoring system (`Yes = 0`, `Not Sure = 1`, `No = 2`) across 4 critical risk dimensions to sort an AI application into distinct risk tiers (Low, Medium, High).
* **Case Study Validation:** Pre-populated using a retroactive audit of the defunct historical Amazon hiring tool, resulting in a maximum severity score of **16/16 (High Risk)** to demonstrate how structured checks flag systemic flaws before deployment.

### 2. [Resume Screening Governance Framework](./resume-screening-governance.md)
* **Purpose:** An end-to-end operational blueprint outlining a continuous organizational control loop.
* **Core Logic:** Maps the four core functional layers of the **NIST AI Risk Management Framework (AI RMF 1.0)** specifically to an internal Machine Learning resume screening pipeline.
* **Regulatory Mapping:** Connects technical engineering actions (like bias tracking, drift measurement, and logging) directly to mandatory compliance clauses under the **EU AI Act (High-Risk AI Systems under Annex III)**.

---

## 🛡️ Core Pillars & Regulatory Alignment

Both documents explore how to operationalize high-level trustworthy AI principles by explicitly mapping them to regional statutes:

* **Data Equity & Representation:** Auditing training datasets for historical bias, proxy features, and demographic equity (**EU AI Act Art. 10**).
* **Technical Stability & Monitoring:** Designing frameworks to track performance degradation and feature/data drift over time (**EU AI Act Art. 15**).
* **System Traceability:** Ensuring robust, automated logging mechanisms are built into the pipeline infrastructure (**EU AI Act Art. 12**).
* **Human Oversight & Governance:** Defining clear executive accountability (CHRO/CRO ownership) and protocols to prevent human confirmation bias (**EU AI Act Art. 14**).

---

## 🛠️ How to Utilize This Repository

This repository is built as a study guide and a practical conceptual reference, rather than a production software application.

* **For Learners & Peer Auditors:** Use the [AI Risk Checklist](./ai-risk-checklist-hiring.md) to see how a historical failure can be broken down systematically into discrete, quantifiable evaluation categories.
* **For Aspiring Applied Scientists & Engineers:** Treat the [Governance Framework Matrix](./resume-screening-governance.md) as a structural exercise to understand the organizational, data, and compliance layers required to support a machine learning pipeline.
* **For Anyone Navigating AI Regs:** Use this repository as a practical translation exercise to visualize how abstract regulatory text maps to a tangible, real-world domain.

---
*Developed as an educational blueprint to transition theoretical trustworthy AI frameworks into structured, auditable concepts.*
