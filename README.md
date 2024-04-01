# Heart Disease Prediction

This project aims to predict the presence of heart disease based on various health metrics using machine learning. The dataset used for this project contains information such as age, sex, cholesterol levels, and other factors that may be indicative of heart disease.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository to your local machine.
2. Install the required Python packages using `pip install -r requirements.txt`.
3. Run the `heart_disease_prediction.ipynb` notebook to train the model and make predictions.

## Dataset

The dataset used for this project is available in the file `heart_disease_data.csv`. It contains the following columns:

- Age
- Sex
- Chest pain type (cp)
- Resting blood pressure (trestbps)
- Serum cholesterol in mg/dl (chol)
- Fasting blood sugar > 120 mg/dl (fbs)
- Resting electrocardiographic results (restecg)
- Maximum heart rate achieved (thalach)
- Exercise induced angina (exang)
- ST depression induced by exercise relative to rest (oldpeak)
- Slope of the peak exercise ST segment (slope)
- Number of major vessels (0-3) colored by fluoroscopy (ca)
- Thalassemia (thal)
- Target variable: Presence of heart disease (1 = Yes, 0 = No)

## Model Training and Evaluation

The data is split into training and testing sets using a 80-20 split. A logistic regression model is trained on the training set and evaluated on the test set. The model achieves an accuracy of approximately 85.5% on the training data.

## Making Predictions

To make predictions for new data, create a tuple containing the input values for the following features in the order listed above: age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal. Then, use the `predict` method of the trained model to predict the presence of heart disease.
