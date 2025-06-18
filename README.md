# ⚡ Energy Consumption Forecasting Using Machine Learning

A data science project that predicts hourly electricity demand using historical load, weather conditions, and time-based features. This solution helps utility companies and smart grid operators optimize power distribution, minimize wastage, and improve grid reliability.

---

## 📌 Project Overview

This project implements a regression model (XGBoost) to forecast energy consumption (in kWh) at an hourly level. It uses:

- Historical electricity load data
- Weather parameters (temperature, humidity, wind speed, solar radiation)
- Time-based features (hour, weekday, month, holiday/weekend)
- Lagged and rolling historical consumption values

---

## 🛠️ Tools & Technologies

- **Language:** Python 3.10+
- **Libraries:** `pandas`, `numpy`, `xgboost`, `matplotlib`, `seaborn`, `scikit-learn`, `joblib`
- **Model:** Gradient Boosting Regression (`XGBRegressor`)

---

## 📂 Project Structure

├── train_model.py # Main script to train the model
├── data_preprocessing.py # Functions for loading and preparing data
├── energy_model.joblib # Trained regression model (output)
├── load.csv # Historical electricity load data
├── weather.csv # Hourly weather data

---

## 🧠 Features Used

| Feature           | Description                                  |
|------------------|----------------------------------------------|
| `temperature`     | Ambient temperature (°C)                     |
| `humidity`        | Relative humidity (%)                        |
| `wind_speed`      | Wind speed (m/s)                             |
| `solar_radiation` | Solar radiation (W/m²)                       |
| `hour`            | Hour of day (0–23)                           |
| `dayofweek`       | Day of week (0–6)                            |
| `month`           | Calendar month (1–12)                        |
| `is_weekend`      | 1 if weekend, 0 otherwise                    |
| `lag_1h`          | Load one hour before                         |
| `lag_24h`         | Load 24 hours before                         |
| `rolling_24h`     | 24-hour rolling mean of load                 |

---


🌍 Real-World Applications

🏙️ Smart Grid Management – Balance supply and demand dynamically

🧾 Billing Forecasts – Predict consumer-level electricity usage

🌤️ Renewable Integration – Optimize solar/wind-based generation scheduling

📦 Infrastructure Planning – Anticipate peak demand periods

🧠 Energy Behavior Analysis – Detect anomalous or wasteful usage patterns

📜 License
This project is licensed under the MIT License.
