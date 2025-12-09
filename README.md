# 📈 Stock Price Movement & Price Prediction Using Machine Learning

This project investigates whether machine learning models can predict stock price direction (up/down) and future price values using historical market data and technical indicators. The study compares classical ML models for classification and an LSTM neural network for regression-based price forecasting.

---

## 🗂️ Project Overview

This repository contains:

- Preprocessing and feature engineering for stock datasets  
- Technical indicator computation (MA, EMA, MACD, Bollinger Bands, Momentum, etc.)
- Classification models:
  - Logistic Regression  
  - Random Forest  
  - Logistic Regression with Random Forest–based feature selection  
- LSTM model for price prediction  
- Visualizations and performance analysis  
- A research-style paper reporting methodology and results

The goal is to evaluate whether price direction and future values can be predicted using supervised learning models trained solely on historical price and indicator data.

---

## 📊 Models Implemented

### 1. Classification Models
Used to predict next-day movement (Up = 1, Down = 0):

- Logistic Regression  
- Random Forest Classifier  
- Logistic Regression + Random Forest Feature Ranking  
  - Uses top-k most important features  
  - Tests whether dimensionality reduction improves linear classifier performance

### 2. LSTM Regression Model
Trained to predict future closing prices, evaluated on:

- Entire test set  
- First year of test data  
- Last year of test data  

The LSTM uses a 60-day sliding window and normalized technical indicators as features.

---


## ⚙️ Installation & Setup

### **1. Clone the repository**

### **2. Create a virtual environment**
- python -m venv .venv
- source .venv/bin/Activate.ps1   (macOS/Linux)
- .venv\Scripts\Activate.ps1      (Windows)

### **3. Install dependencies**
- pip install -r requirements.txt

### **4. Run the ipynb with venv as kernel**
---
