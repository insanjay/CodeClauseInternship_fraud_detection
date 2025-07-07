# Credit Card Fraud Detection 🚨

This project is a machine learning solution for detecting fraudulent credit card transactions using sklearn LogisticRegression. It is designed for internship and learning purposes to showcase model training, evaluation, and basic deployment preparation.


## 📂 Project Structure

```
fraud_detection_project/
│
├── dataset/
│   └── sample.csv               # Sample dataset
│
├── model/
│   └── model.pkl                # Trained LogisticRegression model (saved)
│
├── notebooks/
│   └── fraud_detection.ipynb        # Full E2E Jupyter Notebook
│   └── testing_model.ipynb        # Tested the model here
│
├── snapshots/
│   └── classification_report.png               # Classification Report ss
│   └── confusion_matrix.png               # Confusion Matrix ss
│   └── model_testing_output.png               # Model Testing Output ss
│
├── README.md                        # Project overview
└── requirements.txt                 # Required libraries
```

## 🧠 Problem Statement

Fraudulent credit card transactions are rare but highly impactful. The goal is to train a machine learning model that can identify these frauds with high accuracy and minimal false negatives, using simple model.

## 📊 Dataset

- Source: [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/whenamancodes/fraud-detection)
- Transactions: 2,84,315
- Fraud cases: 492 (highly imbalanced)
- All features are anonymized via PCA (V1–V28) except for `Time`, `Amount`, and `Class`

## ✅ Workflow

1. **Import & Understand the Data**
2. **Preprocessing**
   - Feature scaling (`Amount`)
3. **Model Training**
   - Using `LogisticRegression` without hyperparameter tuning
4. **Evaluation**
   - Confusion Matrix
   - Classification Report (Precision, Recall, F1-score)
5. **Model Saving**
   - Using `joblib` to save the trained model for later use

## 🔍 Results

- **Model Used:** LogisticRegression
- **Best F1 Score Achieved:** ~74%
- **Accuracy:** ~99.92%
- **High Precision and Good Recall on Fraud Class**

## 🧪 Testing

You can test the model using a small sample from the dataset:

```
Consider using the notebook named "testing_model.ipynb", it will make the testing easier for you.
```

> ⚠️ Make sure sample data is **preprocessed in the same way** as training data (scaling etc.)

## 🛠 Dependencies

List of libraries used:

```
pandas  
scikit-learn  
joblib  
```

Install them via:

```bash
pip install -r requirements.txt
```

## 📌 Notes

* No hyperparameter tuning used  
* No advanced model involved 
* Focused purely on understanding model training and evaluation  
* This version is deployment-ready for local or future API integration

## 👤 Author

* **Sanjay Kumar**
* Portfolio: [GitHub](https://github.com/insanjay)
* LinkedIn: (www.linkedin.com/in/insanjay)