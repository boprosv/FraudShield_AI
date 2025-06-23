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
![alt image](https://github.com/boprosv/FraudShield_AI/blob/main/Screenshot%202025-06-23%20104302.png?raw=true)

```text
 Customization & Real-Time Integration

FraudShield AI is built to be modular and extensible, allowing for easy adaptation to various financial environments and fraud detection use cases.

✅ Customization Highlights

Model Retraining: Use your own labeled dataset to retrain the XGBoost model via fraud_model.py

Feature Expansion: Add custom features like geolocation, device type, or transaction frequency

Threshold Tuning: Adjust fraud detection probability thresholds to match business risk levels

⚡ Real-Time Detection Use Case

FraudShield AI can be adapted for real-time monitoring by:

Deploying as a FastAPI microservice with prediction endpoints

Integrating with Kafka or serverless platforms (e.g., AWS Lambda)

Connecting to internal alerting tools for instant response on flagged transactions

The lightweight and fast inference capability of the XGBoost model makes it ideal for live production systems.
```

This project I used a cleaned and anonymized dataset from [Kaggle's Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud).
