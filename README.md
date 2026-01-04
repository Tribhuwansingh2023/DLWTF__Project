# DLWTF__Project

## Agricultural Commodity Price Prediction  
### Using Machine Learning and Deep Learning Techniques

This repository contains the **Major Project** developed for the course  
**Deep Learning with TensorFlow – I (CSE3793)** as part of the  
**B.Tech. Computer Science and Engineering (AI & ML), Semester 5**.

The project focuses on analyzing and predicting agricultural commodity prices using
historical market data from Indian agricultural markets. It emphasizes exploratory data
analysis, feature engineering, and a feasibility comparison of machine learning and deep
learning models under real-world data constraints.

---

## 📌 Project Overview

Agricultural commodity prices are highly volatile due to factors such as seasonal supply,
market demand, weather conditions, transportation constraints, and government policies.
Accurate price prediction can support farmers, traders, and policymakers in making
better-informed decisions.

In this project, historical weekly price data is analyzed to understand price behavior and
evaluate predictive models for short-term agricultural price forecasting. While deep learning
models such as LSTM, GRU, and Transformer-based architectures are explored for feasibility,
a feature-based **Random Forest Regressor** is used as the primary predictive model due to
data limitations.

---

## 🗂️ Dataset

- **Source:** Indian agricultural market price records  
- **File:** `Price_Agriculture_commodities_Week.csv`  
- **Total Records:** 23,093  
- **Attributes:** 10  
- **Date Range:** 27 July 2023 – 02 August 2023  
- **Target Variable:** Modal Price (Rs/quintal)

### Key Attributes
- State, District, Market  
- Commodity, Variety, Grade  
- Arrival Date  
- Minimum Price, Maximum Price, Modal Price  

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Date conversion and chronological sorting  
   - Missing value and duplicate checks  
   - Filtering records for time-series feasibility  

2. **Exploratory Data Analysis (EDA)**
   - Commodity-wise distribution  
   - Price trend and volatility analysis  

3. **Feature Engineering**
   - Lag-based price features  
   - Rolling mean and rolling standard deviation  
   - Calendar-based features  

4. **Modeling**
   - **Primary Model:** Random Forest Regression  
   - **Explored Models:** LSTM, GRU, Transformer (feasibility analysis)

5. **Evaluation Metrics**
   - Root Mean Square Error (RMSE)  
   - Mean Absolute Error (MAE)  
   - R² Score  

---

## 📊 Results

The Random Forest regression model achieved strong predictive performance:

- **RMSE:** 1783.43  
- **MAE:** 565.09  
- **R² Score:** 0.8861  

Actual vs. predicted price visualizations (e.g., for Potato) show that the model effectively
captures general price trends, with deviations during sudden market fluctuations.

---

## ⚠️ Limitations

- Short and irregular time-series length for individual commodities  
- Absence of external influencing factors (weather, fuel prices, policies)  
- Limited suitability of deep learning models due to data constraints  
- Offline, batch-based prediction (no real-time deployment)

---

## 🚀 Future Scope

- Use of longer and more continuous historical datasets  
- Integration of external variables such as weather and inflation data  
- Application of advanced architectures like Temporal Fusion Transformers  
- Deployment as a real-time web or mobile decision-support system  

---

## 🛠️ Tech Stack

- **Programming Language:** Python 3.8+  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning:** Scikit-learn  
- **Deep Learning:** TensorFlow, Keras  
- **Environment:** Jupyter Notebook / Google Colab  

---

## 👥 Authors

- **Tribhuwan Singh** (Reg. No: 2341019538)  
- **Surajit Sahoo** (Reg. No: 2341019165)  
- **Badri Narayan Patra** (Reg. No: 2341016251)  

B.Tech. Computer Science and Engineering (AI & ML)  
Siksha ‘O’ Anusandhan (Deemed to be University)

---

## 📄 License

This project is intended for **academic and educational purposes only**.
