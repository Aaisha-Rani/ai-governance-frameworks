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

  ## Example: Applying the Checklist (Amazon Hiring AI)

| Question | Answer |
|--------|--------|
| Is training data biased? | Yes |
| Is model explainable? | No |
| Is there human oversight? | No |
| Can the system be unfair? | Yes |

### Key Insights

- The system learned bias from historical data  
- Lack of proper checks increased risk  
- The system had a high impact on hiring decisions  

**Final Risk Level: HIGH**

## Final Note

This is an initial version of a simple AI risk checklist.

The aim is to make AI governance more practical and accessible by turning ideas into usable tools.

This will be further refined and expanded.
