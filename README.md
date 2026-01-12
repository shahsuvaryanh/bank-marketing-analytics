# bank-marketing-analytics

This project analyzes a bank marketing dataset to predict which clients are most likely to subscribe to a term deposit and to evaluate whether targeted outreach can improve campaign efficiency.

## Problem Statement
Bank marketing campaigns often contact all clients, which is costly and inefficient due to limited call-centre resources.  
The goal of this project is to identify high-probability clients using data analytics and reduce unnecessary calls while maintaining strong conversion rates.

## Dataset
- Bank Marketing Dataset (~11,000 clients)
- Features include demographic and financial attributes such as age, job, account balance, call duration, and previous contacts
- Target variable: **term deposit subscription (yes / no)**

## Approach
The analysis follows an end-to-end business analytics workflow:
- Data cleaning and feature engineering
- Exploratory data analysis (EDA)
- Predictive modeling using **Logistic Regression**
- Benchmark comparison with **K-Nearest Neighbors (KNN)**
- Customer segmentation using **K-Means clustering**
- Evaluation of a targeted calling strategy using **A/B testing and hypothesis testing**

## Key Results
- Logistic regression achieved **ROC-AUC ≈ 0.84** and **accuracy ≈ 76%**
- Call duration, account balance, and previous contacts were the strongest predictors of subscription
- A targeted calling strategy achieved **similar conversions with ~57% fewer calls**, significantly improving campaign efficiency

## Business Impact
The results demonstrate that data-driven targeting can:
- Reduce operational costs
- Improve marketing efficiency
- Prioritize high-value customer segments while avoiding over-targeting

## Repository Structure
├── analysis.py / Bank_project.ipynb # Main analysis and modeling
├── data/
│ └── bank.csv # Dataset
├── report/
│ └── Bank_Marketing_Analytics_Report.pdf
└── README.md


## How to Run
1. Install required dependencies:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
2. Run the analysis script:
python analysis.py
or open and run the notebook:
jupyter notebook Bank_project.ipynb
