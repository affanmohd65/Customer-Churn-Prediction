# 📈 Customer Churn Prediction

## Project Overview

This project focuses on predicting customer churn for a telecommunications company. By leveraging machine learning techniques, we aim to identify customers who are likely to churn, allowing the company to proactively intervene and improve customer retention strategies.

## Features

- **Data Preprocessing**: Handling missing values, encoding categorical features using Label Encoding, and converting data types.
- **Exploratory Data Analysis (EDA)**: Visualizing distributions of numerical features, analyzing categorical feature counts, and exploring correlations.
- **Imbalance Handling**: Addressing class imbalance in the target variable ('Churn') using SMOTE (Synthetic Minority Over-sampling Technique) to ensure robust model training.
- **Model Training**: Implementing and evaluating multiple classification models, including Decision Trees, Random Forests, and XGBoost, with cross-validation.
- **Model Evaluation**: Assessing model performance using accuracy score, confusion matrix, and classification reports.
- **Predictive System**: Developing a system to load the trained model and make predictions on new, unseen customer data.

## Technologies Used

- Python
- Pandas (for data manipulation)
- NumPy (for numerical operations)
- Matplotlib & Seaborn (for data visualization)
- Scikit-learn (for machine learning models and preprocessing)
- imbalanced-learn (for SMOTE)
- Pickle (for model persistence)

## How to Use

1.  **Clone the repository** (if applicable, otherwise assume it's in a Colab notebook).
2.  **Install dependencies**:
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost
    ```
3.  **Run the Jupyter Notebook / Google Colab**: Follow the cells sequentially to:
    - Load and preprocess the data.
    - Perform EDA.
    - Train the machine learning models.
    - Evaluate the models.
    - Use the predictive system to make new predictions.

## Dataset

The dataset used for this project is `Churn.csv`, containing various customer attributes and their churn status.

## Model Persistence

The trained Random Forest Classifier and the Label Encoders used for feature transformation are saved as `customer_churn_model.pkl` and `encoders.pkl` respectively, allowing for easy loading and deployment of the predictive system.

## Results

The Random Forest Classifier demonstrated the best performance among the evaluated models. The predictive system can take new customer data as input and output a prediction (Churn/No Churn) along with the associated probabilities.
