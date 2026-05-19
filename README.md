# AI Governance Frameworks 🏛️

A structured, operational blueprint for transforming theoretical Responsible AI principles into enforceable enterprise workflows. This repository bridges the gap between high-level policy and engineering execution by mapping auditing tools, metric thresholds, and escalation protocols directly to international standards like the **NIST AI Risk Management Framework (AI RMF 1.0)** and the mandatory compliance requirements of the **EU AI Act (High-Risk AI Systems under Annex III)**.

Using HR recruitment and automated resume screening as a high-stakes foundational anchor (inspired by real-world historical precedents like the Amazon hiring system case study), this repository provides actionable governance architectures designed for Applied Scientists, Risk Auditors, and Compliance Teams.

---

## 📂 Repository Structure

The repository splits the AI governance lifecycle into two core artifacts:

1. **[AI Risk Checklist — Hiring System](./ai-risk-checklist-hiring.md)**
   * *Purpose:* A rapid risk identification and scoring tool designed for pre-deployment screening and ongoing audits.
   * *Regulatory Mapping:* Integrates specific EU AI Act requirements (`Art. 10` Bias, `Art. 12` Logging, `Art. 14` Human Oversight, `Art. 15` Accuracy/Robustness) to calculate quantitative risk scores.
2. **[Resume Screening Governance Framework](./resume-screening-governance.md)**
   * *Purpose:* An end-to-end operational blueprint defining the corporate control loop: **Govern, Map, Measure, and Manage**.
   * *Regulatory Mapping:* Translates NIST functional layers into explicit organizational responsibilities, mathematical bias thresholds (e.g., selection ratios, drift boundaries), and automated system rollback triggers.

---

## 🏛️ Comprehensive Governance Control Loop

Both frameworks in this repository operate under a continuous oversight lifecycle, transforming passive compliance checks into active engineering controls:

+-------------------------------------------------------+
|                       GOVERN                          |
| Define Ownership, Policies, and Board-Level Authority |
+---------------------------+---------------------------+
                            |
                            v
+-------------------------------------------------------+
|                         MAP                           |
| Identify Downstream Harms, Stakeholders, and Proxies  |
+---------------------------+---------------------------+
                            |
                            v
+-------------------------------------------------------+
|                       MEASURE                         |
| Track Disparate Impact, Performance Gaps, and Drift   |
+---------------------------+---------------------------+
                            |
                            v
+-------------------------------------------------------+
|                        MANAGE                         |
| Execute Rollbacks, Human Overrides, and Incident Logs |
+-------------------------------------------------------+


---

## 🛡️ Core Governance Artifacts Breakdown

### 1. AI Risk Checklist — Hiring System
This tool converts qualitative systemic risks into measurable compliance data points. It covers four critical risk dimensions evaluated via a scoring system (`Yes = 0`, `Not Sure = 1`, `No = 2`):

* **Data Risks:** Training set inclusivity, historical pattern bias auditing, and proxy feature classification (**EU AI Act Art. 10**).
* **Model Risks:** Decision consistency across demographics, local explainability metrics, and stability against data drift (**EU AI Act Art. 15**).
* **System Usage Risks:** Automated logging mechanisms (**EU AI Act Art. 12**) and mitigation protocols for human confirmation bias (**EU AI Act Art. 14**).
* **Risk & Impact:** Explicit institutional classification within corporate risk registers (**EU AI Act Annex III**).

#### Practical Application: The Amazon Hiring System Case Study
The checklist provides an instructive historical validation by auditing the defunct Amazon hiring AI tool. Sweeping `No` responses across critical sectors result in a max-severity score of **16/16 (High Risk)**, mapping exactly how lack of technical validation leads to systemic governance failures.

---

### 2. Resume Screening Governance Framework
This framework operationalizes the **NIST AI RMF 1.0** core functions specifically for an internal Machine Learning screening pipeline:

#### 📊 Metric Threshold Matrix (The Monitoring & Detection Layer)
The framework defines explicit mathematical triggers that transition an AI system from a regular operating status to an immediate mitigation phase:

| Metric | Target / Formula | Alert/Action Threshold | Relevant Regulation |
| :--- | :--- | :--- | :--- |
| **Subgroup Selection Ratio** | $\frac{\text{Female Selection Rate}}{\text{Male Selection Rate}}$ | **$< 0.80$** (Immediate Escalation Trigger) | EU AI Act Art. 10 (Non-Discrimination) |
| **Data/Feature Drift** | Population Stability Index / Distribution Shift | **$> 10\%$ Shift** from baseline distributions | EU AI Act Art. 15 (Robustness & Stability) |
| **Human Override Frequency** | $\frac{\text{AI Decisions Reversed}}{\text{Total AI Decisions}}$ | **$> 20\%$ Overrides** across 2 consecutive cycles | EU AI Act Art. 14 (Human Oversight) |
| **Audit Trail Generation** | Automated operations trace-logging | Continuous / Mandatory operational history | EU AI Act Art. 12 (Traceability) |

#### 🚨 Incident Response & Rollback Protocols
When a metric breaches a defined safety boundary, the framework dictates a non-ambiguous escalation path:
1. **Automated Interdiction:** Instantly disable the automated rejection system; fallback to manual human review.
2. **Technical Deconstruction:** Execute global and local feature contribution audits (SHAP/LIME) to detect hidden proxies.
3. **Institutional Reporting:** Update the corporate **AI Risk Register**, inform the AI Governance Committee, and comply with mandatory regulatory incident filing protocols (**EU AI Act Art. 62**).

---

## 📈 Governance Maturity Model: Intent to Action

The fundamental thesis of this repository is that **AI failures are rarely pure algorithmic anomalies—they are structural corporate governance failures.**

┌───────────┐       ┌───────────┐       ┌────────────┐       ┌────────────┐
│  INTENT   │ ───>  │  METRICS  │ ───>  │ THRESHOLDS │ ───>  │ ESCALATION │
│ (Policy)  │       │ (Audits)  │       │ (Triggers) │       │ (Actions)  │
└───────────┘       └───────────┘       └────────────┘       └────────────┘

Without transitioning from abstract organizational policies down into explicit programmatic thresholds and automated code-level or process-level rollbacks, AI compliance remains entirely theoretical.

---

## 🛠️ How to Utilize This Repository

This repository represents a hands-on learning journey—an attempt to figure out how high-level AI policy actually translates into concrete engineering requirements. It is designed as a conceptual blueprint and an educational resource rather than a production-ready software product.

* **For Learners & Peer Auditors:** Use the [AI Risk Checklist](./ai-risk-checklist-hiring.md) as a structural reference. While it is built directly around the historical Amazon hiring case study to ground the concepts, the scoring logic and regulatory questions can serve as a learning template for analyzing other automated HR tools.
* **For Aspiring Applied Scientists & Engineers:** Treat the [Governance Framework Matrix](./resume-screening-governance.md) as a conceptual design exercise. It illustrates how an engineer might begin defining real-time monitoring metrics—like selection ratios, feature drift, and human override logs—for a machine learning pipeline.
* **For Anyone Navigating AI Regs:** Use this repo as a practical translation exercise. It serves as a study guide showing how abstract clauses from the EU AI Act and NIST frameworks might look when mapped to a tangible, real-world application.
---
*Developed as a practical architecture to transition theoretical trustworthy AI policies into auditable, deployment-ready workflows.*
