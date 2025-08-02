# NIDS
NIDS - a machine learning-based Network Intrusion Detection System (NIDS) using KNN for accurate and interpretable threat detection.

# Network Intrusion Detection System using Machine Learning (KNN)

This project implements a **Network Intrusion Detection System (NIDS)** using machine learning techniques, specifically the **K-Nearest Neighbors (KNN)** algorithm. It aims to identify malicious or abnormal network activity using the benchmark **NSL-KDD dataset**. The system supports both binary and multi-class classification and includes an optional real-time alerting feature.

---

## 📌 Features

- Intrusion detection using **KNN** classifier
- Achieves **98.2% accuracy** on NSL-KDD dataset
- Compares performance with **SVM** and **Autoencoder** models
- Real-time **email alert system** for detected intrusions
- Simple **Flask-based web interface** for CSV file upload and prediction

---
## 🧰 Tech Stack

Python · Flask · scikit-learn · pandas · NSL-KDD Dataset · HTML (Jinja2)
---

## 🧠 Algorithms Used

- **K-Nearest Neighbors (KNN)** – Main model
- **Support Vector Machine (SVM)** – Baseline comparison
- **Autoencoder (AE)** – Unsupervised benchmark

---

## 📊 Dataset

- **NSL-KDD Dataset**
  - A refined version of the original KDD Cup 1999 dataset
  - Free of redundant records
  - Ideal for benchmarking IDS models

📥 Download: [NSL-KDD on Kaggle](https://www.kaggle.com/datasets/galaxyh/kddcup99)

---

## 🏗️ Project Structure

nids-knn/
│
├── app.py                    # Flask web server
├── KDDTrain+.txt             # Training dataset
├── templates/
│   ├── index.html            # File upload page
│   └── result.html           # Prediction result display
├── static/                   # (optional) CSS/images if added
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation


---

## 🚀 How to Run

### 1. Clone the repository


git clone https://github.com/vvaishnavi1104/NIDS.git
cd nids-knn


### 2. Install dependencies


pip install -r requirements.txt


### 3. Run the app


python app.py


### 4. Access it in your browser


http://127.0.0.1:5000


## 📬 Real-Time Alerts

The system can send **email alerts** when an attack is detected.
To enable:

* Configure email credentials in `app.py`
* Enable less secure apps or use an app-specific password (if using Gmail/Outlook)

---

## 🧪 Results

| Model       | Accuracy |
| ----------- | -------- |
| **KNN**     | 98.2%    |
| SVM         | 96.6%    |
| Autoencoder | 93.7%    |

---

## 📌 Future Enhancements

* Real-time intrusion detection using live packet capture
* Cross-dataset validation (e.g., CICIDS2017, UNSW-NB15)
* Ensemble models for improved detection
* Lightweight deployment for IoT/edge devices

---

## 👥 Contributors

* Dasari Sathwika Reddy
* Chidara Akshitha
* V. Vaishnavi *(repo owner)*
* Guide: Dr. V. Harika

---

## 🌐 References

* [NSL-KDD Dataset](https://www.unb.ca/cic/datasets/nsl.html)
* Zhao, Zhenghui, *AI-driven NIDS*, ICISCN, 2025.
* Rahman, Shohanur et al., *NIDS using ML*, IEEE RAAICON, 2024.


**`requirements.txt`:**
``
flask
pandas
numpy
scikit-learn
matplotlib
seaborn




