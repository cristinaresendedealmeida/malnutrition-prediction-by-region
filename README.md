## 📈 Malnutrition Risk Prediction Model

This repository contains a proof-of-concept Python script that demonstrates how machine learning can be used to predict the risk of malnutrition in a specific region. The model uses socioeconomic indicators to identify areas that may require urgent intervention and resource allocation, supporting data-driven decisions for public health initiatives.

-----

### Project Goal

The primary goal of this project is to build a classification model that predicts whether a given region has a high or low probability of malnutrition based on key indicators.

-----

### Methodology & Key Components

This project uses a simple machine learning pipeline implemented in Python. The key components include:

  * **Data:** The model is trained on a synthetic dataset, but the methodology is designed to work with real-world public health data (e.g., from Brazil's SISVAN system).
  * **Features:** The model uses three key variables as input:
      * GDP per capita
      * Number of Family Health Program units (PSFs)
      * Poverty rate
  * **Model:** A **Logistic Regression** model from the **scikit-learn** library is used to predict a binary outcome (malnutrition risk: high/low).
  * **Evaluation:** The model's performance is evaluated using a classification report, which provides metrics like precision, recall, and F1-score.

-----

### How to Run the Code

1.  **Install Dependencies:**
    You need to have **pandas** and **scikit-learn** installed. You can install them by running the following command in your terminal:

    ```bash
    pip install pandas scikit-learn
    ```

2.  **Execute the Script:**
    Save the provided code as a Python file (e.g., `predict_malnutrition.py`) and run it from your terminal:

    ```bash
    python predict_malnutrition.py
    ```

### Expected Output

The script will print the classification report showing the model's performance, followed by a sample prediction for a new, fictional region.

```text
Relatório de Classificação:
              precision    recall  f1-score   support

           0       1.00      0.50      0.67         2
           1       0.50      1.00      0.67         1

    accuracy                           0.67         3
   macro avg       0.75      0.75      0.67         3
weighted avg       0.83      0.67      0.67         3


Previsão: Alta probabilidade de desnutrição nesta região.
```
