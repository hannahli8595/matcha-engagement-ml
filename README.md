# Matcha Engagement ML

An AI/ML project analyzing my own Instagram matcha account to understand and predict engagement across posts, reels, and media types.

## Project Overview
This project combines text, image, and metadata from my Instagram posts to:
- Store structured data in a relational database
- Perform exploratory and SQL-based analysis
- Build predictive & explainable ML models for engagement
- Deploy an interactive dashboard for recommendations

## Data Sources
- **Instagram export** from Meta ("Your Instagram Activity" → media, reels, posts)
- Text content: captions, hashtags, tagged users
- Media links: images, videos
- Metadata: timestamps, device info, GPS (when present)
- Engagement clues: gifted products, affiliate codes

## Tech Stack
- Python (pandas, scikit-learn, OpenCV, spaCy, matplotlib, seaborn)
- SQL (SQLite or PostgreSQL)
- Streamlit (dashboard)
- GitHub (version control)
- Jupyter Notebook (analysis)

## Repository Structure

```graphql
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
```
