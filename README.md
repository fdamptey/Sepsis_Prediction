# 🧠 Predicting Sepsis Onset: A Machine Learning-Based Early Warning System

## 📘 Overview

Sepsis is a life threatening clinical emergency with high mortality rate. Early detection of sepsis is critical for improving survival rates, reducing ICU stays, and enabling timely interventions. But currently, there are not sufficiently effective tools for predicting this medical emergency early enough to reduce the high mortality rate. This project, developed by five graduate students at Michigan Technological University, aims to build a machine learning-based early warning system to predict the onset of sepsis in ICU patients before clinical diagnosis. 

The system leverages clinical data from the **PhysioNet 2019 Prediction of Sepsis dataset**, applying models such as Random Forest, XGBoost and Logistic Regression. After thorough preprocessing and feature selection, the **Random Forest model** emerged as the most effective, with an accuracy of **84%** and an AUC of **0.916**. The model's performance is a promising prospect towards developing a clinical tool that is effective at predicting Sepsis early enough to reduvce mortality.


## 🧑‍💻 Team Members
- Uttam Bellamkonda
- Easton Hans
- Sucharitha Reddy
- Fredrick Damptey
- Suhani Yalaga 


## 📂 Repository Structure

├── data/                         # Scripts or references related to dataset access
├── notebooks/                    # Colab notebooks for EDA, preprocessing, training
├── models/                       # Saved models or training scripts
├── utils/                        # Helper functions (preprocessing, metrics, etc.)
├── results/                      # ROC curves, confusion matrices, and visualizations
├── proposal.pdf                  # Project proposal document
├── ML_Project_Report_Paper.pdf   # Final report of the project
├── requirements.txt              # Python dependencies
└── README.md                     # This file


## 🧪 Methods Used

- Models: Logistic Regression, XGBoost, Random Forest  
- Feature Selection: 'SelectKBest' (top 17 features)  
- Imputation: Median-based  
- Resampling: 'RandomUnderSampler' (to address class imbalance)  
- Evaluation: Accuracy, Precision, Recall, F1-score, AUC  
- Validation: 5-fold Stratified Cross-Validation  


## 🏥 Dataset

- **Source**: [PhysioNet 2019 Challenge](https://physionet.org/content/challenge-2019/)
- **Samples**: >1.5 million hourly records from ~40,000 ICU stays  
- **Features**: 42 clinical variables (vital signs and lab values)  
- **Target**: 'SepsisLabel' (0 = no sepsis, 1 = sepsis onset)

---

## 🚀 Results

| Metric     | Random Forest |
|------------|---------------|
| Accuracy   | 84%           |
| Precision  | 0.84          |
| Recall     | 0.84          |
| F1-score   | 0.84          |
| AUC        | 0.916         |


## 🔍 Future Directions
- Further feature exploration and modelling with retuned hyperparameters to improve model performance
- Incorporate time-series modeling
- Integrate unstructured clinical notes using NLP
- Integrate more interpretable AI


## 📦 Installation

```bash
git clone https://github.com/your-username/sepsis-prediction-ml.git
cd sepsis-prediction-ml
pip install -r requirements.txt
```
