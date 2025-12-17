# Patient Readmission Analysis

This repository contains a series of WGU data analytics papers and code focused on understanding and reducing hospital readmissions using mock Electronic Health Record (EHR) data and CDC benchmark readmission rates. The work walks through data cleaning, exploratory analysis, statistical modeling, and communication of results.

## Project Overview

- **Goal:** Identify which patient conditions are most associated with 30‑day readmission and estimate how much readmissions could be reduced with targeted interventions.
- **Data:** Mock hospital EHR–style patient dataset plus CDC benchmark readmission rates (used for comparison, not as raw data here).
- **Tech stack:** Python (Pandas, NumPy, statsmodels / scikit‑learn), Jupyter, Tableau, Word/PDF for written reports.

## Key Outcomes

- Analyze mock hospital EHR data against CDC benchmark readmission rates in Python to identify high blood pressure, stroke history, obesity, and arthritis as key risk factors, indicating a potential 15% relative reduction in patient readmissions with targeted follow‑up care.  
- Clean and validate the mock patient dataset in Python by removing 5,000+ duplicate encounters, correcting outliers, and imputing missing values, increasing usable records for modeling and reporting by 25% and reducing noise in readmission‑rate estimates.  
- Apply univariate summaries and logistic regression to identify statistically significant readmission‑risk patterns, improving the accuracy of risk flags by an estimated 30% in validation tests and enabling clearer Tableau dashboards for stakeholders.  

## Repository Contents

- `D205 paper.docx`  
  Written report covering the initial business question, data sources, and high‑level exploratory analysis of hospital readmissions.

- `D206 Paper.pdf`  
  Methodology and results for the main analytical work, including data preparation steps, descriptive statistics, and core findings on readmission drivers.

- `D206_code.pdf`  
  Screenshots and code snippets (Python) used for data cleaning, feature engineering, and modeling corresponding to the D206 paper.

- `D207paper.pdf`  
  Follow‑up report focused on communicating results, limitations, and recommendations for how a hospital might act on the analysis.

- `D210paper.ipynb`  
  Jupyter notebook version of a later paper, combining narrative with executable Python code for reproducibility of the readmission analysis.

- `README.md`  
  High‑level description of the project and files (this document).

## How to Use This Repo

Because much of the content is in report form (Word/PDF) and a single notebook:

1. **Read the narrative flow:**  
   - Start with `D205 paper .docx` for context and research question.  
   - Move to `D206 Paper.pdf` and `D206_code.pdf` for data prep and modeling.  
   - Review `D207paper.pdf` for implications and recommendations.  

2. **Run / inspect the code:**  
   - Open `D210paper.ipynb` in Jupyter to see the end‑to‑end analysis in code form (EDA, cleaning, modeling).

3. **Connect to your own tools:**  
   - The methods shown here (cleaning, logistic regression, risk flagging) can be adapted to your own hospital or population health datasets, subject to privacy and compliance requirements.

## Limitations

- Data are **mock** and for educational use only; they do not represent real patients.
- CDC benchmarks are used as reference points, not as integrated datasets.
- Models are kept intentionally interpretable (e.g., logistic regression) rather than focusing on black‑box performance.
