# Iris Species Classification – Model Performance Comparison

## 📌 Project Overview

This project focuses on **Iris species classification** using different Machine Learning classification models. The performance of each model is evaluated and compared using **Accuracy, Precision, Recall, F1-Score, and Confusion Matrix**.

The models used in this project are:

- Logistic Regression
- Gaussian Naive Bayes
- K-Nearest Neighbors (KNN)

---

## 📊 Dataset

The project uses the **Iris dataset**, containing **150 samples** and the following features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The target variable is **Species**, containing three classes:

- Iris-setosa
- Iris-versicolor
- Iris-virginica

The `Id` column is removed before model training because it does not represent a meaningful feature for classification.

---

## 🔧 Data Preprocessing

The following preprocessing steps were performed:

1. Loaded the dataset using Pandas.
2. Checked for missing values.
3. Used `LabelEncoder` to convert the species into numerical labels.
4. Removed the `Id` column.
5. Separated features (`X`) and target (`y`).
6. Split the dataset into 50% training and 50% testing data.
7. Used `StandardScaler` for feature scaling in the KNN pipeline.

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

**Performance:**
- Accuracy: **100%**
- Precision: **100%**
- Recall: **100%**
- F1-Score: **100%**

### 2. Gaussian Naive Bayes

**Performance:**
- Accuracy: **98.67%**
- Precision: **98.61%**
- Recall: **98.55%**
- F1-Score: **98.55%**

### 3. K-Nearest Neighbors (KNN)

KNN was implemented using a **Pipeline with StandardScaler and GridSearchCV**.

The tested values of `n_neighbors` were:

```text
3, 5, 7, 9
```

5-fold cross-validation with **macro recall** was used for model selection.

**Performance:**
- Accuracy: **97.33%**
- Precision: **97.33%**
- Recall: **97.10%**
- F1-Score: **97.10%**

---

## 📈 Model Performance Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| **Logistic Regression** | **100.00%** | **100.00%** | **100.00%** | **100.00%** |
| Gaussian Naive Bayes | 98.67% | 98.61% | 98.55% | 98.55% |
| KNN | 97.33% | 97.33% | 97.10% | 97.10% |

### 🏆 Best Performing Model

Based on the test-set results, **Logistic Regression achieved the best performance**, with 100% accuracy, precision, recall, and F1-score.

---

## 🧮 Evaluation Metrics

The models were evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **Confusion Matrix**
- **Classification Report**

For this multiclass classification problem, **macro averaging** was used for Precision, Recall, and F1-Score.

---

## 🛠️ Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook
- StandardScaler
- GridSearchCV
- Pipeline

---

## 📂 Project Structure

```text
Iris-Species-Classification-Model-Performance-Comparison/
│
├── Iris_Species_Prediction_Using_Different_Models.ipynb
├── Iris.csv
└── README.md
```

---

## 🚀 How to Run

### Clone the repository

```bash
git clone https://github.com/your-username/Iris-Species-Classification-Model-Performance-Comparison.git
```

### Open the project

```bash
cd Iris-Species-Classification-Model-Performance-Comparison
```

### Start Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook and run the cells sequentially.

---

## 👨‍💻 Author

**Chandrashekhar Patidar**

B.Tech – Artificial Intelligence & Machine Learning

Acropolis Institute of Technology and Research, Indore

GitHub: `Chandrashekhar-Patidar`

---

## 📌 Conclusion

This project demonstrates and compares the performance of different Machine Learning classification algorithms on the Iris dataset.

Among the tested models, **Logistic Regression achieved the highest test-set performance**, followed by Gaussian Naive Bayes and KNN.