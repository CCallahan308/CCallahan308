# Christian Callahan

**Data Scientist — experimentation, forecasting, and churn/LTV modeling, with the evaluation discipline to know when a model isn't working.**

I build models that hold up to scrutiny: leakage-safe labeling, real baselines, cross-validation, probability calibration, and a clear line between synthetic and real data. Every metric is committed and reproducible from a clean clone. I work end-to-end — from SQL/warehouse modeling through tuned models to Streamlit, FastAPI, and Next.js interfaces.

**I optimize for correct methodology over leaderboard numbers:** proper train/test discipline, baselines, calibration, and clearly-stated limitations.

**Now —** Founder & Principal at [CGC Labs](https://cgclabs.org), building the outsourced BI function for rural and critical access hospitals.

---

### Featured Projects

**[Rural Hospital Closure Risk](https://github.com/CCallahan308/rural-hospital-distress)** — Master's capstone: predicting 1–2 year closure/conversion risk for US rural hospitals from public CMS cost reports alone — 89,912 hospital-years (1997–2021) containing just 133 closures (0.148% base rate). XGBoost, discrete-time hazard, and logistic models with forward-chaining temporal CV, isotonic calibration, SHAP, and a 10-check leakage audit. Hold-out 2019–2021: AUROC 0.867 with 43.7× lift; 3 of the 6 real closures rank in the top 1.2% of scores. The central finding is a defect story: an in-sample calibration bug collapsed scores to ~0 for 11,759 of 11,760 hold-out rows — a false negative (AUROC 0.50) previously blamed on COVID relief funding. Finding and fixing it restored the ranking. 156 tests, published [static report](https://ccallahan308.github.io/rural-hospital-distress/).

**[ED Operations Analytics](https://github.com/CCallahan308/ed-operations-scotland)** — Site-level forecasting of NHS Scotland A&E 4-hour compliance on real Public Health Scotland open data (7,022 Type-1 site-months, 2007–2026). Chronological split, frozen config, holdout scored exactly once; a DuckDB star schema reconciled row-for-row to the Python pipeline. Gradient-boosted + persistence ensemble hits 2.72 pp holdout MAE against a 2.87 pp persistence baseline — but the paired-bootstrap 95% CI on that improvement includes zero, and the README leads with that rather than the win. 111 tests, CI on 3.11/3.12, deployed Streamlit dashboard.

**[A/B Test & Experimentation Analyzer](https://github.com/CCallahan308/ab-test-analyzer)** — A decision engine that returns ship / hold / iterate / kill, not a p-value: power vs a pre-specified minimum worthwhile effect, CIs, Cohen's h, and a sample-ratio-mismatch check on every result; exploratory segments with Holm correction. On the canonical Udacity experiment (290,584 users) it returns an honest, well-powered null — p=0.19 with >99% power to detect the 1pp effect worth shipping — and explains why that's a decision, not a failure. Every README figure regenerates via `scripts/compute_findings.py`; all 16 analytical choices documented in `ASSUMPTIONS.md`. 37 tests.

**[SignalForge](https://github.com/CCallahan308/signalforge)** — Churn modeling on IBM Telco with statistical rigor: Optuna tuning, leakage-free CV, bootstrap 95% CIs, paired t-tests, calibration. The three models land within ~0.003 AUC with overlapping confidence intervals — model choice is a calibration/interpretability call, not an accuracy race.

**[Ticket Intel](https://github.com/CCallahan308/ticket-intel)** — Support-ticket routing and summarization on Banking77 using TF-IDF + Naive Bayes by design: fast, interpretable, with a documented rationale for not using an LLM. [Live demo →](https://ticket-intel-ccallahan308.streamlit.app/)

**[AutoModeler](https://github.com/CCallahan308/automodeler)** — Type a ticker, get a fully-linked 3-statement Excel model with native formulas. FMP API · FastAPI · Python.

---

### Also

- **[Pit Wall Intelligence](https://github.com/CCallahan308/pit-wall-intelligence)** — F1 race strategy: FastF1 → DuckDB + dbt warehouse, calibrated LightGBM undercut classifier, Monte Carlo race simulator, pit-cost calculator across 33 circuits.
- **[SaaS Churn Simulator](https://github.com/CCallahan308/saas-churn-simulator)** — Retention-ROI simulation on 2.76M RetailRocket events: what a churn model is worth when the base rate caps lift. [Live demo →](https://saas-churn-simulator-ccallahan308.streamlit.app/)
- **[Ecommerce Retention & Growth](https://github.com/CCallahan308/ecommerce-retention-growth)** — LTV segmentation and win-back budget sizing on KKBox data, with a synthetic generator so it runs cold.
- **[Healthcare SQL Analytics](https://github.com/CCallahan308/healthcare-sql-analytics)** — Production SQL patterns for EHR analytics on Meditech Paragon: wRVU productivity, SDOH, sepsis, 340B.

---

### Stack

`Python` `SQL` `TypeScript` `scikit-learn` `XGBoost` `LightGBM` `Optuna` `statsmodels` `pandas` `DuckDB` `dbt` `FastAPI` `Streamlit` `Next.js` `PostgreSQL` `Prisma` `pytest` `GitHub Actions` `Docker` `Tableau`

---

### Background

- **Founder & Principal, CGC Labs** (2026–present) — the outsourced business analyst rural and critical access hospitals can't staff, on retainer: audit-ready CMS, HCAHPS, and MBQIP reporting, KPI governance, and the dashboards a small hospital would build in-house if it could afford the seat.
- **BI Analyst** (4 years) — clinical and operational analytics at a critical access hospital on Paragon: physician productivity, clinical quality (SDOH, sepsis, readmissions), 340B compliance, Tableau dashboards, and the BI-side data transformation on a Veradigm-to-Paragon EMR migration alongside Altera.
- **MBA + M.S. Data Science**, Eastern University (expected 2027).
- **Previously —** manufacturing and law enforcement: learned to find signal in noisy data and explain it to people who need a decision, not a model card.

---

[Portfolio](https://christiangcallahan.tech) · [LinkedIn](https://www.linkedin.com/in/christiangcallahan/) · [Email](mailto:Christian.G.Callahan@gmail.com)
