# FraudShield_AI
**FraudShield AI** is an intelligent fraud detection application that uses a trained XGBoost model, SHAP interpretability, and OpenAI-powered explanations to analyze financial transactions and flag suspicious activity. Designed for analysts, risk managers, and auditors, this tool provides both transparency and automation in fraud risk assessment.


fraudshield_ai/
├── app.py # Streamlit frontend & fraud agent logic
├── fraud_model.py # XGBoost training & Optuna tuning script
├── test_fraud_logic.py # Optional: logic testing
├── data/
│ └── creditcard.csv # Sample dataset (Kaggle credit card fraud)
├── models/
│ ├── fraud_model.pkl # Trained XGBoost model
│ └── feature_names.pkl # List of model input features
├── credentials.yml # 🔐 OpenAI API key (exclude in version control)
├── config.toml # Optional app config
├── requirements.txt # Python dependencies
└── README.md # Project overview

![alt image]()
