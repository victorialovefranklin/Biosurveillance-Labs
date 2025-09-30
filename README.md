# CyberInfrastructure & Data Analysis for COVID-19 Surveillance  
*with Google Colab & Python*  

## About  
This repository contains a series of **hands-on labs** focused on secure data handling, analysis, and visualization for **wastewater viral RNA biosurveillance**.  

- **Clean data**: Use clean datasets for baseline forecasting and trend modeling.
- **Outlier data**: Use outlier datasets for anomaly-driven biosurveillance: early outbreak detection, rare-event tracking, and policy evaluation.
Together, these approaches provide a **full picture** of public health: long-term baselines and short-term anomaly detection.  

---

## Introduction  
The labs make use of real-world datasets:  
- **CDC NWSS** — Wastewater Viral Activity Levels (WVAL) of SARS-CoV-2  
- **WastewaterSCAN** — Variant and gene-level detections of SARS-CoV-2  
- **CDC COVID-NET** — Clinical cases and hospitalization records  

**The sequence builds progressively:**  
1. GitHub setup & Colab integration  
2. Secure data handling & access control  
3. Data preprocessing & outlier detection  
4. Trend analysis using cleaned data  
5. Anomaly/event-driven biosurveillance using outlier data  

---

## Lab Sequence  

### Phase 1 — Foundations  
1. **Lab 1: GitHub Setup & Repository Forking**  
   - *Deliverable:* GitHub account + repository linked to Colab  
   - *Focus:* Version control & reproducible workflows  

2. **Lab 2: Secure Storage & Access Control**  
   - *Deliverable:* Secure Google Drive folder + activity log screenshot  
   - *Focus:* Principles of least privilege, restricted access, and audit trails  

---

### Phase 2 — Data Cleaning & Exploratory Analysis  
3. **Lab 3: Process & Clean Data**  
   - *Deliverable:* Cleaned CSV files + preprocessing code (handle missing values, types, outliers, standardization)  

4. **Trend Analysis (Clean Data)**  
   - *Goal:* Identify baseline shifts, seasonal trends, and long-term epidemiological patterns  

5. **Outlier & Anomaly Detection (Outlier Data)**  
   - *Goal:* Detect rare events, spikes, and unusual signals to support outbreak forecasting and public health interventions  

---

## Author  
**Victoria Love Franklin**  
Ph.D. Pre-Candidate in Data Science | Research Focus: Biomedical Applications & Biosurveillance  

📅 **Last Updated:** September 29, 2025  

---

## 📂 Repository Structure  
```bash
├── Lab1_Intro.ipynb                 # GitHub & Colab setup
├── Lab2_Secure_Storage.ipynb        # Secure storage & access control
├── Lab3_Process_Clean_Outliers.ipynb # Data preprocessing & outlier detection
├── data/                            # Example raw data files
├── results/
