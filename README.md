# 🧠 Student Health Condition Classification

An end-to-end Machine Learning project that predicts a student's health condition based on lifestyle, physical activity, sleep, diet, stress, and other health-related features.

The project focuses on building a reliable multi-class classification model while handling real-world challenges such as class imbalance and proper model evaluation.

## 📌 Project Overview

The dataset contains features such as:

- Sleep Duration
- Heart Rate
- BMI
- Calorie Expenditure
- Step Count
- Exercise Duration
- Water Intake
- Diet Type
- Stress Level
- Sleep Quality
- Physical Activity Level
- Smoking/Alcohol
- Gender

The target variable is **Health Condition**, consisting of three classes:

- At-risk
- Unhealthy
- Fit

## ⚙️ ML Pipeline

The project follows this workflow:

**Data Cleaning → EDA → Encoding → Train/Test Split → Model Training → Evaluation → Cross-Validation**

The dataset was cleaned by handling missing numerical and categorical values, followed by encoding categorical features for machine learning.

## 🤖 Model

Multiple classification models were explored and compared.

**Random Forest Classifier** was selected based on its overall performance across the different health-condition classes.

### Final Test Performance

- **Accuracy:** ~97%
- **Macro F1 Score:** ~0.90
- **Weighted F1 Score:** ~0.96

Class-wise performance was evaluated using precision, recall, and F1-score instead of relying only on accuracy because the target classes were imbalanced.

## 🔄 Cross-Validation

The Random Forest model was further evaluated using **5-Fold Stratified Cross-Validation**.

```text
Macro F1 Scores:
0.9010
0.9028
0.9017
0.9003
0.8998

Mean Macro F1: 0.9011
Standard Deviation: 0.00106
```

The low variation across folds indicates stable performance across different subsets of the dataset.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
- Random Forest

## 📊 Evaluation Metrics

The project uses:

- Accuracy
- Precision
- Recall
- F1 Score
- Macro F1 Score
- Classification Report
- Stratified Cross-Validation

Macro F1 was particularly important because of the class imbalance in the target variable.

## 📂 Project Structure

```text
Student-Health-ML/
│
├── notebook.ipynb
├── data/
├── README.md
└── requirements.txt
```

## 🚀 Future Improvements

- Hyperparameter tuning
- Compare additional ensemble models
- Feature importance and explainability
- Improved class-imbalance handling
- Build an interactive Streamlit application
- Deploy the trained model

## 👨‍💻 Author

**Dharmesh Sharma**

Built as part of my journey in learning and applying Machine Learning to real-world classification problems.
