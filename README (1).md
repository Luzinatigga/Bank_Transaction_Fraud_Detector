# 💳 Fraud Detection Project

This repository contains a machine learning project to detect fraudulent financial transactions.  
It includes both the **model analysis & training** (Jupyter Notebook) and a **Streamlit web application** for real-time fraud prediction.

---

## 📂 Project Structure

- `analysis_model.ipynb` → Jupyter Notebook used for:
  - Exploratory Data Analysis (EDA)
  - Data preprocessing and feature engineering
  - Model training and evaluation
  - Exporting the trained pipeline as `fraud_detection_pipeline.pkl`
- `fraud_detection.py` → Streamlit web app for predicting fraud on new transactions.
- `fraud_detection_pipeline.pkl` → Saved trained model pipeline (must be in the root folder).
- `requirements.txt` → Python dependencies for running the app.

---

## 🚀 Features

- **Data Analysis & Model Training** (in Jupyter Notebook)
  - Data cleaning and visualization
  - Feature selection and engineering
  - Machine learning pipeline for fraud detection
  - Model evaluation with metrics (e.g., accuracy, precision, recall)
- **Interactive Web App** with Streamlit:
  - Enter transaction details
  - Predict if a transaction is **Fraudulent** ⚠️ or **Legitimate** ✅
- **Pre-trained ML Model** for instant predictions

---

## 📦 Requirements

Install dependencies from `requirements.txt`:

```bash
pip install -r requirements.txt
```

Key packages used:
- `pandas`
- `joblib`
- `streamlit`
- `scikit-learn`
- `matplotlib` / `seaborn` (for visualizations in the notebook)

---

## ▶️ How to Run the App

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/fraud-detection.git
   cd fraud-detection
   ```

2. Make sure the model file `fraud_detection_pipeline.pkl` is in the same directory.

3. Run the Streamlit app:
   ```bash
   streamlit run fraud_detection.py
   ```

4. Open the URL in your browser (e.g., `http://localhost:8501`).

---

## 📊 Example Usage

- Select `Transaction Type`: `TRANSFER`  
- Enter `Amount`: `5000`  
- Provide balances (Sender & Receiver)  
- Click **Predict**

Output:
- ⚠️ **Fraudulent** if model detects fraud  
- ✅ **Legitimate** if safe  

---

## 📓 Notebook Highlights (`analysis_model.ipynb`)

- **EDA (Exploratory Data Analysis)**  
  - Visualized transaction amounts, types, and balance distributions.  
  - Identified fraud vs. non-fraud patterns.  

- **Preprocessing & Feature Engineering**  
  - Encoded categorical features (transaction type).  
  - Scaled numerical values.  

- **Model Training**  
  - Tested machine learning models (e.g., Logistic Regression, Random Forest).  
  - Trained a fraud detection pipeline.  

- **Evaluation**  
  - Measured accuracy, precision, recall, and F1-score.  
  - Chose the best model for deployment.  

- **Model Export**  
  - Saved trained pipeline as `fraud_detection_pipeline.pkl` for use in the Streamlit app.  

---

## 📄 License

This project is licensed under the MIT License.
