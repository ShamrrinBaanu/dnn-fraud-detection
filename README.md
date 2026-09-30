## Stock Market Fraud Detection Using Deep Neural Networks

## 📌 Project Overview

This project uses a Deep Neural Network (DNN) to detect fraudulent financial transactions.

The model analyzes transaction-related features such as transaction amount, country, merchant, device information, VPN usage, failed attempts, unusual location, and account age to classify a transaction as:

- **0 → Not Fraud**
- **1 → Fraud**

The project demonstrates the complete machine learning workflow from data preprocessing to model training and evaluation.

---

## team member
Shreenidhi N P
Shamrrin Baanu S
Dhanushiya A
Francis Denisa A


## 🎯 Objectives

- Detect fraudulent financial transactions using Deep Learning.
- Preprocess numerical and categorical transaction data.
- Build a Deep Neural Network classification model.
- Predict whether a transaction is fraudulent or non-fraudulent.
- Evaluate the model using accuracy, precision, recall, F1-score, and a confusion matrix.

---

## 📂 Dataset

The dataset contains **50,000 financial transaction records** and **14 columns**.

### Main Features

| Feature | Description |
|---|---|
| `transaction_id` | Unique transaction identifier |
| `date` | Transaction date |
| `hour_of_day` | Hour at which transaction occurred |
| `amount_usd` | Transaction amount |
| `country` | Transaction country |
| `merchant` | Merchant involved in transaction |
| `category` | Transaction category |
| `card_type` | Type of card used |
| `is_new_device` | Indicates whether a new device was used |
| `vpn_used` | Indicates VPN usage |
| `failed_attempts_24h` | Failed attempts in the previous 24 hours |
| `unusual_location` | Indicates an unusual transaction location |
| `account_age_days` | Age of the account in days |
| `is_fraud` | Target variable |

### Target

```text
0 → Not Fraud
1 → Fraud


🧠 Model Architecture

The project uses a Deep Neural Network with the following architecture:

Input Features
      ↓
Dense Layer (128 neurons, ReLU)
      ↓
Dropout (30%)
      ↓
Dense Layer (64 neurons, ReLU)
      ↓
Dropout (20%)
      ↓
Dense Layer (32 neurons, ReLU)
      ↓
Output Layer (1 neuron, Sigmoid)
Training Configuration
Optimizer: Adam
Loss Function: Binary Crossentropy
Batch Size: 64
Maximum Epochs: 50
Early Stopping: Enabled
Train/Test Split: 80/20


⚙️ Technologies Used
Python
Pandas
NumPy
Scikit-learn
TensorFlow / Keras
Matplotlib
Seaborn
Jupyter Notebook


🔄 Project Workflow
Dataset
   ↓
Data Preprocessing
   ↓
Feature Engineering
   ↓
Train-Test Split
   ↓
Feature Scaling & Encoding
   ↓
Deep Neural Network
   ↓
Model Training
   ↓
Fraud Prediction
   ↓
Model Evaluation



📊 Model Evaluation

The model is evaluated using:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix

The complete implementation and generated results are available in the Jupyter Notebook.



📓 Jupyter Notebook

The fraud_detection.ipynb file contains:

Dataset loading
Data preprocessing
Feature engineering
DNN model creation
Model training
Fraud prediction
Classification report
Confusion matrix
Model evaluation

The notebook also contains the generated outputs and visualizations.



