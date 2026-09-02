# Christian Callahan

**Business Intelligence Analyst — executive dashboards that show VPs and the C-suite where the problem is.**

I build the executive view: the few numbers leadership acts on, one agreed definition behind each, and the drill from a red flag to the department, the driver, and the date. Four years as the BI analyst inside a rural critical access hospital, where that view moved patient satisfaction 22 points, took the facility to its first 75th-percentile HCAHPS ranking, and replaced a $150,000 vendor dashboard implementation.

**The discipline underneath:** one definition per metric, real baselines, calibration, stated limitations, and every number reproducible from a clean clone. A dashboard no one opens is a cost.

**Now —** Founder & Principal at [CGC Labs](https://cgclabs.org). Direct engagements, and available to consulting firms as a subcontractor on BI and dashboard workstreams (white-label, NDA/MSA/IC in place, HIPAA and PHI insured).

---

### Featured Projects

**[ED Operations Analytics](https://github.com/CCallahan308/ed-operations-scotland)** — Site-level forecasting of NHS Scotland A&E 4-hour compliance on real Public Health Scotland open data (7,022 Type-1 site-months, 2007–2026), shipped as a deployed Streamlit dashboard. Chronological split, frozen config, holdout scored exactly once; a DuckDB star schema reconciled row-for-row to the Python pipeline. Gradient-boosted + persistence ensemble hits 2.72 pp holdout MAE against a 2.87 pp persistence baseline, but the paired-bootstrap 95% CI on that improvement includes zero, and the README leads with that rather than the win. 111 tests, CI on 3.11/3.12.

**[Rural Hospital Closure Risk](https://github.com/CCallahan308/rural-hospital-distress)** — Master's capstone, published as a [static executive report](https://ccallahan308.github.io/rural-hospital-distress/): 1–2 year closure/conversion risk for US rural hospitals from public CMS cost reports alone. 89,912 hospital-years (1997–2021) containing 133 closures (0.148% base rate). XGBoost, discrete-time hazard, and logistic models with forward-chaining temporal CV, isotonic calibration, SHAP, and a 10-check leakage audit. Hold-out 2019–2021: AUROC 0.867 with 43.7× lift; 3 of the 6 real closures rank in the top 1.2% of scores. The central finding is a defect story: an in-sample calibration bug collapsed scores to ~0 for 11,759 of 11,760 hold-out rows, a false negative previously blamed on COVID relief funding. Finding and fixing it restored the ranking. 156 tests.

**[A/B Test & Experimentation Analyzer](https://github.com/CCallahan308/ab-test-analyzer)** — A decision engine that returns ship / hold / iterate / kill, not a p-value: power against a pre-specified minimum worthwhile effect, CIs, Cohen's h, and a sample-ratio-mismatch check on every result; exploratory segments with Holm correction. On the canonical Udacity experiment (290,584 users) it returns an honest, well-powered null (p=0.19 with >99% power to detect the 1pp effect worth shipping) and explains why that is a decision, not a failure. Every README figure regenerates via `scripts/compute_findings.py`; all 16 analytical choices documented in `ASSUMPTIONS.md`. 37 tests.

**[Churn ROI Simulator](https://github.com/CCallahan308/churn-roi-simulator)** — Event-log churn scoring turned into a retention-budget decision on 2.76M RetailRocket events: what a churn model is actually worth to a VP when the base rate caps the achievable lift. [Live demo →](https://saas-churn-simulator-ccallahan308.streamlit.app/)

**[SignalForge](https://github.com/CCallahan308/signalforge)** — Churn modeling on IBM Telco with statistical rigor: Optuna tuning, leakage-free CV, bootstrap 95% CIs, paired t-tests, calibration. The three models land within ~0.003 AUC with overlapping confidence intervals, so model choice is a calibration and interpretability call, not an accuracy race.

**[Ticket Intel](https://github.com/CCallahan308/ticket-intel)** — Support-ticket routing and summarization on Banking77 using TF-IDF + Naive Bayes by design: fast, interpretable, with a documented rationale for not using an LLM. [Live demo →](https://ticket-intel-ccallahan308.streamlit.app/)

---

### Also

- **[Pit Wall Intelligence](https://github.com/CCallahan308/pit-wall-intelligence)** — F1 race strategy: FastF1 → DuckDB + dbt warehouse, calibrated LightGBM undercut classifier, Monte Carlo race simulator, pit-cost calculator across 33 circuits.
- **[AutoModeler](https://github.com/CCallahan308/automodeler)** — Type a ticker, get a fully-linked 3-statement Excel model with native formulas. FMP API · FastAPI · Python.
- **[Ecommerce Retention & Growth](https://github.com/CCallahan308/ecommerce-retention-growth)** — LTV segmentation and win-back budget sizing on KKBox data, with a synthetic generator so it runs cold.

---

### Stack

`SQL` `Tableau` `Python` `Streamlit` `Excel` `DuckDB` `dbt` `PostgreSQL` `pandas` `TypeScript` `Next.js` `FastAPI` `scikit-learn` `XGBoost` `LightGBM` `Optuna` `statsmodels` `Prisma` `pytest` `GitHub Actions` `Docker`

---

### Background

- **Founder & Principal, CGC Labs** (2026–present) — executive dashboards and the analysis behind them: one view per audience, one agreed definition per number (KPI governance via MeasureMap), audit-ready CMS, HCAHPS, and MBQIP reporting. Direct retainers, and subcontract BI delivery for consulting firms.
- **BI Analyst** (4 years) — owned the BI function at a critical access hospital on Paragon: executive and board dashboards in Tableau, clinical and operational analytics (physician productivity, SDOH, sepsis, readmissions), 340B compliance, 200+ automated reports and submissions with zero missed deadlines, and the BI-side data transformation on a Veradigm-to-Paragon EMR migration alongside Altera.
- **MBA + M.S. Data Science**, Eastern University (expected 2027).
- **Previously —** manufacturing and law enforcement: learned to find signal in noisy data and explain it to people who need a decision, not a model card.

---

[Portfolio](https://christiangcallahan.tech) · [CGC Labs](https://cgclabs.org) · [LinkedIn](https://www.linkedin.com/in/christiangcallahan/) · [Email](mailto:Christian.G.Callahan@gmail.com)
