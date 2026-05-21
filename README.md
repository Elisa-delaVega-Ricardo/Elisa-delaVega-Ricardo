<h1 align="center">Elisa de la Vega Ricardo</h1>

<p align="center">
  <strong>Founder & Lead Data Scientist · Ricardo Data & AI Consulting, LLC</strong><br>
  <em>M.S. Data Science — University of Virginia (Dec 2025)</em><br>
  <em>B.A. Data Analytics — University of Richmond (May 2023)</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white"/>
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white"/>
</p>

---

## About Ricardo Data & AI Consulting, LLC

I build production-grade machine learning systems for service businesses in the Greater Richmond, Virginia area — med spas, dental practices, HVAC contractors, and other operations-heavy industries. My work focuses on three things business owners actually pay for: **more leads converted**, **fewer no-shows**, and **higher customer retention**.

Every platform I build is a research-backed, deployable application — not a slide deck. Models are validated on held-out test sets, tuned for the business cost asymmetry of the problem, and shipped as live web apps that decision-makers can actually use.

---

## Featured Projects

### 🦷 Bright Smile Dental — AI Operations Platform
**Live demo:** [bright-smile-dental.streamlit.app](https://bright-smile-dental.streamlit.app)
**Repo:** [Bright-Smile-Dental-AI-Operations-Platform](https://github.com/Elisa-delaVega-Ricardo/Bright-Smile-Dental-AI-Operations-Platform)

Three production ML models solving the most expensive operational problems in dentistry:

| Model | Algorithm | AUC | Problem Solved |
|---|---|---|---|
| Lead Scoring | Random Forest (best of LR / RF / GB) | 0.833 | Convert new-patient inquiries faster |
| No-Show Risk | Random Forest (class-balanced) | 0.733 | Recover the $105K/yr lost to no-shows |
| Treatment Acceptance | Gradient Boosting | 0.675 | Lift case acceptance above 61% national average |

Built with: Python · scikit-learn · Streamlit · Plotly · synthetic data generation matched to industry benchmarks (CertifyHealth, Henry Schein, Pankey Institute, Overjet).

---

### ❄️ Comfort Pro HVAC of Richmond — AI Operations Platform
**Live demo:** [comfort-pro-hvac.streamlit.app](https://comfort-pro-hvac.streamlit.app)
**Repo:** [comfort-pro-hvac](https://github.com/Elisa-delaVega-Ricardo/comfort-pro-hvac)

Targets the three ROI killers documented by CallCap, FieldEdge, and ACCA: missed calls, low booking rates, and maintenance agreement churn. Service area: Richmond City, Henrico, Chesterfield, Hanover, Petersburg, and Fredericksburg.

| Model | Algorithm | AUC | Problem Solved |
|---|---|---|---|
| Lead Scoring | Logistic Regression (best of LR / RF / GB) | 0.899 | Prioritize high-intent calls in real time |
| Missed-Call Recovery | Random Forest (class-balanced) | 0.770 | Recover the 25-70% of inbound calls competitors capture today |
| Membership Churn | Gradient Boosting | 0.752 | Hold renewal rates above the 70-80% industry target |

Threshold-tuned for asymmetric business cost — a missed install lead is worth more than 20,000 unnecessary recovery texts.

---

### ✨ Glow Aesthetics VA — Med Spa Lead Scoring Platform
**Live demo:** [glow-aesthetics-va.streamlit.app](https://glow-aesthetics-va.streamlit.app)
**Repo:** [glow-aesthetics-va](https://github.com/Elisa-delaVega-Ricardo/glow-aesthetics-va)

ML-powered lead scoring for med spas — the highest-revenue, lowest-competition niche identified in my market analysis (8.6/10 opportunity score). Trained on 2,000 synthetic treatment inquiries calibrated to American Med Spa Association benchmarks. Predicts which Botox, laser, and body contouring leads will convert before staff invests time.

Built with: Python · scikit-learn (Gradient Boosting) · Streamlit · Plotly.

---

### 🔍 First RAG System — Build From Scratch
**Repo:** [project-1-first-rag-system](https://github.com/Elisa-delaVega-Ricardo/project-1-first-rag-system)

A complete Retrieval-Augmented Generation pipeline implemented from first principles — no LangChain, no LlamaIndex, no black boxes. TF-IDF embeddings are implemented manually in NumPy; cosine similarity search is implemented from scratch before offering a FAISS alternative.

**Retrieval Performance (TF-IDF baseline):**
- Hit Rate (Top-1): **75.0%**
- Avg Precision@5: **22.5%**
- Vocabulary: 540 terms after stop-word removal

Includes hyperparameter sensitivity analysis across 5 chunk sizes, three chunking strategies (fixed / sentence / recursive), and a full evaluation harness with Precision@K, Recall@K, MRR, and Hit Rate. Built to make the RAG mechanics legible before reaching for abstractions.

---

## What I Bring

**Machine Learning** — End-to-end pipelines from feature engineering through evaluation. Classification, regression, time-series, churn modeling. Comfortable with class imbalance, threshold tuning, and the cost-asymmetry decisions that matter in production.

**Statistical Modeling** — Hypothesis testing (t-tests, ANOVA, chi-square), regression (linear, logistic, multinomial), Bayesian inference (Stan, ADVI), survival analysis. Every analysis answers a real business or policy question — not just produces numbers.

**Information Retrieval & NLP** — TF-IDF and dense embeddings from scratch, vector indexing with FAISS, retrieval evaluation, RAG pipeline design.

**Data Engineering** — Reproducible ETL workflows, messy real-world dataset wrangling, synthetic data generation calibrated to industry benchmarks.

**Communication** — Plain-English translation of model choices, computational cost, and business tradeoffs. Stakeholders can defend my work in their own meetings without me in the room.

---

## Technical Stack
