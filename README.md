  # COVID-19 Biosurveillance: Machine Learning, Outlier Dynamics, Gene Marker Visualization & Policy Insights
*with Google Colab & Python*  

Integrating wastewater, genomic, and clinical surveillance data to detect anomalies, forecast trends, and guide vaccination and policy strategies for COVID-19.
---

## About  
This repository contains a series of **hands-on labs** demonstrating secure data handling, analysis, and visualization workflows for **COVID-19 biosurveillance**.  

It integrates:  
- **Wastewater viral RNA** → biosurveillance for early outbreak detection  
- **Clinical hospitalization data** → burden & age-risk analysis  
- **Genomic markers** → SARS-CoV-2 gene targets and **3D protein visualization** from the PDB database  
- **Machine learning models** → trend forecasting, anomaly detection, and risk classification  

**Approach:**  
- **Clean datasets** → establish baselines, trends, and forecasts  
- **Outlier datasets** → study rare, extreme, or early-warning events  
- **Gene-level analysis** → visualize spike proteins and vaccine target sites  
- **Clinical burden analysis** → determine which age groups are most at risk and guide vaccination priorities  

---

## Introduction  
**Datasets used:**  
- **CDC NWSS** — Wastewater Viral Activity Levels (WVAL) of SARS-CoV-2  
- **WastewaterSCAN** — Variant and gene marker detections (S, N, ORF1ab, Spike proteins)  
- **CDC COVID-NET** — Clinical cases and hospitalizations, stratified by age groups  

**Integrated workflows allow you to:**  
- Detect **outliers & anomalies** in biosurveillance data  
- Benchmark forecasting models (ARIMA, Random Forest, XGBoost)  
- Visualize **spike proteins in 3D** (via PDB database + py3Dmol)  
- Analyze **age-based clinical burden** to identify **priority groups for vaccination**  

---

## Lab Sequence  

### Phase 1 — Foundations  
**Lab 1: GitHub Setup & Repository Forking**  
- Deliverable: GitHub repo linked to Colab  
- Focus: Version control & reproducible workflows  

**Lab 2: Secure Storage & Access Control**  
- Deliverable: Secure Google Drive folder + activity log  
- Focus: Restricted access, least privilege, audit trail  

---

### Phase 2 — Data Preprocessing & Outlier Detection  
**Lab 3: Process & Clean Data**  
- Deliverable: Cleaned CSV files (handle missing values, types, outliers, standardization)  
- Focus: Prepare datasets for modeling  

**Lab 4: Model Benchmarking**  
- Models: ARIMA (SARIMAX), Random Forest, XGBoost  
- Validation: Walk-forward (expanding window)  
- Metrics: RMSE, MAE, R²  
- Deliverable: Comparison tables + visualizations  

---

### Phase 3 — Outlier Dynamics & Rare-Event Modeling  
**Lab 5: Outlier Dynamics with Markov Chains**  
- Normal ↔ Outlier state transitions  
- Persistence analysis & transition matrices  
- Lead/lag analysis: wastewater → clinical  

**Lab 6: Gene Marker Detection & Protein Visualization**  
- Detect SARS-CoV-2 gene markers (S, N, ORF1ab, Spike)  
- Visualize **Spike protein (PDB: 6VSB)** in **3D** using py3Dmol  
- Map **target points relevant for vaccine binding**  

---

### Phase 4 — Epidemiological & Policy Analysis  
**Lab 7: Age-Risk and Vaccination Prioritization**  
- Analyze clinical cases by age group  
- Identify which groups show the highest burden (hospitalizations/ER visits)  
- Recommend vaccination focus based on **burden analysis**  

**Lab 8: Advanced Epidemiology & Policy**  
- Burden Analysis: Outlier vs. baseline weeks  
- Disparities: Link outliers with SDOH/EJScreen  
- Policy Impact: Spikes linked to interventions (mask mandates, vaccine campaigns, emissions testing termination)  
- Seasonality: Outlier clustering by season  

---

## Author  
**Victoria Love Franklin**  
*Ph.D. Pre-Candidate in Data Science | Research Focus: Biomedical Applications, Biosurveillance, Genomics & Policy Analysis*  

**Last Updated:** September 30, 2025  

---

## Repository Structure  
```bash
├── Lab1_Intro.ipynb                     # GitHub setup
├── Lab2_Secure_Storage.ipynb            # Secure storage
├── Lab3_Process_Clean_Outliers.ipynb    # Preprocessing & outlier detection
├── Lab4_Model_Benchmarking.ipynb        # ARIMA, RF, XGBoost
├── Lab5_Markov_Outlier_Transitions.ipynb # Outlier dynamics & Markov chains
├── Lab6_GeneMarkers_AgeRisk.ipynb       # Gene marker detection & 3D spike visualization
├── Lab7_AgeRisk_BurdenVaccination.ipynb # Age risk analysis & vaccine targeting
├── Lab8_Policy_Analysis.ipynb           # Epidemiological & policy insights
├── data/                                # Input datasets
├── results/                             # Outputs (figures, tables, exports)

# Highlight:
This updated workflow now links genomic insights (PDB + WastewaterSCAN) with clinical burden analysis to deliver actionable vaccination strategies while also supporting forecasting and anomaly detection for COVID-19 biosurveillance.
