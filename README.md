# Christian Callahan

**Data / ML Engineer — reproducible, leakage-safe machine learning and honest evaluation.**

I build models that hold up to scrutiny: leakage-safe labeling, real baselines, cross-validation, probability calibration, and a clear line between synthetic and real data. Every metric is committed and reproducible from a clean clone. I work end-to-end — from SQL/warehouse modeling through tuned models to Streamlit, FastAPI, and Next.js interfaces.

**I optimize for correct methodology over leaderboard numbers:** proper train/test discipline, baselines, calibration, and clearly-stated limitations.

**Now —** Founder & Principal at [CGC Labs](https://cgclabs.org), building the outsourced BI function for rural and critical access hospitals.

---

### Featured Projects

**[Pit Wall Intelligence](https://github.com/CCallahan308/pit-wall-intelligence)** — F1 race-strategy analytics: FastF1 data in a DuckDB + dbt warehouse; tyre-degradation and undercut-success models served via FastAPI and a 6-page Streamlit dashboard. Calibrated LightGBM undercut classifier (AUC 0.66 ± 0.05, 5-fold GroupKFold on 62/21 train/test race split — GREEN-flag stops only). Monte Carlo race simulator. Pit-cost calculator across 33 circuits with bootstrap CIs, SC/VSC regime separation.

**[SignalForge](https://github.com/CCallahan308/signalforge)** — Churn modeling on IBM Telco with statistical rigor: Optuna tuning, leakage-free CV, bootstrap 95% CIs, paired t-tests, calibration. The three models land within ~0.003 AUC with overlapping confidence intervals — model choice is a calibration/interpretability call, not an accuracy race.

**[SaaS Churn Simulator](https://github.com/CCallahan308/saas-churn-simulator)** — Leakage-safe churn + retention-ROI pipeline on RetailRocket (2.76M events). Time-windowed labeling, visitor-disjoint splits, Optuna-tuned LightGBM, isotonic calibration. 5-fold CV ROC-AUC 0.88 ± 0.06. Reports honestly that the ~99% base rate caps business lift. [Live demo →](https://saas-churn-simulator-ccallahan308.streamlit.app/)

**[Ecommerce Retention & Growth](https://github.com/CCallahan308/ecommerce-retention-growth)** — 30-day churn prediction and LTV segmentation on KKBox data; calibrated XGBoost (ROC-AUC ~0.79), ROI simulator. Ships a synthetic generator so it runs without the large download.

**[Ticket Intel](https://github.com/CCallahan308/ticket-intel)** — Support-ticket routing and summarization on Banking77 using TF-IDF + Naive Bayes by design: fast, interpretable, with a documented rationale for not using an LLM. [Live demo →](https://ticket-intel-ccallahan308.streamlit.app/)

---

### Also

- **[Healthcare SQL Analytics](https://github.com/CCallahan308/healthcare-sql-analytics)** — Production EHR analytics SQL patterns from 4 years of clinical and operational BI on Paragon: wRVU physician productivity, SDOH screening compliance, 340B drug utilization extract, sepsis missed-identification rate. Synthetic identifiers throughout.
- **[AutoModeler](https://github.com/CCallahan308/automodeler)** — Type a ticker, get a fully-linked 3-statement Excel model. FMP API · FastAPI · Python.

---

### Stack

`Python` `SQL` `TypeScript` `scikit-learn` `XGBoost` `LightGBM` `Optuna` `pandas` `DuckDB` `dbt` `FastAPI` `Streamlit` `Next.js` `PostgreSQL` `Prisma` `pytest` `GitHub Actions` `Docker` `Tableau`

---

### Background

- **Founder & Principal, CGC Labs** (2026–present) — the outsourced business analyst rural and critical access hospitals can't staff, on retainer: audit-ready CMS, HCAHPS, and MBQIP reporting, KPI governance, and the dashboards a small hospital would build in-house if it could afford the seat.
- **BI Analyst** (4 years) — clinical and operational analytics at a critical access hospital on Paragon: physician productivity, clinical quality (SDOH, sepsis, readmissions), 340B compliance, Tableau dashboards, and the BI-side data transformation on a Veradigm-to-Paragon EMR migration alongside Altera.
- **MBA + M.S. Data Science**, Eastern University (expected 2027).
- **Previously —** manufacturing and law enforcement: learned to find signal in noisy data and explain it to people who need a decision, not a model card.

---

[Portfolio](https://christiangcallahan.tech) · [LinkedIn](https://www.linkedin.com/in/christiangcallahan/) · [Email](mailto:Christian.G.Callahan@gmail.com)
