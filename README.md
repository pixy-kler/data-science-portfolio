# Data Science Portfolio — pixy-kler

A collection of my Data Science and Data Analysis projects.
I started my journey in **March 2026** and have since completed two
intensive programs — one in Machine Learning and one in Data Science.

This repository is the entry point to everything I build: educational
projects as the foundation, plus pet projects, Kaggle competitions, and
commercial case studies as they come.

**Legend:** 🏆 Commercial · 🧪 Pet · 🏅 Kaggle · 🎓 Educational

---

## 🏆 Commercial Projects

*In progress — case studies will appear here.*

**Planned format:** problem → approach → result → stack. Code and data
shared where NDA permits; otherwise a detailed case study without
sensitive material.

---

## 🧪 Pet Projects

### [Sber Events Parser](https://github.com/pixy-kler/sber-events-parser)

**Motivation:** As an aspiring Data Scientist, I wanted to attend hackathons and meetups to build my network and gain practical experience. Manually checking the Sber events page was tedious, and their email newsletters were often too generic.

**Problem:** Build an automated system to monitor the website, filter events by personal relevance (AI/ML, online, hackathons), and send notifications only when new, suitable events appear.

**Data:** HTML page with embedded `__NEXT_DATA__` JSON (Next.js), containing 152 `EventPage` objects with dates, tags, and locations.

**Approach:** 
1. **Recon:** Avoided heavy browser automation (Selenium/Playwright) by extracting the raw JSON directly from the `<script id="__NEXT_DATA__">` tag.
2. **Parsing:** Normalized dates, extracted cities from the location strings, and classified events (online/offline) using heuristics.
3. **Scoring & Filtering:** Developed a weighted scoring system (e.g., +5 for Hackathons, +3 for AI/ML topics, -4 for "expert-only" meetups). Filtered out past events.
4. **Delivery:** Generated custom HTML email cards and sent them via SMTP.
5. **State Management:** Saved seen event `slugs` to a JSON file to prevent duplicate emails.

**Results:** A fully automated local Python script (runs via Windows Task Scheduler) that delivers a curated list of relevant events directly to my inbox.

**What I learned:** Deepened my understanding of web scraping beyond basic HTML parsing, practiced modular Python code design (separating parser, filtering, storage, and mailer), and gained experience with SMTP and environment variable security (`.env`).

**Stack:** Python, `requests`, `smtplib`, `python-dotenv`

---

## 🏅 Kaggle & Competitions

*In progress — coming soon.*

**Planned format:** competition → approach → public score / position →
notebook link → what worked and what didn't.

---

## 🎓 Educational Projects (Foundation)

Projects completed during two intensive programs. They form the technical
foundation behind everything else in this portfolio.

### ⭐ Featured

| Project | Type | What it's about | Stack |
| :--- | :--- | :--- | :--- |
| **[DSB8 — A/B Test of the Newsfeed (SQL)](https://github.com/pixy-kler/dsb8-sql-ab-test)** | 🎓 DS Intensive, Module 8 | Product hypothesis → SQL → datamart → A/B test on real platform data | sqlite3, pandas, SQL |
| **[DSB12 — Nutritionist: from Notebook to CLI](https://github.com/pixy-kler/dsb12-nutritionist-cli)** | 🎓 DS Intensive, Module 12 | Notebook → module → CLI + external nutrition API + bonus daily-menu generator | scikit-learn, `requests`, OOP |
| **[ml5-trees-gbdt — Decision Trees and GBDT from Scratch](https://github.com/pixy-kler/ml5-trees-gbdt)** | 🎓 ML Course, Module 5 | `Node`, `DecisionTree`, `RandomForest`, `GBDT` on NumPy + comparison with LightGBM, CatBoost, XGBoost | NumPy, scikit-learn, LightGBM, CatBoost, XGBoost |

### Second Tier

| Project | Type | What it's about | Stack |
| :--- | :--- | :--- | :--- |
| **[DSB6 — MovieLens: Module + PyTest](https://github.com/pixy-kler/dsb6-movielens-analytic)** | 🎓 DSB, Module 6 | 4 OOP classes, full PyTest suite, interactive Q&A report | OOP, PyTest, pandas |
| **[DSB9 — Data Visualization: 9 Chart Types](./dsb9-dataviz)** | 🎓 DS Intensive, Module 9 | Line, bar, histogram, boxplot, scatter matrix, heatmap, Seaborn, Plotly animation | Matplotlib, Seaborn, Plotly, sqlite3 |
| **[DSB11 — Regularization, GridSearch, Ensembles, Pipelines](./dsb11-ml-toolkit)** | 🎓 DS Intensive, Module 11 | L1/L2, GridSearchCV, metrics (P/R/F1, ROC-AUC), Voting/Bagging/Stacking, OOP + `Pipeline` | scikit-learn, pandas |
| **[ml3 — Validation and Feature Selection](./ml3-validation-feature-selection)** | 🎓 ML Course, Module 3 | Custom CV schemes, Lasso, permutation importance, SHAP, Grid/Random/Optuna | scikit-learn, SHAP, Optuna |
| **[DSB10 — Classifiers, SVM, Clustering](./dsb10-classifiers-clustering)** | 🎓 DS Intensive, Module 10 | Binary/multiclass classification, SVM decision boundaries, cross-validation, unsupervised clustering | scikit-learn |

### Learning Log

The exercises behind the foundation — Python basics, OOP, Shell/CLI,
Pandas, ML fundamentals — live in a single archive repository:

→ **[learning-exercises](https://github.com/pixy-kler/learning-exercises) — DSB1–DSB7, ml1, ml2, ml4**

---

## 🛠 Tech Stack

**Languages:** Python, SQL

**Data:** Pandas, NumPy, sqlite3, `requests`

**Visualization:** Matplotlib, Seaborn, Plotly

**ML:** scikit-learn, LightGBM, CatBoost, XGBoost

**Engineering:** OOP, PyTest, `Pipeline`, `category_encoders`

**Methodology:** Cross-validation, feature engineering, SHAP, Optuna,
A/B testing

---

## 📫 Get in Touch

- GitHub: [@pixy-kler](https://github.com/pixy-kler)
- 📧 [pixynimble@gmail.com](mailto:pixynimble@gmail.com)
