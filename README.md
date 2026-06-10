# Bluestock Fintech — Mutual Fund Analytics Platform
**Capstone Project | June 2026 | Data Engineering + Analytics + Dashboard**

---



## Project Summary
End-to-end analytics platform for the Indian mutual fund industry.
- 40 real AMFI schemes
- 46,000+ NAV records
- 32,000+ investor transactions
- 4.5 years of market data

---

## Quick Start

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Copy CSV files
Paste all 10 CSV files into `data/raw/`

### 3. Run ETL pipeline
```bash
python scripts/etl_pipeline.py
```

### 4. Open Jupyter notebooks in order
```
notebooks/01_data_ingestion.ipynb
notebooks/02_data_cleaning.ipynb
notebooks/03_eda_analysis.ipynb
notebooks/04_performance_analytics.ipynb
notebooks/05_advanced_analytics.ipynb
```

### 5. Open dashboard
```
dashboard/bluestock_mf_dashboard.html  ← open in Chrome
dashboard/bluestock_mf.pbix            ← open in Power BI
```

---

## Folder Structure
```
Bluestock_MF_Capstone/
├── data/
│   ├── raw/                    ← 10 original CSV files
│   ├── processed/              ← cleaned CSVs
│   └── db/
│       └── bluestock_mf.db     ← SQLite database
├── notebooks/
│   ├── 01_data_ingestion.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda_analysis.ipynb
│   ├── 04_performance_analytics.ipynb
│   └── 05_advanced_analytics.ipynb
├── scripts/
│   └── etl_pipeline.py
├── sql/
│   └── schema_and_queries.sql
├── dashboard/
│   ├── bluestock_mf.pbix
│   └── bluestock_mf_dashboard.html
├── reports/
│   ├── Final_Report.docx
│   ├── Presentation.pptx
│   └── *.png (5 EDA charts)
├── requirements.txt
└── README.md
```

---

## Deliverables

| # | Deliverable | File | Status |
|---|---|---|---|
| D1 | ETL Pipeline | `scripts/etl_pipeline.py` | ✅ |
| D2 | SQLite Database | `data/db/bluestock_mf.db` | ✅ |
| D3 | EDA Notebook | `notebooks/03_eda_analysis.ipynb` | ✅ |
| D4 | Performance Metrics | `notebooks/04_performance_analytics.ipynb` | ✅ |
| D5 | Dashboard | `dashboard/bluestock_mf.pbix` | ✅ |
| D6 | Advanced Analytics | `notebooks/05_advanced_analytics.ipynb` | ✅ |
| D7 | Final Report | `reports/Final_Report.docx` | ✅ |

---

## Key Findings
1. SBI MF leads with ₹12.5L Cr AUM — doubled since 2022
2. SIP inflows grew 169% — ₹31,002 Cr all-time high Dec 2025
3. SBI Small Cap Direct tops scorecard (72.8/100)
4. Banking + IT = 34% of all equity portfolio weight
5. Folio count doubled from 13.26 Cr to 26.12 Cr (+97%)

---

## Data Sources
| Source | URL | Data |
|---|---|---|
| AMFI India | amfiindia.com | NAV, AUM, SIP, Folio |
| mfapi.in | api.mfapi.in/mf/{code} | Historical NAV |
| NSE India | nseindia.com | Nifty indices |
| BSE India | bseindia.com | BSE SmallCap |

> For educational purposes only. Not financial advice.
