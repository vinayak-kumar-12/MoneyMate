# 🧠 MoneyMate 2.0 AI Insights (SMS Analysis)

> **Natural Language Processing for Personal Finance.**  
> A Flask-based microservice that uses machine learning to transform messy SMS text into structured financial transactions and meaningful alerts.

---

## 🚀 Key Functions

- **Automated Extraction**: Pulls amount, merchant name, and transaction type (Debit/Credit) from raw SMS.
- **ML Classification**: Uses a trained **TF-IDF + Scikit-learn** model to categorize messages.
- **Contextual Anomaly Detection**: Calculates Z-Scores and variance relative to historical spending to flag unusual activity.
- **Financial Mapping**: Intelligently identifies merchants even from vague SMS strings using priority regex patterns.

---

## 🛠️ Tech Stack

- **Framework**: Flask (Python)
- **ML Libraries**: Scikit-learn, Pickle
- **Processing**: Regular Expressions (RE), Math (Statistical Anomaly Detection)
- **CORS**: Flask-CORS for secure cross-origin mobile app communication.

---

## 📡 API Reference

### `POST /analyze-sms`
Analyzes a single SMS string for basic transaction details.

### `POST /analyze-contextual`
Performs deep analysis including anomaly detection by comparing a new SMS against a historical transaction array.

### `POST /analyze-batch`
Efficiently processes an array of messages (used during manual sync).

---

## 🏃 Getting Started

1. **Install Dependencies**:
   ```bash
   pip install flask flask-cors scikit-learn pandas
   ```

2. **Run the Service**:
   ```bash
   python app.py
   ```

3. **Verify Health**:
   Visit `http://localhost:5050/health` to confirm the model is loaded and ready.

---

## 📂 Model Artifacts
- `sms_model.pkl`: The trained classification model.
- `tfidf_vectorizer.pkl`: The vectorizer used to process text before prediction.

---

*MoneyMate Intelligence — Turning Text into Insights.*
