<!-- readme-refresh 2026-11 -->
<div align="center">

# 🔍 Customer Churn with Explainable AI

**Predicts who will churn, explains why and suggests what to do**

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" /> <img src="https://img.shields.io/badge/XGBoost-189FDD?style=for-the-badge" alt="XGBoost" /> <img src="https://img.shields.io/badge/SHAP-0B1628?style=for-the-badge" alt="SHAP" /> <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" alt="scikit-learn" /> <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />

</div>

## ✨ Highlights

- XGBoost scores each customer's churn risk
- SHAP TreeExplainer finds each customer's reasons
- Reasons become plain-language retention actions
- [Live demo](https://customer-churn-explanation.streamlit.app/)

<!-- body -->
## 🚀 Overview
This project predicts customer churn using machine learning and explains predictions using SHAP. It goes beyond prediction by providing **human-readable reasons and actionable business suggestions** to reduce churn.

---

## 🎯 Problem Statement
Telecom companies face high customer churn, leading to revenue loss. Traditional ML models predict churn but fail to explain:
- Why a customer is likely to churn
- What actions can prevent churn

---

## 💡 Solution
Built an **Explainable + Actionable AI system** that:
- Predicts churn using XGBoost
- Explains predictions using SHAP
- Converts explanations into **human-readable insights**
- Provides **business recommendations to reduce churn**
- Deploys via interactive Streamlit dashboard

---

## 📊 Dataset
- Source: Kaggle Telco Customer Churn Dataset
- Rows: ~7,000 customers
- Features:
  - Demographics (gender, senior citizen)
  - Account info (tenure, contract)
  - Services (internet, security, support)
  - Billing (charges, payment method)
- Target: `Churn (Yes/No)`

---

## 🧠 Model & Explainability
- Model: XGBoost Classifier
- Explainability: SHAP (TreeExplainer)
- Outputs:
  - Global feature importance
  - Local explanations per customer
  - Natural language reasoning
  - Actionable suggestions

---

## 📈 Project Metrics
- Accuracy: ~80–85%
- ROC-AUC: ~0.85+
- Handles class imbalance via stratified split
- Real-time inference with explanations

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- SHAP
- Streamlit
- Matplotlib

---

## 📁 Folder Structure
customer-churn-xai/
│
├── data/
│ ├── raw/
│ └── processed/
│
├── src/
│ ├── data/
│ ├── models/
│ ├── explainability/
│ └── utils/
│
├── models/
│ ├── churn_model.pkl
│ └── feature_columns.pkl
│
├── reports/
│ └── shap_outputs/
│
├── app.py
├── main.py
└── requirements.txt

---

## ⚙️ System Architecture
1. Data Ingestion → Load raw dataset  
2. Preprocessing → Clean + encode features  
3. Model Training → XGBoost classifier  
4. Explainability → SHAP values generation  
5. Interpretation Layer → Convert SHAP → human insights  
6. UI Layer → Streamlit dashboard  

---

## 🤖 Why This Tech Stack
- XGBoost → best for tabular data  
- SHAP → industry-standard explainability  
- Streamlit → fast deployment  
- Sklearn → reliable preprocessing pipeline  

---

## 🔥 Key Features
- Predict churn probability
- Explain predictions (why)
- Suggest actions (what to do)
- Interactive UI
- Per-customer analysis

---

## 🚀 Future Improvements
- Batch prediction via CSV upload
- Real-time API (FastAPI)
- Deployment (Docker / Cloud)
- Advanced recommendation engine
- What-if simulation dashboard

---

## 💪 Why This Project is Strong
- Combines ML + Explainability + Business impact
- Moves beyond prediction → decision-making
- Production-ready architecture
- Real-world use case (telecom churn)
- Demonstrates end-to-end ML pipeline

---

## ▶️ Run Project
```bash
pip install -r requirements.txt
python main.py
streamlit run app.py

---

<div align="center"><sub>Built by <a href="https://github.com/Mokshitsharma">Mokshit Sharma</a> · <a href="https://mokshitsharma27.vercel.app/">Portfolio</a> · <a href="https://www.linkedin.com/in/mokshit-sharma-75b5ab305">LinkedIn</a></sub></div>
