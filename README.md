# matcha-engagement-ml

matcha-engagement-ml/
│
├── README.md                # Project summary & usage instructions
├── .gitignore               # Exclude raw data, secrets, environment files
├── LICENSE                  # MIT (or other) license
├── requirements.txt         # Python package dependencies
├── data/
│   ├── raw/                  # .gitignored - original Instagram export
│   ├── interim/              # processed intermediate CSVs
│   └── processed/            # clean ML-ready datasets
├── notebooks/
│   ├── 01_data_ingestion.ipynb
│   ├── 02_sql_analysis.ipynb
│   ├── 03_eda.ipynb
│   ├── 04_modeling.ipynb
│   ├── 05_advanced_analysis.ipynb
│   └── 06_dashboard_demo.ipynb
├── src/
│   ├── __init__.py
│   ├── data_ingestion.py     # parse HTML → DB
│   ├── feature_engineering.py
│   ├── modeling.py
│   └── utils.py
├── sql/
│   ├── schema.sql            # CREATE TABLE statements
│   └── eda_queries.sql
├── dashboard/
│   └── app.py                # Streamlit app
└── docs/
    └── er_diagram.png        # ER diagram & project documentation
