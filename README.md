# Soham Lodh

**B.Tech CSE (AI & ML) · KIIT University · CGPA 9.31**

Backend-heavy full-stack engineer with a focus on ML systems — from pipeline architecture through production inference. I build things that ship: deployed APIs, live ML endpoints, and multi-role applications with real users.

📍 Kolkata, India · [sohamlodh06@gmail.com](mailto:sohamlodh06@gmail.com) · [LinkedIn](https://linkedin.com/in/soham-lodh) · [Portfolio](https://portfolio-soham-lodh.vercel.app/)

---

## What I Build

End-to-end ML pipelines (feature engineering → model selection → FastAPI inference) and production full-stack systems (MERN, Next.js, TypeScript). I care about correctness under load, clean API contracts, and things that work in production, not just on localhost.

---

## Featured Work

### RiskLens — Credit Default Risk Prediction Platform
`Logistic Regression · Optuna · SMOTETomek · SHAP · FastAPI · React`

[Live](https://credit-default-risklens.vercel.app/) · [GitHub](https://github.com/Soham-Lodh/RiskLens)

An 18-stage ML pipeline on 50,000 records across three relational data sources. Key engineering decisions: stratified splitting before EDA to prevent leakage, VIF-based multicollinearity elimination (5 features dropped), WoE/IV feature selection (10 retained, IV up to 2.38), and SMOTETomek resampling for 10.6% class imbalance. Bayesian optimisation via Optuna (50 trials, TPE sampler) outperformed a tuned XGBoost baseline.

| Metric | Result |
|--------|--------|
| AUC-ROC | **0.9834** |
| Macro F1 | **0.9776** |
| KS Statistic | **85.91** |

Inference served via FastAPI + Uvicorn on Render. Frontend on Vercel with SHAP explainability and a logit-space credit scoring algorithm mapping default probability to a 300–900 institutional risk scale.

---

### PremiumIQ — Health Insurance Premium Predictor
`XGBoost · RandomizedSearchCV · FastAPI · React · Vercel`

[Live](https://premiumiq.vercel.app/) · [GitHub](https://github.com/Soham-Lodh/PremiumIQ)

End-to-end regression pipeline on 9,905 records. Designed a composite `total_risk_score` feature from compound medical history fields to replace high-cardinality categoricals — materially improved model signal. Validated 18 features via VIF (all < 2.5); hybrid ordinal + one-hot encoding pipeline; tuned XGBoost via `RandomizedSearchCV`.

| Metric | Result |
|--------|--------|
| R² Score | **0.9944** |
| vs. Linear Regression baseline | 0.956 |
| vs. Tuned Random Forest | 0.978 |

---

### Prescripto — Medical Appointment Platform
`MERN · JWT · Cloudinary · Vercel`

[Live (Patient)](https://prescripto-o5lf.vercel.app/) · [Live (Admin/Doctor)](https://prescripto-admin-lyart.vercel.app/) · [GitHub](https://github.com/Soham-Lodh/Prescripto)

Production MERN platform across two independently deployed frontends backed by a centralised Express REST API on MongoDB Atlas. Role-based JWT authentication with separate login flows and permission-scoped dashboards for three account types. Appointment scheduling with slot-conflict detection; hardened with input validation, bcrypt hashing, and rate limiting.

---

## Engineering Experience

**Technical Member — Web Development · Coding Ninjas KIIT Chapter** *(Aug 2025 – Present)*

- Architected a full-stack event management platform (Next.js, Hono, Prisma, MongoDB) with a real-time leaderboard handling concurrent score streams from multiple judges; engineered the write pipeline to prevent race conditions under parallel load.
- Built a secure quiz platform with server-side session tracking, tab-switch detection, timed execution, and randomised question delivery.
- Developed a Project Management System with four role levels enforcing access-controlled workflows via middleware; authored API contracts and permission-logic docs for downstream contributors.

**Open Source Contributor · GirlScript Summer of Code** *(Jul – Oct 2025)*

- Implemented authentication modules: OTP login, JWT sessions, Google OAuth, and password recovery — with unit tests across success and failure paths for all four flows.
- Diagnosed and resolved production-level defects by reproducing failure conditions from logs; fixes reviewed and merged into main.

---

## Tech Stack

### Languages
<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black" />
</p>

### ML & Data Science
<p>
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/XGBoost-FF6600?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Optuna-4B8BBE?style=for-the-badge" />
  <img src="https://img.shields.io/badge/SHAP-FF4B4B?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge" />
</p>

### Backend
<p>
  <img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/Hono-E36002?style=for-the-badge&logo=hono&logoColor=white" />
  <img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
</p>

### Frontend
<p>
  <img src="https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" />
</p>

### Databases
<p>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
</p>

### Tools & Deployment
<p>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Render-46E3B7?style=for-the-badge&logo=render&logoColor=black" />
  <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white" />
</p>

---

## Education

**KIIT University** — B.Tech, CSE (AI & ML) · 2024–2028 · CGPA 9.31

*Relevant Coursework: Data Structures & Algorithms, Operating Systems, DBMS, OOP*

---

## Certifications

- Classify Images with TensorFlow on Google Cloud — Google (2025)
- DSA in Python — NPTEL (2025)
- Postman API Student Expert — Postman (2025)

---

## 📊 GitHub Stats

<p align="center">

<img 
src="https://github-readme-stats.shion.dev/api?username=Soham-Lodh&theme=dark&hide_border=false&include_all_commits=true&count_private=false" 
height="180"
/>

<img 
src="https://github-readme-stats.shion.dev/api/top-langs/?username=Soham-Lodh&theme=dark&hide_border=false&include_all_commits=true&count_private=false&layout=compact&card_width=320" 
height="180"
/>

</p>

---

## 🔥 Contribution Streak

<p align="center">

<img 
src="https://streak-stats.demolab.com/?user=Soham-Lodh&theme=dark&hide_border=false" 
height="180"
/>

</p>

---

## 📈 Activity Graph

<p align="center">
  <img 
    src="https://github-readme-activity-graph.vercel.app/graph?username=Soham-Lodh&theme=tokyo-night&hide_border=true" 
  />
</p>

---

## 📅 Profile Summary

<p align="center">
  <img 
    src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Soham-Lodh&theme=tokyonight" 
  />
</p>
