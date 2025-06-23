# FraudShield_AI
**FraudShield AI** is an intelligent fraud detection application that uses a trained XGBoost model, SHAP interpretability, and OpenAI-powered explanations to analyze financial transactions and flag suspicious activity. Designed for analysts, risk managers, and auditors, this tool provides both transparency and automation in fraud risk assessment.

```text
fraudshield_ai/
├── app.py                 # Streamlit frontend & fraud agent logic
├── fraud_model.py         # XGBoost training & Optuna tuning script
├── test_fraud_logic.py    # Optional: logic testing
├── data/
│   └── creditcard.csv     # Sample dataset (Kaggle credit card fraud)
├── models/
│   ├── fraud_model.pkl    # Trained XGBoost model
│   └── feature_names.pkl  # List of model input features
├── credentials.yml        # 🔐 OpenAI API key (exclude in version control)
├── config.toml            # Optional app config
├── requirements.txt       # Python dependencies
└── README.md              # Project overview
```

![alt image](https://raw.githubusercontent.com/boprosv/FraudShield_AI/8a77d13377036e184c241d463c7d94a60ef94566/Screenshot%202025-06-23%20104211.png)

```text
Features :

XGBoost + Optuna: Hyperparameter tuning for optimal fraud detection performance.

SHAP Explainability: Model transparency with top contributing features.

GPT-4 Agent: Fraud expert summaries in plain English for every flagged transaction.

Streamlit Interface: Clean and fast visual UI for business users.

Secure: API keys and local data are not exposed or shared.
```
![alt image](https://raw.githubusercontent.com/boprosv/FraudShield_AI/dd36721f9bbee9657ea48407f0bae41a4485245a/Screenshot%202025-06-23%20104243.png)
```text
How It Works:

User uploads a CSV file with transaction data.

The backend model calculates the probability of fraud.

Top flagged transactions are highlighted with a confidence score.

SHAP explains the reasoning behind each flag.

GPT-4 provides a natural language summary of why the transaction may be suspicious.
```
