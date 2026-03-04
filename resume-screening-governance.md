# AI Governance Artifact  
## Resume Screening Model  
### Case Study Inspired by the Amazon Hiring System

---

## Table of Contents

- [Overview](#overview)
- [AI Governance Control Loop](#ai-governance-control-loop)
- [Governance Control Framework](#governance-control-framework)
- [Govern — Ownership Layer](#1-govern--ownership-layer)
- [Map — Risk Discovery Layer](#2-map--risk-discovery-layer)
- [Measure — Detection Layer](#3-measure--detection-layer)
- [Manage — Response Layer](#4-manage--response-layer)
- [Key Governance Insight](#key-governance-insight)
- [Governance Maturity Model](#governance-maturity-model)
- [Key Governance Takeaways](#key-governance-takeaways)
- [Governance Implementation Checklist](#governance-implementation-checklist)
- [Note](#note)

  ----
  ## 📌 Overview

This document presents a governance framework for an AI-based **resume screening system** used to shortlist job candidates.

The objective is to demonstrate how **AI governance principles can be operationalized** through structured oversight, risk identification, monitoring, and response mechanisms.

This artifact draws inspiration from the **Amazon hiring AI case**, where bias emerged due to historical training data and lack of governance oversight.

----

# AI Governance Control Loop

        +-----------+
        |  GOVERN   |
        | Ownership |
        +-----+-----+
              |
              v
        +-----+-----+
        |   MAP     |
        | Risk Scan |
        +-----+-----+
              |
              v
        +-----+-----+
        |  MEASURE  |
        | Monitoring|
        +-----+-----+
              |
              v
        +-----+-----+
        |  MANAGE   |
        | Response  |
        +-----------+
              |
              v
          Continuous
           Oversight

   -----           

# Governance Control Framework

The governance model follows four layers:

| Layer | Purpose |
|------|--------|
| **Govern** | Define ownership and accountability |
| **Map** | Identify risks and impacted stakeholders |
| **Measure** | Monitor fairness, drift, and system behavior |
| **Manage** | Escalate and respond to risk events |

---

# 1️⃣ GOVERN — Ownership Layer

Defines **who is responsible for AI oversight and decision authority**.

### Who Approves AI Use?

- Chief Human Resources Officer (**CHRO**)
- Chief Risk Officer (**CRO**)
- AI Governance Committee

For high-risk AI systems, **board-level oversight** may also apply.

---

### Who Defines Acceptable Risk?

An **Executive Risk Committee** including:

- HR leadership  
- Legal & compliance  
- Risk management  
- AI/ML leadership  

Responsibilities include defining:

- fairness thresholds  
- monitoring requirements  
- acceptable risk tolerance

---

### Who Signs Off Before Deployment?

Deployment approval should involve:

- Data Science Lead  
- HR Lead  
- Legal Representative  
- Risk Officer  
- Ethics / Compliance Representative  

Deployment should only occur after:

- fairness validation  
- subgroup performance testing  
- documentation of residual risk

---

### Required Policies

Organizations should implement policies such as:

- Equal Opportunity Hiring Policy  
- Bias & Fairness Testing Policy  
- Mandatory Subgroup Evaluation  
- Human-in-the-loop Hiring Policy  
- AI Monitoring & Incident Escalation Policy  

Governance must be **documented and enforceable**.

---

# 2️⃣ MAP — Risk Discovery Layer

Identifies **where harm can occur and who may be affected**.

### Decision Influenced by AI

The system influences:

- candidate shortlisting  
- resume ranking  
- automated rejection decisions

---

### Who Can Be Harmed?

Potentially affected groups include:

- female candidates  
- minority groups  
- candidates from women-dominated colleges  
- candidates with non-traditional backgrounds

---

### Misuse Scenarios

Possible risks include:

- over-reliance on automated scoring  
- automated rejection without human review  
- hidden proxy features for gender  
- feature importance amplifying historical bias

---

### Contextual Risk Factors

Risk may arise from:

- historically male-dominated hiring data  
- imbalanced training datasets  
- engineering-heavy hiring pipelines  
- lack of fairness validation during development

---

### Secondary Organizational Risks

- reputational damage  
- regulatory scrutiny  
- reduced workforce diversity  
- erosion of public trust

---

# 3️⃣ MEASURE — Detection Layer

Defines **metrics used to detect bias or harmful outcomes**.

Monitoring must be **continuous after deployment**.

---

## Key Monitoring Metrics

### Selection Rate by Gender

Selection Rate = Shortlisted Candidates / Total Applicants

Compare across demographic groups.

---

### Subgroup Performance Gap

Metric:

Female Selection Rate / Male Selection Rate

| Ratio | Interpretation |
|------|---------------|
| ≥ 0.90 | Acceptable |
| 0.80 – 0.89 | Monitor |
| < 0.80 | Escalation Trigger |

---

### False Negative Rate by Subgroup

False Negative Rate = Qualified Candidates Rejected / Total Qualified Candidates

Compare across demographic groups.

---

### Drift Monitoring

Track changes in system behavior over time:

- gender distribution among shortlisted candidates  
- feature importance changes

**Trigger Example**

If subgroup distribution shifts by **more than 10% from baseline**, initiate investigation.

---

### Human Override Frequency

Override Rate = AI Decisions Reversed / Total AI Decisions

Example threshold:

- if override rate exceeds **20% for two consecutive review cycles**, the model must be re-evaluated.

High override rates may indicate:

- model misalignment  
- hidden bias  
- data degradation

---

### Complaint Signals

Additional signals include:

- candidate complaints  
- HR internal audit findings  
- legal inquiries

All complaints should be logged in the **AI risk register**.

---

# 4️⃣ MANAGE — Response and Escalation

Defines **actions taken when governance thresholds are breached**.

---

### When Should the System Be Paused?

Automation should be paused if:

- subgroup selection ratio falls below threshold  
- drift monitoring thresholds are breached  
- legal complaints arise  
- override rate exceeds tolerance limits

---

### Escalation Chain

1. AI Governance Committee  
2. CHRO and Chief Risk Officer  
3. Legal & Compliance  
4. Executive Risk Committee

Clear ownership prevents governance ambiguity.

---

### Rollback Protocol

If bias or risk is detected:

1. disable automated rejection  
2. switch to human review  
3. conduct feature contribution analysis  
4. retrain model excluding biased proxies  
5. revalidate fairness metrics

---

### Incident Reporting

All incidents should follow structured reporting:

- incident logged in governance register  
- root cause analysis conducted  
- executive summary prepared  
- regulatory notification if required

---
# Key Governance Insight

The Amazon hiring system failure illustrates that **AI failures are often governance failures**.

Common causes include:

- lack of fairness thresholds  
- absence of monitoring controls  
- undefined escalation processes

The model behaved according to its training data.

The organization lacked **structured oversight mechanisms**.

----

# Governance Maturity Model

AI governance becomes operational when risk is translated into:

Intent → Metrics → Thresholds → Escalation → Documentation

Without measurable thresholds and accountability structures, governance remains theoretical.

-----
 ## Key Governance Takeaways

- AI failures are rarely algorithm failures — they are governance failures.
- Bias detection requires **predefined monitoring metrics and thresholds**.
- Responsible AI requires **continuous oversight**, not one-time validation.
- Clear escalation paths are essential when governance thresholds are breached.

  ---

## Governance Implementation Checklist

Before deploying a resume screening AI system, organizations should verify:

- [ ] Fairness metrics defined and validated
- [ ] Subgroup performance testing completed
- [ ] Human oversight defined
- [ ] Monitoring thresholds established
- [ ] Escalation procedures documented
- [ ] Incident reporting process established


---

# Note

This artifact is part of an effort to translate **AI governance principles into operational frameworks** for real-world ML systems.

The goal is to move beyond policy discussions and toward **practical governance architectures for trustworthy AI deployment**.

AI governance becomes operational when risk is translated into:

