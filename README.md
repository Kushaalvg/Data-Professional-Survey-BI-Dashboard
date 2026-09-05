# 📊 Global Data Professional Sentiment & Compensation BI Dashboard

## 📌 Project Overview
This repository contains an end-to-end data transformation and business intelligence project executed entirely within Microsoft Power BI Desktop. The pipeline ingests a fragmented, unformatted global survey dataset containing complex, nested text-based entries from data professionals across multiple industries, countries, and age groups. 

The raw input was cleaned via **Power Query**, modeled using an optimized relational **Star Schema**, and visualized through an interactive executive dashboard. This project simulates a corporate HR and market intelligence initiative, identifying the key drivers behind tech salary distributions, tool preferences, and workplace satisfaction vectors.

---

## 🎯 Core Business Questions Answered
1. **The Compensation Matrix:** How do current yearly salary tiers scale across distinct roles (`Data Analyst`, `Data Scientist`, `Data Engineer`)?
2. **The Tooling Ecosystem:** What are the actual preferred programming languages across new market entrants vs. veteran analysts?
3. **The Sentiment Vector:** How do critical workplace satisfaction metrics (`Work/Life Balance`, `Management Quality`, `Upward Mobility`) correlate across global geographic regions?
4. **Market Entry Friction:** How difficult is it for modern professionals to break into the data domain based on their education tier?

---

## 🛠️ Tech Stack & Advanced Power BI Features Used
* **ETL & Data Cleansing:** **Power Query Editor** (advanced delimiter splitting, string standardizations, removing text anomalies, and conditional formatting).
* **Data Modeling:** Built a robust **Star Schema Data Model** mapping flat multi-attribute records into optimized dimensional lookup layers connected via 1-to-many (`1:*`) relationships.
* **Analytical Expressions:** Formulated custom **DAX (Data Analysis Expressions)** measures to aggregate respondent sentiment scores and calculate regional averages.
* **UI/UX Reporting Design:** Engineered a clean, minimalist dark-themed executive canvas utilizing cross-filtering **Slicers** (Region, Education, Title) and dynamic KPI card indicators.

---

## 📂 Repository Architecture & File Mapping
```text
Data-Professional-Survey-BI-Dashboard/
│
├── Data_Professional_Survey_Dashboard.pbix  --> [Master Power BI Visual Report File]
├── Data_Professional_Survey_Raw.csv         --> [Raw Unformatted Input Dataset]
└── README.md                                --> [Master Project Documentation]
```

---

## 📂 Ingestion & Data Quality Transformations (ETL)

To protect chart axis boundaries and eliminate default reporting noise, the raw dataset underwent comprehensive programmatic restructuring inside Power Query:
* **Fuzzy Categorical Cleanups:** Handled cluttered country extensions (e.g., mapping text anomalies like `"Other (Please Specify):Nigeria"` cleanly into `"Nigeria"`).
* **Delimiter Text Splitting:** Parsed custom long-form text responses within the programming column (e.g., custom feedback fields) using advanced word-boundary isolations to extract clean tool variables (`Python`, `R`, `SQL`).
* **Axis Optimization:** Applied systematic numeric indexing to text-based salary and difficulty columns to override default alphabetical chart sorting, ensuring financial distributions flow chronologically from lowest to highest.

---

## 📈 Executive Insights Summary
* **The Dominant Stack:** Python continues to hold a massive lead over R and native SQL variants as the top preferred language among modern data professionals, making it a critical asset for candidate screenings.
* **The Sweet Spot:** The `Middle Age` cohort represents the absolute engine of conversion volume, with professional data analysts concentrating heavily in the `$41k-$65k` and `$66k-$85k` USD brackets depending on corporate sector scaling.
* **Remote Work Propensity:** Workplace satisfaction metrics reveal a massive positive correlation between high `Work/Life Balance` scores and organizations offering flexible or 100% remote-work infrastructure.

---

## 📊 Data Quality & Optimization Impact Matrix

| Analytical Dimension | Ingested Dataset Condition | Optimized Production Condition | Business Value Passed to Boardroom |
| :--- | :--- | :--- | :--- |
| **Tool Categorization** | Fragmented custom text blocks | **Isolated Clean Variables** | Ensures flawless segmentation inside visual tool charts. |
| **Geographic Mappings** | Unstandardized country text rows | **Normalized Country Fields** | Prevents visual map splits and geographical reporting errors. |
| **Salary Distribution** | Scrambled text brackets | **Indexed Chronological Flow** | Grants the C-suite a logical, progressive view of income tiers. |
| **Data Schema** | Flat, bloated single sheet | **Relational Star Schema Model** | Drastically minimizes dashboard calculation latency. |

---

## 🏁 Automation & Maintenance
Because the data preparation lifecycle was engineered entirely through native **Power Query steps**, this dashboard layout is fully automated and scalable. When next quarter's raw survey records are dropped into the source folder, stakeholders simply click **'Refresh All'** on the Power BI Home ribbon. The data model will instantly re-run the text splits, calculate the structural metrics, and update the executive visualizations automatically in seconds.
