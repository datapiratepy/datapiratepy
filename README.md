# Harsh Kamat

**Final-year Computer Science Engineering student. I build AI-powered software in Python — retrieval systems, machine-learning workflows, and the APIs and tests around them.**

Bengaluru, India · [Portfolio](https://harshkamat.vercel.app) · [LinkedIn](https://www.linkedin.com/in/harshkamat/) · harshkamat.2307@gmail.com

---

## Featured Work

- **[NutriMind AI](https://github.com/datapiratepy/NutriMind-AI)** — RAG assistant on IBM watsonx.ai
- **[Redrob Ranker](https://github.com/datapiratepy/redrob-ranker)** — deterministic candidate ranking
- **[Customer Churn Analysis](https://github.com/datapiratepy/customer-churn-analysis)** — churn classification + Power BI
- **[Financial Markets Analytics](https://github.com/datapiratepy/financial-markets-analytics)** — Monte Carlo optimization
- **[Climate & Energy Analytics](https://github.com/datapiratepy/climate-energy-analytics)** — SQL on BigQuery

---

## About

Final-year B.E. Computer Science Engineering student in Bengaluru. My work sits at the application layer of AI: taking language models, retrieval and classical ML, and building software around them that can be tested, explained and re-run.

Most of what I build is deliberately boring in the right places. Citations are constructed in code rather than generated, so a model cannot invent a source. Ranking logic is deterministic, so the same input produces byte-identical output. I would rather ship something a reviewer can verify than something that demos well once.

IBM SkillsBuild AI & Cloud intern (2026). Google-certified Data Analyst.

---

## Current focus

- Data structures and algorithms for interviews
- SQL beyond aggregation — joins, window functions, query plans
- ML evaluation: thresholds, imbalance, cross-validation

---

## Technical skills

**Languages** — Python, SQL, JavaScript, HTML/CSS

**AI & LLMs** — IBM watsonx.ai, Granite, RAG, ChromaDB, embeddings, prompt engineering, agent routing

**ML & data** — scikit-learn, Pandas, NumPy, EDA, classification, model evaluation, class imbalance, Monte Carlo

**Backend & quality** — Flask, REST APIs, SQLAlchemy, SSE, pytest, GitHub Actions, Git

**Data & BI** — Google BigQuery, SQLite, Power BI, DAX, Matplotlib, Seaborn

**Web & tools** — Next.js, TypeScript, Tailwind, IBM Cloud, Jupyter, Colab, VS Code

---

## Featured projects

### [NutriMind AI](https://github.com/datapiratepy/NutriMind-AI)

A Flask app on IBM watsonx.ai Granite models that answers nutrition questions from documents you upload. Retrieval is citation-backed: the citation list is assembled in Python from stored metadata, so the model cannot fabricate a source. Built during my IBM SkillsBuild internship, with 156 automated tests at 88% coverage in CI.

`Python` `IBM watsonx.ai` `Granite` `RAG` `ChromaDB` `Flask` `pytest`

### [Redrob Ranker](https://github.com/datapiratepy/redrob-ranker)

Ranks the top 100 of a 100,000-profile pool against a job description, on CPU alone and in under a minute — built for the Redrob × Hack2Skill INDIA.RUNS challenge. Scoring is interpretable and fully deterministic: every placement is explainable from the input, and repeated runs are byte-identical. No machine-learning model in it, by design; embeddings were evaluated and rejected, with the reasoning documented.

`Python` `Algorithm Design` `Feature Engineering` `Deterministic Systems`

### [Customer Churn Analysis](https://github.com/datapiratepy/customer-churn-analysis)

A logistic-regression churn classifier on 7,032 Telco records — cleaning, one-hot encoding, and scaling fitted on the training split only. Class balancing raised churn-class recall from 0.52 to 0.79 at 0.50 precision, a trade made deliberately for a retention use case. Results ship as a Power BI dashboard.

`Python` `scikit-learn` `Pandas` `Power BI` `DAX`

### [Financial Markets Analytics](https://github.com/datapiratepy/financial-markets-analytics)

5,000 Monte Carlo simulations across eight years of AAPL, MSFT, GOOGL and AMZN data (2018–2025, 2,011 trading days), improving the Sharpe ratio from 0.87 to 0.92 and plotting the Efficient Frontier.

`Python` `Pandas` `NumPy` `Matplotlib`

### [Climate & Energy Analytics](https://github.com/datapiratepy/climate-energy-analytics)

SQL analysis of global CO₂ emissions in BigQuery using Our World in Data — filtering, decade aggregation and a scalar subquery for top emitters, with GDP-versus-emissions comparisons in Power BI — a visual comparison, not a computed correlation.

`SQL` `Google BigQuery` `Power BI`

---

## Certifications

- **Google Data Analytics Professional Certificate** — Google / Coursera, 2025
- **IBM SkillsBuild AI & Cloud Internship** — Edunet Foundation with AICTE, 2026
- **Redrob × Hack2Skill INDIA.RUNS Data & AI Challenge** — 2026

## Education

**B.E., Computer Science Engineering** — AMC Engineering College, Bengaluru · 2023–2027

## Open to opportunities

Looking for **AI/ML, Generative AI, Data Science and Python engineering internships**, and **graduate software engineering roles** from 2027. Bengaluru or remote.
