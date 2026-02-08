# 🩺 Diabetes Detection Machine Learning Project

**A machine learning pipeline to detect diabetes using clinical and lifestyle features.**

This repository contains a complete ML workflow — from exploratory data analysis and preprocessing to model training, evaluation, and visualization.

---

## 📌 Problem Statement

Diabetes is a major global health issue. Early and accurate detection can help prevent long-term complications. This project builds and evaluates ML models to classify whether a person is diabetic based on features such as glucose level, BMI, blood pressure, age, etc.

The project implements:
- Data cleaning and preprocessing
- Model training
- Hyperparameter tuning
- Evaluation using robust metrics

---

## 📂 Repository Structure

```

Diabeties_Detection/
│
├── Notebook.ipynb               # Main notebook with EDA and modeling steps
├── requirements.txt             # Python dependencies
├── Diabetes Prediction Dataset/ # Original dataset (if included)
├── models/                     # Saved trained models (optional)
├── visuals/                    # Plots and charts (optional)
└── README.md

````

---

## 🧠 Approach

The project consists of:

### 🔹 1. Exploratory Data Analysis (EDA)
- Summary statistics
- Class distribution bar charts
- Histograms and distributions to understand skewness and outliers

### 🔹 2. Data Cleaning
- Replace impossible 0-values (e.g., in glucose, BMI) with `NaN`
- Handle missing values using median imputation

### 🔹 3. Data Preprocessing
- Feature scaling using StandardScaler
- Train-validation split
- Cross-validation to ensure robust model evaluation

### 🔹 4. Model Training
Implemented classifiers:
- **K-Nearest Neighbors (KNN)**
- **Logistic Regression**
- **Random Forest**

Cross-validation and hyperparameter tuning were used to find optimal models.

---

## 📊 Evaluation Metrics

To compare models, the following metrics were used:

| Metric        | Description |
|---------------|-------------|
| Accuracy      | Fraction of correct predictions |
| ROC-AUC       | Area under the ROC curve (ranking ability) |
| Precision     | Correctness of positive predictions |
| Recall        | Ability to detect positive class |

ROC-AUC was emphasized for better evaluation of classifier performance on imbalanced datasets.

---

## 💡 Key Results

| Model                  | Validation Accuracy | Validation ROC-AUC |
|------------------------|---------------------|---------------------|
| K-Nearest Neighbors    | ~0.72               | ~0.75               |
| Logistic Regression    | ~0.75               | ~0.78               |
| Random Forest          | ~0.74               | ~0.76               |

**Logistic Regression performed best overall for this dataset.**

---

## 🧪 How to Run

1. Clone the repository

```bash
git clone https://github.com/PriyanshuN19/Diabeties_Detection.git
cd Diabeties_Detection
````

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Open and run the notebook:

```bash
jupyter notebook Notebook.ipynb
```

---

## 🔁 Future Work

* Try **Gradient Boosting Models** (XGBoost / LightGBM) for potential improvement.
* Visualize **feature importance** to find most predictive factors.
* Explore **SMOTE / class weights** if class imbalance impacts performance.
* Deploy as a web app using **Streamlit / Flask / FastAPI** for real-time predictions.

---

## 📬 Contact

Made by **Priyanshu Nailwal**

Feel free to raise issues or contribute improvements!

---

## 📄 License

This project is open-source and free to use.
