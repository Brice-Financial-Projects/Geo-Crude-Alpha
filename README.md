# 🛢️ Geo-Crude-Alpha

**Forecasting crude oil prices using geopolitical sentiment, weather data, and time series analysis.**

Geo-Crude-Alpha is a collaborative quant research project focused on modeling oil price movements using a multi-factor framework. We integrate **NLP-driven sentiment analysis**, **weather-based signals**, and **time series forecasting techniques** to explore predictive relationships in global energy markets.

---

## 📌 Project Goals

- Extract sentiment from news headlines, social media, and other text data related to **geopolitical and economic events**
- Integrate weather data as a factor influencing oil supply/demand dynamics
- Apply and compare classical and machine learning time series models (ARIMA, LSTM, Prophet)
- Visualize the impact of external features (sentiment & weather) on oil price trends
- Deliver an interpretable and modular forecasting pipeline

---

## 🔍 Use Case

With growing geopolitical instability and climate-driven energy concerns, traditional oil price models fall short. Geo-Crude-Alpha aims to capture **real-time signals** from global events and environmental shifts to provide **smarter, more adaptable forecasting** tools.

---

## 📦 Project Structure (WIP)

geo-crude-alpha/
├── data/ # Raw and processed datasets
├── notebooks/ # EDA, modeling, and feature engineering
├── src/ # Core modules (NLP, weather integration, modeling)
├── models/ # Serialized models and forecasts
├── reports/ # Output visualizations and documentation
├── requirements.txt # Python dependencies
└── README.md # Project overview


---

## 🛠️ Technologies & Tools

- Python (Pandas, NumPy, scikit-learn, TensorFlow/PyTorch)
- Natural Language Processing (spaCy, VADER, Hugging Face Transformers)
- Weather APIs (e.g., NOAA, OpenWeatherMap)
- Time Series Libraries (statsmodels, Prophet, tsfresh)
- Data Visualization (Plotly, Matplotlib, Seaborn)

---

## 🚧 Current Status

**In Progress** — Ainesh, Lex, and Brice are currently collecting and preprocessing data for the sentiment and weather pipelines. Time series baselines are being established.

---

## 🤝 Contributors

- [Brice A. Nelson](https://www.devbybrice.com) — Data Strategist 
- Ainesh Balaga[TBD GitHub link] - Quant Trader Collaborator
- Lex Pinedo[TBD GitHub link] — Quant Research Collaborator

---

## 📈 Future Work

- Integrate macroeconomic data (CPI, interest rates)
- Experiment with transformer-based time series models
- Deploy as a Streamlit or Dash app for live forecasting

---

## 📜 License

This project is open source and freely available under the MIT License.

