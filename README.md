# 💳 Credit Card Fraud Detection

This project focuses on detecting fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced, and we apply three classification algorithms—**Logistic Regression**, **K-Nearest Neighbors (KNN)**, and **Decision Tree**—to compare performance.

## 📁 Dataset

The dataset used is **[creditcard.csv]**, which contains transactions made by European cardholders. It includes:

- **Time**: Time elapsed between the transaction and the first transaction
- **V1-V28**: PCA components of original features (for confidentiality)
- **Amount**: Transaction amount
- **Class**: Target variable (1 = fraud, 0 = non-fraud)

> ⚠️ **Note:** The dataset is large (~150 MB) and has been removed from the repository to comply with GitHub's file size limit. Please download it manually from [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

---

## 🛠️ Technologies Used

- Python
- Jupyter Notebook
- NumPy & Pandas
- Scikit-learn (LogisticRegression, KNeighborsClassifier, DecisionTreeClassifier)
- Matplotlib (optional for visualization)

---

## 🚀 Project Workflow

1. **Data Loading & Cleaning**
   - Loaded dataset using `pandas`
   - Removed duplicate rows
   - Scaled `Amount` and `Time` using `StandardScaler`

2. **Train-Test Split**
   - Used `train_test_split` with 80/20 ratio

3. **Model Building**
   - Trained 3 different models:
     - Logistic Regression
     - K-Nearest Neighbors
     - Decision Tree Classifier

4. **Evaluation**
   - Accuracy score
   - Classification report (Precision, Recall, F1-score)

---

## 📊 Model Performance Snapshot

| Model               | Accuracy | Comment                       |
|--------------------|----------|-------------------------------|
| Logistic Regression| ~99.93%  | Performs well on imbalanced data |
| KNN                | ~99.91%  | Sensitive to scaling & K-value |
| Decision Tree      | ~99.93%  | Might overfit on training data |

> Detailed evaluation metrics are available in the notebook.

---

## 📁 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
