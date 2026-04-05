# AI Risk Checklist – Hiring System (Case Study: Amazon Hiring AI)

## Overview

This checklist is a simple attempt to evaluate risks in AI systems using a real-world case (Amazon hiring AI).

The goal is to move from understanding problems to creating a practical way to assess them.

This checklist focuses on identifying risks related to data, model behavior, system usage, and overall impact.

## 1. Data Risks

- Is the training data missing any important groups of people?  
- Does the data include diverse genders, backgrounds, and age groups?  
- Is there a risk that past bias is present in the data?  
- Is sensitive data (like gender or name) handled appropriately?  
- Do we know where the data comes from?  
- Is the data reviewed or updated regularly?

 ## 2. Model Risks

- Does the model make consistent decisions for similar candidates?  
- Can we understand why the model selected or rejected a candidate?  
- Has the model been tested on different types of candidates?  
- Are there signs that the model behaves unfairly for certain groups?  
- Can the model be corrected or improved if issues are found?  
- Is the model’s performance measured using clear metrics?

  ## 3. System Usage Risks

- Is there a human reviewing or validating AI decisions?  
- Can candidates appeal or request feedback on decisions?  
- Is the system monitored regularly after deployment?  
- Is there a process to handle errors or failures in the system?  
- Is there a clear owner responsible for this AI system?  
- Are users informed that AI is being used in decision-making?

## 4. Risk & Impact

- Can this system unfairly reject qualified candidates?  
- Could this system negatively impact certain groups of people?  
- Is this system being used in a high-stakes decision (like hiring)?  
- Are the most critical risks identified and prioritized?

  ## 5. Risk Scoring

Each question can be answered as:

- Yes = 0 (Low risk)  
- Not Sure = 1 (Uncertain / potential risk)  
- No = 2 (High risk)  

*Note: Questions are framed in a positive form (e.g., “Is the system fair?”)  
so that “Yes” indicates low risk and “No” indicates higher risk.*

### How to use:
- Answer all questions  
- Add up the total score  

### Risk Levels (for full checklist)

- 0–10 → Low Risk  
- 11–25 → Medium Risk  
- 26+ → High Risk  

*Note: These ranges apply when all checklist questions are used.  
For partial examples, risk interpretation should consider context.*


  

## Example: Applying the Checklist (Amazon Hiring AI)

| Section | Question | Answer | Score |
|--------|----------|--------|-------|
| Data | Is the training data free from bias? | No | 2 |
| Data | Does the data include diverse groups of candidates? | No | 2 |
| Model | Can the model’s decisions be clearly explained? | No | 2 |
| Model | Does the model behave fairly across different groups? | No | 2 |
| Usage | Is there human oversight in decision-making? | No | 2 |
| Usage | Is the system monitored regularly after deployment? | No | 2 |
| Risk & Impact | Is the system safe to use in high-stakes decisions like hiring? | No | 2 |
| Risk & Impact | Are critical risks identified and addressed? | No | 2 |

### Total Score

16 out of 16 (sample subset of questions)

### Final Risk Level

High Risk

### Key Insights

- The system relied on biased historical data  
- Lack of transparency made decisions hard to explain  
- No human oversight increased the risk of unfair outcomes  
- High-impact usage (hiring) amplified the consequences  


## Final Note

This is an initial version of a simple AI risk checklist.

The aim is to make AI governance more practical and accessible by turning ideas into usable tools.

This will be further refined and expanded.
