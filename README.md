# Time-Series-Forecasting-ARIMA-
Time-series analysis and forecasting of **electricity Load** and **Solar Generation** for the year *2016* using classical ARIMA models.  
# ⚡ Forecasting Energy Load & Solar Generation using ARIMA (2016 Data)

Time-series analysis and forecasting of **electricity Load** and **Solar Generation** for the year *2016* using classical ARIMA models.  

---

## 📊 Dataset

- File: `TimeSeries_TotalSolarGen_and_Load_IT_2016.csv`
- Attributes:
  - `utc_timestamp`
  - `IT_load_new`
  - `IT_solar_generation`

---

## 🔧 Tools Used

Python ・ Pandas ・ Matplotlib ・ Statsmodels ・ Sklearn

---

## 🔁 Project Steps

1. **Load & Visualize data**
2. **Handle Missing Values** (`forward fill`)
3. **Stationarity Check** → *Augmented Dickey-Fuller Test*
4. **Plot ACF & PACF** → to determine p, d, q
5. **Split Train/Test (80-20)**
6. **Build ARIMA models**
7. **Evaluate using RMSE**
8. **Grid search to find best (p, d, q)**

---

## 🔍 Key Results

| Series               | Best Model    | RMSE        |
|---------------------|--------------:|------------:|
| IT_load_new         | ARIMA (2,1,2) | ~ 993       |
| IT_solar_generation | ARIMA (3,1,3) | ~ 2302.7    |

---

## 📉 Visualization

Plots include:
- Load vs Solar Generation (time series)
- ACF & PACF
- Actual vs Predicted curves

---

## 📂 Folder Structure

├── TimeSeries_TotalSolarGen_and_Load_IT_2016.csv
├── ARIMA_Forecasting.ipynb
└── README.md


---

## ⚠️ Limitations

- ARIMA struggles to capture sharp peaks.
- Does not handle **seasonality** explicitly — *SARIMA* or *LSTM* could improve performance.

---

## 🧠 Possible Extensions

- Seasonal ARIMA (SARIMA)
- Exogenous variables → SARIMAX (weather, holidays)
- Deep Learning → LSTM/RNN

---

## ✍️ Author

**Mohammed Sohail**  
