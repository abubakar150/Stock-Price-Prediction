# 📊 Stock Price Prediction using LSTM

This project was developed as part of an internship by **Hafiz Muhammad Abubakar Bhatti** (Intern ID: ARCH-2508-0867) at **Arch Technologies**. It demonstrates the use of Long Short-Term Memory (LSTM) neural networks for predicting stock prices based on historical data including Open, High, Low, Close, and Volume.

---

## 🔍 Overview

The goal of this project is to build a machine learning model that predicts the future closing price of a stock using past data. Real-time stock data (e.g., Apple - AAPL) is retrieved using the `yfinance` API, preprocessed using MinMaxScaler, and passed through a two-layer LSTM model for time series forecasting.

---

## ✅ Features

- Real-time stock data collection with `yfinance`
- Feature scaling using `MinMaxScaler`
- Sequence generation using sliding window (60 days)
- LSTM model training using TensorFlow/Keras
- Visualization of actual vs. predicted prices
- Evaluation using Mean Squared Error (MSE)

---

## 🧰 Tools & Technologies

- Python 3.x  
- Google Colab / Jupyter Notebook  
- Libraries: `yfinance`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `tensorflow.keras`

---

## 📂 Files Included

- `stock_price_prediction.ipynb` – Main notebook
- `README.md` – Project overview
- `Internship_Report.docx` – Internship submission report
- `requirements.txt` – Required Python packages

---

## 🧠 How It Works

1. **Data Collection:** AAPL stock data (2020–2024) downloaded using `yfinance`.
2. **Preprocessing:** Normalization + 60-day sequence creation.
3. **Model Building:** LSTM layers with Dense output.
4. **Training:** Model trained over 10 epochs with batch size 32.
5. **Evaluation:** MSE + plot of actual vs. predicted prices.

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/stock-price-prediction.git
cd stock-price-prediction
pip install -r requirements.txt
jupyter notebook stock_price_prediction.ipynb
