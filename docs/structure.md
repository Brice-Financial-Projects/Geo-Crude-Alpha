# Geo-Crude-Alpha-File-Structure

geo-crude-alpha/
│
├── data/ # 📦 Versioned data folder (DO NOT track raw)
│   ├── raw/ # - Unprocessed input data (local copy only)
│   ├── interim/ # - Intermediate transformed data
│   ├── processed/ # - Final model-ready data
│   └── external/ # - 3rd party or externally sourced datasets
│
├── notebooks/ # 📓 Individual analysis notebooks (clearly scoped)
│   ├── eda/ # - Exploratory Data Analysis (one per team member)
│   ├── experiments/ # - Modeling experiments and failed trials
│   └── final/ # - Cleaned and shareable notebooks
│
├── reports/ # 📊 Analysis results and deliverables
│   ├── figures/ # - Generated plots/images
│   ├── metrics/ # - Output evaluation reports (.json/.csv)
│   └── summary/ # - Slide decks, executive summaries
│
├── models/ # 🤖 Trained model artifacts (versioned)
│   ├── checkpoints/ # - Intermediate model weights
│   ├── final_models/ # - Best-performing saved models
│   └── registry.json # - Registry of model versions and metadata
│
├── src/ # 🧩 Core source code
│   ├── init.py
│
│   ├── config/ # - Environment vars, API keys, secrets (local only)
│   │     └── settings.py
│
│   ├── data/ # - Data ingestion & transformation
│   │     ├── weather_loader.py
│   │     ├── sentiment_scraper.py
│   │     ├── merge_data.py
│   │     └── init.py
│
│   ├── features/ # - Feature engineering
│   │     ├── sentiment_features.py
│   │     ├── weather_features.py
│   │     └── lag_features.py
│
│   ├── modeling/ # - Forecasting models and wrappers
│   │     ├── arima_pipeline.py
│   │     ├── prophet_pipeline.py
│   │     ├── lstm_pipeline.py
│   │     └── base_model.py
│
│   ├── evaluation/ # - Backtesting and performance metrics
│   │     ├── backtest.py
│   │     ├── sharpe_calc.py
│   │     └── model_diagnostics.py
│
│   ├── pipeline/ # - Workflow orchestration (airflow, luigi optional)
│   │     └── full_pipeline.py
│
│   └── utils/ # - Logging, helpers, constants
│       ├── logger.py
│       ├── timer.py
│       └── config_loader.py
│
├── tests/ # ✅ Unit & integration tests
│   ├── test_data/
│   ├── test_features/
│   ├── test_modeling/
│   └── test_end_to_end.py
│
├── scripts/ # 🛠️ CLI or automation scripts
│   ├── run_training.py
│   ├── run_forecast.py
│   └── update_data.py
│
├── deployment/ # 🚀 App/streamlit deployment (optional)
│   ├── app.py
│   ├── requirements.txt
│   └── Procfile
│
├── docs/ # 🧾 Internal architecture, scopes, planning
│   ├── feat-QR_scope.md
│   ├── feat-Data_scope.md
│   ├── feat-QT_scope.md
│   ├── roadmap.md
│   ├── team_roles.md
│   ├── structure.md
│   └── architecture_diagram.drawio
│
├── .github/ # 🤖 CI/CD workflows and GH-specific config
│   └── workflows/
│   └── ci.yml
│
├── .env.example # Example of env var structure
├── .gitignore # Ignore data, secrets, etc.
├── README.md # Main overview + SEO
├── environment.yml # Full Conda environment (dev ready)
├── requirements.txt # Pip freeze version
├── setup.py # Optional: package structure
└── LICENSE # MIT or custom license