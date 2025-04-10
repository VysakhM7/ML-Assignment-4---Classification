# 🧠 Breast Cancer Classification – Supervised Learning Project

This project demonstrates the application of various supervised learning algorithms on the **Breast Cancer dataset** from `sklearn`. The goal is to classify tumors as malignant or benign using five popular classification techniques and compare their performance.

---

## 📂 Dataset

- **Source**: `sklearn.datasets.load_breast_cancer`
- **Samples**: 569
- **Features**: 30 numeric features (mean, standard error, and worst values of measurements)
- **Target**: Binary (0 = malignant, 1 = benign)

---

## 🧪 Objective

To evaluate and compare the following classification algorithms:

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **Support Vector Machine (SVM)**
5. **k-Nearest Neighbors (k-NN)**

---

## ⚙️ Preprocessing

- **Missing Values**: Checked and confirmed there are none.
- **Feature Scaling**: Standardization using `StandardScaler` from `sklearn.preprocessing` to ensure models like SVM and k-NN perform optimally.
- **Train-Test Split**: Dataset split into 80% training and 20% testing for model evaluation using `train_test_split`.

---

## 📊 Algorithms Overview

### 🔹 Logistic Regression
- A linear model used for binary classification.
- Suitable due to the simplicity and interpretability of results.

### 🔹 Decision Tree
- Non-linear model that splits data into branches based on feature values.
- Useful for interpretability but prone to overfitting.

### 🔹 Random Forest
- Ensemble method that builds multiple decision trees and averages the result.
- Reduces overfitting and improves accuracy.

### 🔹 SVM
- Finds an optimal hyperplane to separate classes in feature space.
- Works well for high-dimensional datasets.

### 🔹 k-NN
- Instance-based algorithm that classifies based on the most common label among the nearest neighbors.
- Simple but sensitive to feature scaling and choice of `k`.

---

## 📈 Results

Each model was evaluated using **accuracy** and **classification report (precision, recall, F1-score)**. Results may vary slightly depending on random state.

| Model              | Accuracy |
|-------------------|----------|
| Random Forest      | ~0.98    |
| SVM                | ~0.97    |
| Logistic Regression| ~0.96    |
| k-NN               | ~0.95    |
| Decision Tree      | ~0.93    |

> ✅ **Best Performing**: Random Forest  
> ❌ **Lowest Accuracy**: Decision Tree

---

## 📌 Project Structure

```
.
├── breast_cancer_classification.ipynb   # Main Jupyter Notebook
├── README.md                            # Project README
```

---

## 🚀 How to Run

1. Clone this repository  
2. Install dependencies (`scikit-learn`, `numpy`, `pandas`, `matplotlib`, `seaborn` if needed)  
3. Open the notebook and run cells step-by-step

---

## 📝 Author & License

- Developed as part of a supervised learning assessment project.
- Licensed under the [MIT License](LICENSE) *(optional to include)*

