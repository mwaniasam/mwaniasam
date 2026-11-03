# Samuel Mwania

**Software Engineer · Machine Learning & Data Systems**

I build machine learning and data systems that turn real-world problems into deployable software: model, API, container, deployment, load test, retraining path. Seven built, two answering live requests in production.

BSc Software Engineering (Machine Learning), African Leadership University · Completing December 2026, graduation ceremony June 2027 · Based in Kenya

Open to internships, graduate roles, research opportunities and full-time roles. Internships and project-based work now, full-time from January 2027.

**[Portfolio](https://www.mwaaniasam.com)** · **[Resume (PDF)](https://www.mwaaniasam.com/Samuel-Mwania-Resume.pdf)** · **[LinkedIn](https://www.linkedin.com/in/mwaaniasam)** · **[Email](mailto:mwaaniasamuel@gmail.com)**

---

## Selected work

| Project | What it is | Result | Evidence |
|---|---|---|---|
| **AegisVeritas** | Finds bidders in Kenyan public procurement that look independent but are linked to each other or to a debarred party. My capstone | Pre-registered: average precision 0.146 against 0.067 for Adamic-Adar in Kenya; AUC 0.85 against 0.57 in Estonia; 665 backend tests | [Case study](https://www.mwaaniasam.com/aegisveritas/) · [Walkthrough](https://youtu.be/g4tlftDK7T4) |
| **Maize Yield Prediction** | Random Forest regression API and Flutter app for Nigerian smallholder farms | Live on Render. R² 0.2372 against a mean-predictor baseline; the limitations are documented | [Source](https://github.com/mwaniasam/ML-MobileApp_Linear-regression) · [Live API](https://ml-mobileapp-linear-regression.onrender.com/docs) |
| **CoffeeGuard** | Coffee leaf disease classifier: MobileNetV2, FastAPI, Streamlit, Docker, Locust | 98.80% accuracy, 98.36% macro F1 on 58,549 images; zero failed requests at 50 concurrent users | [Source](https://github.com/mwaniasam/MLOPs_summative) · [Live](https://coffeeguard-hwhq.onrender.com) |
| **Multilingual Health QA** | Health question answering in five African languages: dense retrieval with per-language answer selection | **Zindi final rank 17th of 1,651.** Public score 0.6908, 41% above the TF-IDF baseline, 44 logged experiments | [Case study](https://www.mwaaniasam.com/health-qa/) · [Source](https://github.com/mwaniasam/multilingual-health-qa) |
| **Freeway DQN** | Controlled 30-experiment study of DQN hyperparameters, team of three | Discount factor 0.90 beat the conventional 0.99 | [Source](https://github.com/kelvintawe12/Freeway-DQN_formative3) |

More: [Milan traffic forecasting](https://github.com/mwaniasam/time-series_forecasting) (5GB telemetry; LSTM and TCN against a SARIMA baseline) · [Synapse](https://github.com/mwaniasam/synapse-platform) (adaptive learning platform, Next.js and PostgreSQL) · [MoMo Analyst](https://github.com/Bonaparte003/Momo-Data_Analyst) (mobile money analytics; I built the data pipeline)

---

## Experience

**Data Engineer Intern, Hello Tractor** · Nairobi · April to August 2025

Agritech platform connecting smallholder farmers with tractor owners across Africa. Prepared and audited datasets for reporting, and supported batch prediction runs.

---

## Research and AegisVeritas

**Uncovering Hidden Supplier Links in Kenyan Public Procurement: A Graph-Based Machine Learning Approach** · Capstone, 2026 · Supervisor: Kevin Sebineza

**[Read the AegisVeritas case study →](https://www.mwaaniasam.com/aegisveritas/)**

- **Problem:** supplier screening matches bidders by name against debarment and sanctions lists. A debarred party can return through a related company with an unrelated name, and two "competing" bidders can share one owner.
- **What changed:** the proposal's graph neural network did not beat a size-only baseline on the 18 confirmed Kenyan cases. So the question became "are these two firms under one control?", where Kenyan awards disclose 12,441 ownership links to learn from.
- **Method:** supplier pairs scored from three kinds of evidence (shared owners or directors, shared contacts, and award behaviour from LightGBM with isotonic calibration), combined Fellegi-Sunter style so every flag keeps its reasons.
- **Results:**
  - Kenya, 7,884 held-back pairs (pre-registered): average precision 0.146 against 0.067 for Adamic-Adar; 25 of the top 100 flags are real links.
  - Estonia, firms the model never saw (pre-registered): AUC 0.85 against 0.57, checked against Estonia's open ownership register.
  - KeRRA contractor registers, which the model never saw (corroboration run after the detector was built, not pre-registered): owner-linked pairs share a P.O. Box 209.9 times more often than same-buyer controls (p = 1.0e-42), and 118.6 times more often than random pairs from the same region.
  - Two tests failed, and are reported in full. Every number was rerun on a clean database after submission.
- **System:** FastAPI, PostgreSQL with row-level security, Neo4j, Celery and Redis, a Next.js app and a SHA-256 hash-chained audit log. 665 backend tests, and 80 of 80 browser tests across Chromium, Firefox and WebKit. Not on the open internet: invited evaluators reach it through Cloudflare Access, and a person always decides.
- **Now:** expert evaluation, with practitioners completing guided tasks in the app and a usability questionnaire (ALU ethics approval SEPT26-BEL-070). [Technical report (PDF)](https://www.mwaaniasam.com/aegisveritas/AegisVeritas_Technical_Report.pdf).

---

## Skills

- **Machine learning:** PyTorch, TensorFlow / Keras, scikit-learn, Hugging Face Transformers, FAISS, LoRA, Stable Baselines3
- **Data:** Python, pandas, NumPy, PyArrow, PostgreSQL, MySQL, SQLite
- **Backend and APIs:** FastAPI, Pydantic, SQLAlchemy 2.0 async, Flask, REST API design
- **ML systems:** Docker, CUDA and GPU training, model serving, load testing with Locust
- **Graph and record linkage:** Neo4j, Fellegi-Sunter record linkage, LightGBM, PyTorch Geometric, entity resolution
- **Engineering:** Linux, Git, TypeScript, Next.js, React, Flutter

---

## Interests

Graph machine learning · entity resolution · risk analytics · AI for public-sector and financial systems · low-resource African language NLP
