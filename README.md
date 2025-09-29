[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/victorialovefranklin/YOUR_REPO/blob/main/NOTEBOOK_NAME.ipynb)



# CyberInfrastructure & Data Analysis for (COVID-19) Surveillance with Google Colab & Python

## About
This repository contains a series of **hands-on labs** designed to teach secure data handling, analysis, and visualization techniques for **wastewater viral RNA biosurveillance**.  

## Introduction
The labs use real-world data from:
- **CDC NWSS** – Wastewater viral activity level (WVAL) of SARS-CoV-2 viral RNA trends  
- **WastewaterSCAN** – SARS-CoV-2 variant and gene-level detections  
- **CDC COVID-NET** – Clinical case and hospitalization data  

The sequence is designed to build progressively:
1. **Secure data handling**  
2. **Data cleaning and exploratory analysis**  
3. **Machine learning and anomaly detection**  
4. **Interactive dashboards and GIS mapping**  
5. **Bioinformatics and AI-driven applications**  

Together, these labs provide a complete workflow for understanding how biosurveillance data can be collected, processed, modeled, and translated into insights.

---

## Lab Sequence 

### Phase 1 — Foundations
1. **Lab 1: Secure Storage & Access Control**  
   - **Deliverable:** Secure Google Drive folder, Activity log screenshot.  
   - **Focus:** Least privilege, restricted links, audit trail.  

2. **Lab 2: Retrieval in Colab**  
   - **Deliverable:** Colab notebook that mounts Drive and loads the 3 CSVs, quick data check.  

---

### Phase 2 — Data Cleaning & EDA
3. **Lab 3: Process & Clean Data**  
   - Deliverable: Cleaned CSV(s) + code (handle missing values, types, outliers, standardization).  

4. **Lab 4: EDA & Statistics**  
   - Deliverable: Colab notebook with summary stats (mean, std, min/max), correlation heatmap, notes.  
   - Concepts: correlation, lag-correlation (intro), distributions.  

---

### Phase 3 — Time Series & Forecasts
5. **Lab 5: Time Series Analysis**  
   - Deliverable: Time series plots, ACF/PACF, STL decomposition, lag correlation (wastewater → hospitalizations).  

6. **Lab 6: Predictive Modeling (Classical)**  
   - Deliverable: Baseline models (linear regression, ARIMA, Prophet) with MAE/RMSE and commentary.  
   - Concepts: train/validation split, gradient descent (intuition), hyperparameters (basic).  

---

### Phase 4 — ML & Anomaly Detection
7. **Lab 7: Supervised ML**  
   - Deliverable: Random Forest / Gradient Boosting comparison, simple tuning, feature importance.  
   - Concepts: hyperparameters, cross-validation.  

8. **Lab 8: Anomaly Detection**  
   - Deliverable: Isolation Forest results + flagged dates; optional Markov-chain event-state toy model.  
   - Concepts: anomaly scores, thresholds; AT/DT/RT (attack time, detection time, response time).  

---

### Phase 5 — Visualization Apps & GIS
9. **Lab 9: Streamlit Dashboard**  
   - Goal: Build an interactive dashboard for time series & anomaly analysis.  
   - Deliverable: `streamlit_app.py` with controls (date range, site filter), charts (rolling mean, anomalies), and KPIs.  
   - Suggested libs: `streamlit`, `pandas`, `matplotlib` or `plotly`.  
   - Run:  
     ```bash
     streamlit run streamlit_app.py
     ```  
     or deploy on Streamlit Community Cloud.  
   - Privacy: Use only de-identified, aggregate CSVs.  

10. **Lab 10: GIS Mapping**  
   - Goal: Map Tennessee wastewater sites and trends.  
   - Deliverable: Interactive map (`map.html`) with sites colored by recent viral load/trends.  
   - Suggested libs: `geopandas`, `folium`, `shapely` (or `keplergl`).  
   - Artifacts: export `map.html`, link from README or embed in Streamlit.  

---

### Phase 6 — Data Management & Bioinformatics
11. **Lab 11: Database (MySQL)**  
   - Deliverable: SQL schema for sites, measurements, variants; ETL script to load cleaned data; sample queries.  

12. **Lab 12: Bioinformatics Sources & Gene Markers**  
   - Deliverable: Notebook showing how GISAID sequence/lineage data and PDB structures contextualize wastewater trends.  
   - Tasks: simple gene-marker detection (regex/ID mapping), variant visualization.  
   - ⚠️ Note: Respect GISAID terms; do not redistribute restricted data.  

---

### Phase 7 — Advanced AI/ML
13. **Lab 13: Autoencoder Feature Extraction**  
   - Deliverable: Autoencoder trained on multivariate time series; reconstruction error vs Isolation Forest anomalies.  

14. **Lab 14: Generative AI & RAG for Context**  
   - Deliverable: RAG demo on local docs (methodology notes, metadata, logs).  
   - Concepts: chunking, embeddings, retrieval, guardrails; contextualizing logs with citations.  

---

## 🔧 Where Your “Other” Concepts Fit
- **Heatmap** → Lab 4 (EDA correlations)  
- **Correlation & Lag correlation** → Labs 4–5  
- **AT/RT/DT metrics** → Lab 8 (Anomaly Detection)  
- **Markov Chains** → Lab 8 (State transitions for outbreaks)  
- **Isolation Trees** → Lab 8 (Isolation Forest)  
- **Gradient Descent & Hyperparameters** → Labs 6–7  
- **Non-deterministic behavior (stochasticity)** → Labs 5–8  
- **Contextualize logs** → Lab 14 (RAG/GenAI)  
- **Averages / Standard Deviation** → Labs 3–4  
- **LFO/MFO (frequency analysis)** → Lab 5 (spectral/seasonal trends)  

---

## 🎯 Minimal Deliverables per Lab
- Notebook or script with results & a short reflection  
- Artifacts (plots, `map.html`, `streamlit_app.py`, SQL schema, etc.)  
- Update this `README.md` with links/screenshots for your outputs  

---

## ✍️ Author
**Victoria Love Franklin**  
PhD Researcher | Data Science & Biomedical Applications  

📅 **Last Updated:** February 2025
