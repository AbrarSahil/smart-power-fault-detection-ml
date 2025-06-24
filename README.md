# Smart Power Fault Detection using Machine Learning

This project focuses on building a machine learning-based system to classify faults in electrical power systems. The aim is to automatically detect and classify different types of faults using real-time electrical parameters like voltage and current.

---

## 🔍 Problem Statement

Faults in power systems can lead to huge system losses or even blackouts. Manual monitoring is not scalable or efficient. We use supervised machine learning models to classify fault types based on features like voltage, current, and load parameters.

---

## 🧾 Dataset

**Dataset Source:** Kaggle (Dataset name: "Electrical Fault Detection and Classification")
**Format:** CSV files (`classData.csv`, `detect_dataset.csv`)
**Total Records:** 12,001 rows
**Features:**

* Ia, Ib, Ic (Line Currents)
* Va, Vb, Vc (Line Voltages)

**Target Class (Output S):**

* 0: Normal condition
* 1: Fault condition (aggregated faults)

---

## ⚙️ Tools and Libraries

* Google Colab
* Python
* pandas, numpy
* sklearn (Random Forest, SVM)
* xgboost
* matplotlib, seaborn

---

## 🚀 Model Building & Results

### 1. Random Forest

* Accuracy: **99.79%**
* Excellent classification and generalization

### 2. XGBoost

* Accuracy: **99.75%**
* Slightly less than Random Forest but still near-perfect

### 3. SVM (RBF Kernel)

* Accuracy: **98.38%**
* Performed well, but less robust to data variation than ensemble models

---

## 📊 Model Comparison

```
| Model           | Accuracy     |
|----------------|--------------|
| Random Forest  | 99.79%       |
| XGBoost        | 99.75%       |
| SVM            | 98.38%       |
```

---

## 📁 Project Structure

```
├── electrical-fault-detection-and-classification.zip
├── classData.csv
├── detect_dataset.csv
├── fault_detection_colab.ipynb
├── README.md
└── results/
    ├── model_accuracy_plot.png
    └── classification_reports.txt
```

---

## 📌 Future Work

* Fault type-specific classification (e.g., short-circuit, overload, ground fault)
* Real-time streaming with IoT/SCADA
* Deployment using Flask or FastAPI for real-time dashboards

---

## 👨‍💻 Author

**Abrar Mahir Uddin Sahil**
Machine Learning Enthusiast | Aspiring PhD in AI/Power Systems
