# ML-Driven Emergency Department Triage & Resource Allocation System

## Overview
This project presents a **machine learning–driven triage system** integrated with a **simulation-based resource allocation model** for Emergency Departments (EDs).  

It predicts patient severity and optimizes hospital resource allocation using scheduling and queueing strategies.

---

## Objectives
- Predict Emergency Severity Index (ESI) using ML models  
- Design a **priority-based scheduling algorithm**  
- Simulate patient flow under constrained hospital resources  
- Minimize waiting time and improve ICU utilization  

---

##  Methodology

### 1. Machine Learning Models
- Logistic Regression  
- Random Forest  
- XGBoost (best performing)

### 2. Feature Engineering
- Shock Index  
- Oxygen Risk  
- Composite Criticality Score  
- Vital sign-based features  

### 3. Evaluation Metrics
- Accuracy: **81.1% (XGBoost)**  
- Mean Absolute Error (MAE): **0.189**  
- Validation using **permutation importance**  
- Data leakage checks  

---

## Scheduling Algorithm

A hybrid scheduling approach combining:

- **Severity-based prioritization**
- **Logarithmic aging** (to prevent starvation)
- **Weighted Shortest Processing Time (WSPT)**

 This ensures:
- Fairness  
- Efficiency  
- Reduced waiting time  

---

## Simulation Model

A **discrete-time simulation** was developed to model:

- Patient arrivals  
- Queue formation  
- Resource constraints (beds, ICU, staff)  

### Results:
-  Waiting time reduced by ~47%  
-  Critical waiting time reduced by ~78%  
-  ICU utilization increased by ~81%  

---

##  Files
- `notebooks/main.ipynb` → Full implementation  
- `scheduling_logic.pdf` → Entire pdf explaining the scheduling logic 
---
