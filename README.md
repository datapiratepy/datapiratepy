# Harsh Kamat

**Final-year Computer Science Engineering student building applied AI systems in Python:
retrieval-augmented LLM applications, ML evaluation, and the backend engineering, testing
and deployment around them.**

Bengaluru, India · [Portfolio](https://harshkamat.vercel.app) ·
[LinkedIn](https://www.linkedin.com/in/harshkamat/) · harshkamat.2307@gmail.com

Open to **AI/ML engineering internships**, and to **entry-level roles from 2027**, in applied
and generative AI, retrieval and RAG, and AI backend systems. Bengaluru or remote.

I prefer systems a reviewer can check: citations assembled in code instead of generated,
arithmetic kept out of the model, and results reported together with the checks they failed.

---

## Selected work

### [NutriMind AI](https://github.com/datapiratepy/NutriMind-AI) · RAG application on IBM watsonx.ai

A multi-user nutrition assistant that answers from each user's own PDFs. Citations are
built from stored chunk metadata, requests are routed rule-first to four specialist agents
with a Granite classification fallback, and every number is computed deterministically
rather than by the model. [Live demo](https://nutrimind-ai-0rby.onrender.com).

- **Tested:** 472 automated tests at 91% line coverage. CI runs lint, the suite, migrations
  against a real PostgreSQL server, and a boot check of the production Docker image on
  every push.
- **Multi-user by construction:** per-user isolation enforced down to vector search,
  asynchronous document ingestion, CSRF protection, a nonce-based Content-Security-Policy,
  rate limiting, and account export and deletion.
- **Deployed** on Render in IBM Live mode, with its limits documented: one process by
  design, password-reset links not emailed, no error alerting.

`Python` `Flask` `IBM watsonx.ai` `Granite` `RAG` `ChromaDB` `SQLAlchemy` `PostgreSQL` `Docker` `pytest`

### [VeriQA](https://github.com/datapiratepy/veriqa) · selective question answering · VTU team project

A CPU-only question-answering system that declines to answer when its calibrated risk of
being wrong is too high, built with Harsh Ranjan and Manish Kumar. **My part** was the
extractive reader and the reliability layer: 16 retrieval, reader and cross-passage
agreement signals, a gradient-boosted risk model with isotonic calibration, and the
baselines it is measured against.

- Adding retrieval and agreement signals to a reader-only calibrator raised
  error-prediction ROC-AUC from 0.524 to 0.639 on 3,585 held-out SQuAD 2.0 questions; the
  bootstrap interval for the risk–coverage improvement excludes zero.
- Three of the seven pass/fail gates failed, because the classical (non-transformer)
  reader is weak at 11% base accuracy. The README reports them as failures.
- Re-running the full pipeline from the raw data reproduces every frozen result table
  exactly; only host-dependent latency changes.

`Python` `scikit-learn` `gradient boosting` `isotonic calibration` `SQuAD 2.0` `selective prediction`

### [Redrob Ranker](https://github.com/datapiratepy/redrob-ranker) · deterministic candidate ranking

Ranks the top 100 of 100,000 candidate profiles against a job description, built for the
Redrob × Hack2Skill INDIA.RUNS challenge. Measured at about 40 seconds and 21 MB of peak
memory on CPU, with byte-identical output across runs. There is no ML model, by design:
an embedding layer was evaluated and rejected, and the reasoning is documented.

`Python` `algorithm design` `feature engineering` `deterministic systems`

### Open-source contribution · [Lamatic AgentKit, PR #408](https://github.com/Lamatic/AgentKit/pull/408)

A roster-rules auditor template submitted to Lamatic's open-source AgentKit for the
AgentKit Challenge. LLM nodes transcribe a roster and plain-English scheduling rules; a
deterministic JavaScript evaluator does all the arithmetic, checks every value against the
line it came from, and returns `INCOMPLETE` rather than guessing.
**Status: open pull request under review, not yet merged (September 2026).**

## Earlier data and ML projects

- [Customer Churn Analysis](https://github.com/datapiratepy/customer-churn-analysis):
  logistic-regression churn classifier on 7,032 Telco records. Class balancing raised
  churn recall from 0.52 to 0.79 at 0.50 precision, and the repository documents an
  encoding bug and its fix.
- [Financial Markets Analytics](https://github.com/datapiratepy/financial-markets-analytics):
  Monte Carlo portfolio optimisation under Modern Portfolio Theory for four large-cap
  stocks.
- [Climate & Energy Analytics](https://github.com/datapiratepy/climate-energy-analytics):
  SQL analysis of global CO₂ emissions in Google BigQuery, visualised in Power BI.

## Skills

- **AI and ML:** LLM applications on IBM watsonx.ai (Granite) · RAG, embeddings, ChromaDB ·
  prompt design · scikit-learn: classification, gradient boosting, isotonic calibration ·
  model evaluation
- **Engineering:** Python, SQL, JavaScript · Flask, SQLAlchemy, Alembic, SQLite and
  PostgreSQL · pytest, GitHub Actions, Docker, Git
- **Data:** Pandas, NumPy, Matplotlib, Google BigQuery, Power BI

## Education and credentials

- **B.E., Computer Science and Engineering**, AMC Engineering College (VTU), Bengaluru,
  2023–2027
- **IBM SkillsBuild AI & Cloud internship** (Edunet Foundation with AICTE), 2026:
  NutriMind AI began as its project
- **Google Data Analytics Professional Certificate** (Google / Coursera), 2025
