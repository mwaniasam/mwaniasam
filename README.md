# Samuel Mwania

**Software Engineer · Machine Learning & Data Systems**

I build machine learning and data systems that turn real-world problems into deployable software: model, API, container, deployment, load test, retraining path. Seven built, two answering live requests in production.

BSc Software Engineering (Machine Learning), African Leadership University · Completing December 2026, graduation ceremony June 2027 · Based in Kenya

Open to internships, graduate roles, research opportunities and full-time roles. Internships and project-based work now, full-time from January 2027.

**[Portfolio](https://www.mwaaniasam.com)** · **[Resume](https://docs.google.com/document/d/1P5MNIAe3ejL193irf26fcbxkm3EahZN5T39hx1_UtCg/view)** · **[LinkedIn](https://www.linkedin.com/in/samuel-mwania-73sa17)** · **[Email](mailto:mwaaniasamuel@gmail.com)**

---

## Selected work

| Project | What it is | Result | Evidence |
|---|---|---|---|
| **Maize Yield Prediction** | Random Forest regression API and Flutter app for Nigerian smallholder farms | Live on Render. R² 0.2372 against a mean-predictor baseline; the limitations are documented | [Source](https://github.com/mwaniasam/ML-MobileApp_Linear-regression) · [Live API](https://ml-mobileapp-linear-regression.onrender.com/docs) |
| **CoffeeGuard** | Coffee leaf disease classifier: MobileNetV2, FastAPI, Streamlit, Docker, Locust | 98.80% accuracy, 98.36% macro F1 on 58,549 images; zero failed requests at 50 concurrent users | [Source](https://github.com/mwaniasam/MLOPs_summative) · [Live](https://coffeeguard-hwhq.onrender.com) |
| **Multilingual Health QA** | Health question answering in five African languages: dense retrieval with per-language answer selection | **Zindi final rank 17th of 1,651.** Public score 0.6908, 41% above the TF-IDF baseline, 44 logged experiments | [Source](https://github.com/mwaniasam/multilingual-health-qa) |
| **AegisVeritas** | Graph-based screening platform, the production system behind my capstone research | In development | See below |
| **Freeway DQN** | Controlled 30-experiment study of DQN hyperparameters, team of three | Discount factor 0.90 beat the conventional 0.99 | [Source](https://github.com/kelvintawe12/Freeway-DQN_formative3) |

More: [Milan traffic forecasting](https://github.com/mwaniasam/time-series_forecasting) (5GB telemetry; LSTM and TCN against a SARIMA baseline) · [Synapse](https://github.com/mwaniasam/synapse-platform) (adaptive learning platform, Next.js and PostgreSQL) · [MoMo Analyst](https://github.com/Bonaparte003/Momo-Data_Analyst) (mobile money analytics; I built the data pipeline)

---

## Research and AegisVeritas

**Uncovering Hidden Supplier Links in Kenyan Public Procurement: A Graph-Based Machine Learning Approach** · Capstone, September to November 2026

Procurement research → graph machine learning → AegisVeritas → production screening system.

- **Problem:** supplier screening matches bidders by name against debarment and sanctions lists. A debarred party can return through a related company with an unrelated name.
- **Question:** can relational structure in public procurement and ownership records identify exposure that name-based screening misses, and do learned graph representations stay effective on a real Kenyan graph?
- **Approach:** an ownership, directorship and contract award graph built from public records, scored with a graph attention network. It is compared against a deterministic baseline, conventional machine learning, and engineered graph features with a tree ensemble. Evaluation uses entity-disjoint splits, ten seeds, ablation and permutation testing.
- **AegisVeritas, built so far:** GNN risk scoring with a heuristic fallback for sparse subgraphs, five API endpoints with hash-chained audit logging, timing-equalised authentication, and 164+ passing automated tests.
  - **Stack:** FastAPI, async SQLAlchemy 2.0, Neo4j, PyTorch Geometric, Argon2id, Next.js.
- **Status:** in progress. Results will be published when the evaluation is done.

---

## Skills

- **Machine learning:** PyTorch, TensorFlow / Keras, scikit-learn, Hugging Face Transformers, FAISS, LoRA, Stable Baselines3
- **Data:** Python, pandas, NumPy, PyArrow, PostgreSQL, MySQL, SQLite
- **Backend and APIs:** FastAPI, Pydantic, SQLAlchemy 2.0 async, Flask, REST API design
- **ML systems:** Docker, CUDA and GPU training, model serving, load testing with Locust
- **Graph:** Neo4j, PyTorch Geometric, graph attention networks, entity resolution
- **Engineering:** Linux, Git, TypeScript, Next.js, React, Flutter

---

## Interests

Graph machine learning · entity resolution · risk analytics · AI for public-sector and financial systems · low-resource African language NLP
