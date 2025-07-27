# 📈 Unemployment Rate Forecasting by Age Group using LSTM

This project predicts the monthly unemployment rate for multiple age groups using a **Long Short-Term Memory (LSTM)** model. It uses multivariate time series data to forecast future unemployment trends, providing insights that can assist policymakers and researchers.

---

## 📂 Project Overview

This deep learning project was developed as a final assignment for the Deep Learning course at **Politeknik Caltex Riau**.

- **Goal**: Predict unemployment rates for age groups using historical time series data.
- **Approach**: Preprocess, normalize, window, and feed data into an LSTM model for forecasting.
- **Scope**: 7 age groups over 16 years (2008–2024).

---

## 📊 Dataset

- **Source**: [Kaggle - Unemployment by Age Groups](https://www.kaggle.com/datasets/sahirmaharajj/unemployment-by-age-groups-dataset)
- **Timeframe**: Feb 2008 – Mar 2024
- **Frequency**: Monthly
- **Features**:
  - `Unemployment_16_19`
  - `Unemployment_20_24`
  - `Unemployment_25_34`
  - `Unemployment_35_44`
  - `Unemployment_45_54`
  - `Unemployment_55_64`
  - `Unemployment_65_plus`

---

## 🧠 Model Architecture

- **Model**: LSTM
- **Layers**:
  - LSTM (64 units)
  - Dropout
  - Dense Output Layer
- **Training Params**:
  - Epochs: 50
  - Batch Size: 16
  - Loss Function: MSE
  - Optimizer: Adam

---

## ⚙️ Preprocessing Steps

- Convert `Date` to datetime
- Handle missing values (linear interpolation)
- Normalize features using `MinMaxScaler`
- Create sliding window (e.g., 6 months input → 1-month output)
- Split into 80% train and 20% test (chronologically)

---

## 📈 Evaluation Metrics

- **Mean Absolute Error (MAE)**
- **Root Mean Squared Error (RMSE)**

Results showed the model performs well, particularly for younger age groups (16–24), with low forecasting error and clear trend capture.

---

## 📊 Visualizations

- Unemployment rate trends per age group
- Correlation heatmaps between age groups
- Actual vs Predicted plots for all segments
- 12-month future forecast using autoregressive predictions

---

## 👥 Authors

- **Davin Williem** – [GitHub](https://github.com/Vinonyx)  
- **Rio Fitra Mutaqin**

Supervised by:  
Dr. Juni Nurma Sari, S.Kom., M.MT  
Ahmad Ali Munawar, S.Tr. Kom

---

## 📄 License

This project is intended for academic and research purposes. Please credit the authors when reusing any part of the work.

---
