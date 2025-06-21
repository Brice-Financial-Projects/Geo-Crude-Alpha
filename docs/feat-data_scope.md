# 📡 Feature Branch Scope: `feat-Data`

## 🔍 Objective
The `feat-Data` branch is dedicated to building the data ingestion, transformation, and enrichment layer for the **Geo-Crude-Alpha** project. This branch serves as the foundation for all pipelines related to:

- Real-time and historical **weather data**
- **Geopolitical and economic news** scraping
- **Sentiment extraction** from text-based sources
- Preprocessing, cleaning, and storing structured datasets for modeling

---

## 🔧 Components in Scope

### 1. 🌦️ Weather Data Integration
- Connect to APIs such as NOAA, OpenWeatherMap, or WeatherAPI
- Normalize key weather variables (e.g., temperature, precipitation, storms)
- Map weather data to oil-producing regions and timestamps

### 2. 🗞️ Geopolitical & Market News Scraping
- Target reliable sources (e.g., Reuters, Bloomberg, OilPrice.com)
- Build scripts to collect, deduplicate, and timestamp articles
- Store raw and preprocessed text in a consistent format (CSV/JSON/DB)

### 3. 🧠 Sentiment Enrichment
- Implement basic sentiment scoring (VADER, TextBlob)
- Tag sentiment to key entities (countries, companies, commodities)
- Build structured output tables for modeling (date, source, sentiment, tag)

### 4. 🧹 Data Cleaning & Storage
- Handle missing values, outliers, and formatting inconsistencies
- Output to `.csv`, `.parquet`, or store in SQLite/DuckDB for later retrieval
- Ensure version-controlled `data/` subdirectory with raw, interim, and processed folders

---

## ⛔️ Out of Scope
The following are **not part** of `feat-Data` scope and belong to other feature branches:
- Time series forecasting models (→ `feat-QR`)
- Strategy implementation and trading logic (→ `feat-QT`)
- Dashboard/visualization frontends (→ future frontend branch or main)

---

## 📁 Suggested Subfolders
