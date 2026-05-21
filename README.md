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

<details>
<summary><strong>📖 What this means for a dental practice (plain English)</strong></summary>

This platform is a smart assistant that runs quietly in the background of a dental practice and answers three questions every front-desk team struggles with every single day:

**1. "Which new patient calls are worth dropping everything for?"**
The Lead Scoring model looks at every inquiry — phone call, web form, referral — and instantly rates it 0 to 100. A score of 85 means "this person is very likely to book and become a real patient." A score of 15 means "this is just price-shopping, don't burn 20 minutes on them." The model is right roughly 8 times out of 10. That lets the front desk stop treating every call the same and pour their attention into the inquiries that actually become revenue.

**2. "Which of tomorrow's appointments is going to no-show?"**
Around 1 in 10 dental appointments end in a no-show, which costs the average practice over $105,000 a year in lost chair time. The No-Show Risk model looks at each scheduled appointment 48 hours out and flags the ones most likely to ghost — based on the patient's history, how far in advance they booked, whether they confirmed, the weather, and other patterns. The team can then call those high-risk patients personally (instead of just sending another text), or double-book the slot. Even saving 2 no-shows per week is roughly $40,000 a year recovered.

**3. "Which treatment plans is the patient about to walk out without accepting?"**
Nationally, only 61% of dental treatment plans get accepted, and that number drops sharply when the bill goes over $3,000. The Treatment Acceptance model predicts — before the patient leaves the chair — whether they are likely to say yes. If the answer is "probably no," the system tells the team exactly what to do: bring in the treatment coordinator, offer CareCredit financing, phase the work across two insurance years, or address the patient's anxiety. Acting on those signals lifts acceptance rates well above the national average.

**What it costs and what it earns.** The whole system runs on a $5–20/month server, trains in under a minute, and responds in milliseconds. It pays for itself in the first week if it prevents even 2 or 3 no-shows per month. No GPU, no enterprise software, no IT department needed.

</details>
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

<details>
<summary><strong>📖 What this means for an HVAC contractor (plain English)</strong></summary>

This platform is a 24/7 digital dispatcher that runs alongside the office team and answers three questions that decide whether an HVAC business is growing or leaking cash:

**1. "Which call should we answer first when the phones are blowing up?"**
On a 95-degree July day in Richmond, an HVAC office can get 30 calls in an hour. The team cannot answer them all. The Lead Scoring model rates every inbound call 0 to 100 in real time — based on what the caller needs, where they are, whether they are a repeat customer, how old their system is, and a dozen other signals. A Gold member calling about a dying 18-year-old AC scores 94 (drop everything, send the senior tech). Someone price-shopping a tune-up scores 18 (auto-text them pricing and move on). The model is right roughly 9 times out of 10. The team stops treating all calls the same and finally focuses on the calls that pay the bills.

**2. "We just missed a call. Is that lead already gone to a competitor, or can we still save it?"**
Industry data is brutal: HVAC contractors miss 25-40% of inbound calls on average, and up to 70% during peak season. 80% of those callers never leave a voicemail. 78% of them call the next company on the list. Once they book the competitor, they are gone forever. The Missed-Call Recovery model scores every missed call the second it happens and tells the team where to focus: "This $8,500 AC replacement lead has a 60% chance of being recoverable if you text them in the next 60 seconds — go." Or: "This one called at 10pm Saturday and waited 30 minutes; they already booked someone else, send a polite follow-up and move on." Recovering even 2 of those calls a week at a $4,200 average margin is roughly $400K/year back in the business.

**3. "Which maintenance members are about to cancel — and what should we do about it?"**
Service agreements are the most profitable line in an HVAC business. According to the Air Conditioning Contractors of America, contractors with active maintenance programs see 60-80% customer retention; those without see only 20-30%. Every $1 of agreement revenue brings $2 of additional repair and replacement work. The Membership Churn model looks at every member 90 days before renewal and flags the ones at risk — based on whether they completed their tune-ups, how long since anyone called them, their satisfaction scores, and whether they are on auto-pay. Then it tells the team exactly what to do: "Call this Gold member personally — they missed both visits and have not heard from us in 200 days. Schedule the overdue tune-up before sending the renewal." The #1 churn driver (per Oxmaint 2026) is missed visits. This model catches it before the customer cancels.

**The Richmond math that closes the sale.** A typical contractor doing 100 inbound calls/month at a $350 average ticket and the industry-average 46% booking rate makes $193,200 a year on those calls. Lifting the booking rate to just 65% — well below the 85% top performers hit — adds **$80,000 a year** with zero extra marketing spend. The platform that delivers this costs $5–20/month to host. The math is not subtle.

</details>
---

### ✨ Glow Aesthetics VA — Med Spa Lead Scoring Platform
**Live demo:** [glow-aesthetics-va.streamlit.app](https://glow-aesthetics-va.streamlit.app)
**Repo:** [glow-aesthetics-va](https://github.com/Elisa-delaVega-Ricardo/glow-aesthetics-va)

ML-powered lead scoring for med spas — the highest-revenue, lowest-competition niche identified in my market analysis (8.6/10 opportunity score). Trained on 2,000 synthetic treatment inquiries calibrated to American Med Spa Association benchmarks. Predicts which Botox, laser, and body contouring leads will convert before staff invests time.

Built with: Python · scikit-learn (Gradient Boosting) · Streamlit · Plotly.

<details>
<summary><strong>📖 What this means for a med spa (plain English)</strong></summary>

This platform is a smart triage system for the front desk at a med spa. It answers the one question that determines whether a Botox practice or aesthetics clinic is profitable: **which inquiries are real money, and which are tire-kickers?**

**The problem every med spa owner knows.** The average med spa generates between $1.4 million and $2 million per location annually, with a customer lifetime value over $6,000. But that revenue is buried in noise. A practice can receive 100 inquiries a week through Instagram, Facebook ads, website forms, and walk-ins — and the front desk has no way to tell which ones are serious. A Botox regular ready to book today gets the same generic reply as someone who saw a discount ad and is comparing five practices. By the time staff figures out who is serious, the high-value lead booked somewhere else.

**What the model does.** Every inquiry gets a score from 0 to 100, instantly, the second it arrives:

- A returning client asking about laser hair removal scores 90+. Recommended action: call them within 5 minutes, book the appointment today, mention the loyalty discount.
- A new lead from Instagram asking about a Botox special scores 55. Recommended action: send a personalized text with pricing, schedule a free consultation within 48 hours.
- A cold lead with a generic "what do you offer?" message scores 18. Recommended action: auto-respond with a brochure link, add to the monthly newsletter, do not tie up staff time.

The result is a front desk that stops wasting hours on inquiries that will never convert and pours their attention into the leads that turn into $500 Botox appointments, $3,000 laser packages, and $6,000+ body contouring journeys.

**Why this niche specifically.** My market analysis identified med spas as the highest-scoring niche on my opportunity matrix (8.6/10) for one reason: extremely high revenue per customer combined with almost zero competition from data science providers. Most med spas rely on generic marketing agencies running ads, with no analytics layer underneath. There is no software anywhere in the industry that does what this platform does — predict, in real time, which Botox inquiry is worth the staff's next 10 minutes.

**The economics.** The platform runs on a $5–20/month server. A single high-value treatment package recovered per month — one client who would have otherwise been ignored — pays for the system for the year. Most practices that adopt lead scoring see meaningful lift in their conversion rate within the first 30 days, simply because the team is finally responding to the right people first.

</details>
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

```
Languages        Python · R · SQL
ML / DL          scikit-learn · XGBoost · LightGBM · PyTorch · TensorFlow / Keras
NLP / RAG        TF-IDF (from scratch) · sentence-transformers · FAISS
Data & Viz       pandas · NumPy · SciPy · matplotlib · seaborn · Plotly · Tableau · Power BI
Deployment       Streamlit · Streamlit Cloud · joblib · FastAPI · Docker
Statistical      Bayesian Inference (Stan, ADVI) · Hypothesis Testing · Survival Analysis
Engineering      Git · GitHub · Linux / Bash · REST APIs
```

---

## Earlier Work

| Project | Focus |
|---|---|
| [Henrico County Education Analytics](https://github.com/Elisa-delaVega-Ricardo/henrico-education-analytics) | 8 years of Virginia SOL data — trend analysis, equity gap assessment, COVID impact modeling |
| Enhancing Remote Therapy with Facial Expression Recognition (FACEMINE) | Real-time computer vision for telehealth, built with PyTorch |

---

## Education

**M.S. Data Science** — University of Virginia *(Dec 2025)*
Coursework: Deep Learning · Bayesian Machine Learning · Scalable Data Engineering · Statistical Modeling

**B.A. Data Analytics** — University of Richmond *(May 2023)*

---

## Let's Connect

I work with service businesses in the Greater Richmond, VA area on lead scoring, no-show prediction, churn modeling, and operations analytics. If your business sees more than 50 leads or appointments per week and your team is reacting instead of predicting, I can help.

<p align="center">
  <a href="https://www.linkedin.com/in/elisa-delavega-ricardo">LinkedIn</a> ·
  <a href="mailto:elisadelavegaricardo@gmail.com">Email</a> ·
  <a href="https://github.com/Elisa-delaVega-Ricardo">GitHub</a>
</p>

<p align="center">
  <em>Ricardo Data & AI Consulting, LLC · Richmond, Virginia</em>
</p>
