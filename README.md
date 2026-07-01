# 🔍 Fraud & Anomaly Detection — Hybrid Ensemble Model 

A full-stack web application that detects fraudulent and anomalous transactions using a hybrid ensemble of supervised machine learning algorithms, built with Django and deployed as an interactive tool for real-time fraud screening.

<img width="572" height="270" alt="Screenshot 2026-07-01 091139" src="https://github.com/user-attachments/assets/4d8c6d85-3a78-4f5c-a2d9-f2827c6690c4" />


## 📌 Project Overview

Fraud detection is a high-stakes classification problem where missing a fraudulent transaction (false negative) or flagging a legitimate one (false positive) both carry real costs. This project combines multiple machine learning models into a hybrid ensemble to improve detection robustness, wrapped in a Django web application so the model can be used interactively rather than just in a notebook.

**Goal:** Build a usable tool where a transaction (or batch of transactions) can be checked for fraud/anomaly risk through a simple web interface.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Backend** | Python, Django |
| **Machine Learning** | Ensemble of supervised learning algorithms (e.g., Random Forest, SVM, Naive Bayes|
| **Data Handling** | Pandas, NumPy |
| **Frontend** | Django Templates / HTML / CSS |
| **Environment** | VS Code |

---

## 🔍 How It Works

1. **Data Preprocessing** — Cleaned and prepared transaction data (`Datasets.csv`, `Labeled_Data.csv`), including feature engineering to highlight patterns linked to fraudulent behavior.
2. **Model Building** — Trained a hybrid ensemble combining multiple supervised learning algorithms, aggregating their outputs to improve classification accuracy and reduce false positives.
3. **Web Integration** — Wrapped the trained model in a Django app (`views.py`, `models.py`, `forms.py`) so users can input transaction data and get a fraud/anomaly prediction through a browser interface.

---

#System design

<img width="568" height="268" alt="Screenshot 2026-07-01 091819" src="https://github.com/user-attachments/assets/172cbb4d-862a-4287-9192-75e578caee05" />

---
## 📊 Model Evaluation

```python
from sklearn.metrics import classification_report, confusion_matrix, accuracy_score

print(classification_report(y_test, y_pred))
print(confusion_matrix(y_test, y_pred))
print("Accuracy:", accuracy_score(y_test, y_pred))

---

## 🚀 Running the App Locally

```bash
# Clone the repository
git clone https://github.com/Vashista12/HYBRID-ENSMBLE-MODEL-FOR-FRAUD-AND-ANOMALY-DETECTION.git
cd HYBRID-ENSMBLE-MODEL-FOR-FRAUD-AND-ANOMALY-DETECTION

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the server
python manage.py runserver
```

Then open `http://127.0.0.1:8000/` in your browser.


---

## 📂 Repository Structure

```
HYBRID-ENSEMBLE-FRAUD-DETECTION/
├── Datasets.csv
├── Labeled_Data.csv
├── models.py
├── views.py
├── forms.py
├── admin.py
├── apps.py
├── manage.py
├── images/
│   └── app_screenshot.png
└── README.md
```

---

## Outputs
<img width="570" height="281" alt="Screenshot 2026-07-01 091157" src="https://github.com/user-attachments/assets/5cfbe49b-7353-46e4-974b-3d9201cff646" />

<img width="560" height="278" alt="Screenshot 2026-07-01 091209" src="https://github.com/user-attachments/assets/72627429-2f72-467a-ba8b-e3fc72e03da3" />

---

## 🔮 Future Improvements

- Add full model evaluation metrics (confusion matrix, ROC-AUC curve)
- Add a `requirements.txt` and setup instructions for reproducibility
- Deploy the app live (e.g., Render, Railway, or PythonAnywhere) and link it here
- Add unit tests (`tests.py` currently exists but may need actual test cases)

---

## 📬 Contact

**Vashista Chintalapalli**
📧 vashistachintalapalli12@gmail.com
🔗 [LinkedIn](https://linkedin.com/in/vashista-chintalapalli-9663362ba/) • [GitHub](https://github.com/Vashista12)
