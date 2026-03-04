AI Governance Artifact
Resume Screening Model (Case Study Inspired by Amazon Hiring System)
1. Purpose

This document outlines a governance control framework for an AI-based resume screening system used to shortlist job candidates.

The objective is to demonstrate how AI risk can be governed using structured ownership, risk discovery, measurement, and response mechanisms.

This artifact is inspired by lessons learned from the Amazon hiring case, where bias emerged due to historical training data.

Governance Control Framework

The framework follows four governance layers:

Govern (Ownership & Accountability)

Map (Risk Discovery)

Measure (Monitoring & Detection)

Manage (Response & Escalation)

1️⃣ GOVERN — Ownership Layer
Who Approves AI Use?

Chief Human Resources Officer (CHRO)

Chief Risk Officer (CRO)

AI Governance Committee

(Board oversight for high-risk deployments.)

Who Defines Acceptable Risk?

Executive Risk Committee, including:

HR leadership

Legal

Compliance

AI/ML leadership

Risk Management

They define:

Acceptable fairness thresholds

Bias tolerance levels

Monitoring requirements

Who Signs Off Before Deployment?

AI Governance Committee:

Data Science Lead

HR Lead

Legal Representative

Risk Officer

Ethics/Compliance Representative

Deployment approval requires:

Fairness validation

Subgroup performance testing

Documentation of residual risk

Policies Required

Equal Opportunity Hiring Policy

Bias & Fairness Testing Policy

Mandatory Subgroup Evaluation Policy

Human-in-the-loop Requirement

AI Monitoring & Incident Escalation Policy

Governance is not intent-based — it is documented and enforceable.

2️⃣ MAP — Risk Discovery Layer
Decision Influenced by AI

Candidate shortlisting

Ranking of resumes

Automated rejection decisions

Who Can Be Harmed?

Female candidates

Minority groups

Candidates from women-dominated colleges

Non-traditional background applicants

Misuse Scenarios

Over-reliance on automated scoring

Fully automated rejection without review

Hidden proxy features for gender

Feature importance unintentionally amplifying bias

Contextual Risk Factors

Historical male-dominated workforce

Imbalanced training data

Engineering-heavy hiring patterns

Lack of fairness review before deployment

Secondary Risks

Reputational damage

Regulatory action

Talent pool reduction

Public trust erosion

3️⃣ MEASURE — Detection Layer

This layer translates principles into operational metrics.

Key Monitoring Metrics
1. Selection Rate by Gender

Percentage of candidates shortlisted by subgroup.

2. Subgroup Performance Gap

Selection Rate Ratio:

Female Selection Rate / Male Selection Rate

Thresholds:

≥ 0.90 → Green

0.80–0.89 → Monitor

< 0.80 → Escalation Trigger

(Aligned conceptually with adverse impact principles used in employment contexts.)

3. False Negative Rate by Subgroup

Percentage of qualified candidates incorrectly rejected per subgroup.

4. Drift Threshold Monitoring

Monitor:

Gender distribution of shortlisted candidates over time

Feature importance shifts

Trigger:

If subgroup distribution shifts > 10% from baseline → investigation required.

5. Human Override Frequency

Definition:
Percentage of AI decisions reversed by human recruiters.

Threshold:

If override rate > 20% for two consecutive review cycles → re-evaluation required.

High override rates may indicate:

Model misalignment

Hidden bias

Data degradation

6. Complaint Signals

Candidate complaints

HR internal audit findings

Legal inquiries

Complaints are logged in risk register and reviewed quarterly.

4️⃣ MANAGE — Response & Escalation Layer

Governance requires predefined response protocols.

When Do We Pause the System?

Pause or restrict automation if:

Subgroup ratio < 0.80

Drift threshold breached

Legal complaint filed

Override rate exceeds tolerance

Escalation Chain

AI Governance Committee

CHRO + Chief Risk Officer

Legal & Compliance

Executive Risk Committee (if severe)

Clear ownership prevents ambiguity.

Rollback Protocol

Disable automated rejection

Switch to human review

Conduct feature contribution analysis

Retrain model excluding biased proxies

Revalidate fairness metrics before redeployment

Incident Reporting Process

Incident logged in governance register

Root cause analysis conducted

Executive summary submitted

Regulatory disclosure if required

Post-incident policy review

Key Governance Insight

The failure in the Amazon hiring system was not solely algorithmic.

It was a governance failure characterized by:

Lack of predefined fairness thresholds

Absence of monitoring triggers

No structured escalation framework

The model behaved according to its training data.
The organization lacked structured oversight.

Governance Maturity Model (Learning Outcome)

AI governance becomes operational when risk is translated into:

Intent → Metrics → Thresholds → Escalation → Documentation

Without thresholds, governance remains theoretical.

With structured control loops, governance becomes enforceable.

Author Note
This artifact is part of a broader effort to operationalize AI governance in enterprise ML systems.

The goal is to design governance as a continuous control loop — not a one-time compliance exercise.

This artifact is part of a broader effort to operationalize AI governance in enterprise ML systems.

The goal is to design governance as a continuous control loop — not a one-time compliance exercise.
