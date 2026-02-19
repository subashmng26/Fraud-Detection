# Fraud Detection Prediction App

A machine learning web application that predicts whether a financial transaction is fraudulent.

## Overview

This project uses a trained machine learning pipeline to classify transactions as:

- 1 → Fraud
- 0 → Not Fraud

The model is deployed using Streamlit to provide an interactive web interface.

## Features

- Transaction type selection
- Amount input
- Sender balance before & after transaction
- Receiver balance before & after transaction
- Real-time fraud prediction

## Tech Stack

- Python
- Pandas
- Scikit-learn
- Joblib
- Streamlit

## Project Structure

```
fraud_detection.py          # Streamlit app
fraud_detection_pipeline.pkl # Trained ML pipeline
README.md
requirements.txt
.gitignore
```

## Dataset

The dataset used for training is not included in this repository due to its large size (>450MB).

You can download it from:

https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset?resource=download

After downloading, place the dataset file in the project root directory before training the model.


Dataset Name: AIML Dataset  
Source: Kaggle  

Due to its size (>450MB), the dataset is not included in this repository.  
Please download it from Kaggle and place it in the project root directory before training.



## Installation

Clone the repository:

```
git clone https://github.com/subashmng26/fraud-detection-app.git
cd fraud-detection-app
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the application:

```
streamlit run fraud_detection.py
```

The app will open in your browser at:

```
http://localhost:8501
```

## Model Information

The model was trained as a supervised binary classification problem using transaction-related features such as:

- Transaction type
- Transaction amount
- Sender and receiver balance changes

The trained pipeline includes preprocessing and classification steps.

## Future Improvements

- Handle class imbalance
- Add model performance metrics
- Deploy to Streamlit Cloud
- Add model explainability (SHAP)

## License

This project is for educational purposes.

