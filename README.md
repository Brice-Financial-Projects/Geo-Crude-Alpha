# 🛢️ Geo-Crude-Alpha

**Forecasting crude oil prices using geopolitical sentiment, weather data, and time series modeling.**

Geo-Crude-Alpha is a collaborative **quantitative research** project focused on building a multi-factor oil price prediction engine. We integrate **natural language processing (NLP)**, **weather-based feature signals**, and **time series forecasting techniques** to explore predictive relationships in global energy markets.

---

## 📌 Project Goals

- Extract sentiment from news headlines, social media, and global news sources related to **geopolitical and economic events**
- Integrate **weather data** as a factor influencing oil supply/demand dynamics
- Apply and compare **classical and deep learning time series models** (ARIMA, LSTM, Prophet)
- Visualize the impact of external features on crude oil pricing trends
- Deliver a modular and interpretable forecasting pipeline

---

## 🔍 Use Case

With increasing geopolitical risk and climate-related volatility, traditional oil pricing models fall short. Geo-Crude-Alpha aims to capture **real-time, real-world signals** from both structured and unstructured data to build a **smarter, adaptive forecasting framework** for energy markets.

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

- **Languages**: Python (Pandas, NumPy, scikit-learn, TensorFlow/PyTorch)
- **NLP**: spaCy, VADER, Hugging Face Transformers
- **Time Series**: statsmodels, Prophet, LSTM, tsfresh
- **Weather Data**: NOAA API, OpenWeatherMap
- **Visualization**: Plotly, Seaborn, Matplotlib

---

## 👥 Contributors

- [Brice A. Nelson](https://www.devbybrice.com) — *Data Strategist, ML Engineer, Full-Stack, Quant Research*
- [Ainesh Balaga](https://github.com/abalaga09) — *Quant Trader, Quant Research Collaborator*
- [Lex Pinedo](https://github.com/lexpinedo) — *Quant Research Collaborator*

---

## 🌱 Current Status

**In Progress** — Ainesh, Lex, and Brice are actively building the sentiment and weather pipelines. Time series model baselines are being explored.

---

## 📈 Future Work

- Integrate macroeconomic indicators (e.g., CPI, interest rates)
- Test transformer-based forecasting architectures (e.g., Temporal Fusion Transformer)
- Deploy interactive dashboard using Streamlit or Dash for live inference

---

## 🔁 Team Branches

| Branch Name   | Purpose                            |
|---------------|------------------------------------|
| `feat-QR`     | Quant Research (modeling, testing) |
| `feat-QT`     | Quant Trading (backtesting, metrics) |
| `feat-Data`   | Data Strategy (APIs, scraping, cleaning) |

---

## 🏷️ Keywords (for discoverability)

`quantitative research`, `oil price prediction`, `geopolitical sentiment`, `natural language processing`, `time series forecasting`, `weather data`, `crude oil`, `ARIMA`, `LSTM`, `Prophet`, `machine learning`, `energy markets`

---

## 📜 License

This project is open-source under the [MIT License](./LICENSE).
