# 🩺 Disease Detector

## 📌 Overview
The Disease Detector is a machine learning project designed to predict diseases based on patient health data. The model is trained using classification techniques to analyze symptoms/medical attributes and provide predictions that can assist in healthcare diagnostics.

This project is implemented in Python with Jupyter Notebook and leverages machine learning libraries for training and evaluation.

## 🚀 Features

Data preprocessing and cleaning for health-related datasets Training ML models for disease prediction Model evaluation with accuracy and metrics Exporting trained model for reuse Easy-to-use interface via Jupyter Notebook

## 🛠️ Technologies Used
Python 3.x NumPy, Pandas → Data handling Scikit-learn → Machine learning algorithms Matplotlib, Seaborn → Visualization Joblib → Model persistence

📂 Project Structure Disease_Detector/ │── Disease_Detector.ipynb # Main Jupyter Notebook │── requirements.txt # List of dependencies │── README.md # Project documentation │── models/ # Saved ML models │── data/ # Dataset (if available)

## ⚙️ Installation

Clone the repository: git clone https://github.com/Seth724/Disease-Prediction---ML.git cd Disease-Prediction---ML

Create and activate a virtual environment (recommended): python -m venv venv source venv/bin/activate # On Linux/Mac venv\Scripts\activate # On Windows

Install dependencies: pip install -r requirements.txt

# Data Preprocessing Script

This script also demonstrates how to handle missing values in numeric columns
of a pandas DataFrame.

## Code Example

``` python
numeric_columns = df.select_dtypes(include=['number']).columns
df[numeric_columns] = df[numeric_columns].fillna(df[numeric_columns].mean())
```

## Explanation

1.  **Select numeric columns**

    ``` python
    numeric_columns = df.select_dtypes(include=['number']).columns
    ```

    This selects all columns with numeric data types (integers, floats).

2.  **Fill missing values with column mean**

    ``` python
    df[numeric_columns] = df[numeric_columns].fillna(df[numeric_columns].mean())
    ```

    For each numeric column, missing values are replaced with the mean
    of that column.

## ▶️ Usage

Open Colab Notebook:

Run the Disease_Detector.ipynb file step by step.

Train the model and generate predictions.

(Optional) Use the saved model (.pkl file) for deployment in other applications.

📊 Example Workflow Load dataset Preprocess data Train ML model (Random Forest / Logistic Regression / etc.) Evaluate accuracy, confusion matrix Save trained model for later usage

🔮 Future Improvements Build a Streamlit Web App for user-friendly interaction Expand dataset for more disease categories Add Deep Learning models for better accuracy Deploy on Cloud (AWS/GCP/Heroku)

👨‍💻 Author

Sethna Amanethmi
