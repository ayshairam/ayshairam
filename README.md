<div align="center">

# 👋 Hi, I'm Aysha Iram

### AI & Data Science Engineer • Machine Learning • Computer Vision • NLP • Generative AI

<p>
  <a href="https://github.com/ayshairam">
    <img src="https://img.shields.io/badge/GitHub-ayshairam-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
  <a href="https://www.linkedin.com/in/aysha-iram-80785a335/">
    <img src="https://img.shields.io/badge/LinkedIn-Aysha%20Iram-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="mailto:ayshairam29@gmail.com">
    <img src="https://img.shields.io/badge/Email-ayshairam29%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/>
  </a>
</p>

<p>
  <img src="https://komarev.com/ghpvc/?username=ayshairam&style=for-the-badge&color=blueviolet" alt="Profile views"/>
</p>

</div>

---

## 👩‍💻 About Me

I am an **Artificial Intelligence & Data Science undergraduate** at Don Bosco Institute of Technology, Bengaluru, focused on building practical machine learning systems that move beyond experimentation into usable, explainable software.

My work spans **Machine Learning, Computer Vision, NLP, Retrieval-Augmented Generation, risk modelling, data engineering, and full-stack AI systems**.

I enjoy working at the intersection of:

- 🤖 Machine Learning & Applied AI
- 👁️ Computer Vision
- 🧠 NLP & Large Language Models
- 🔎 Retrieval-Augmented Generation
- 📊 Data Analytics & Risk Modelling
- 🛡️ Financial Crime & Transaction Monitoring
- ⚙️ Backend & AI System Engineering
- 🧪 Model Evaluation, Ablation & Explainability

I am particularly interested in building AI systems where **the model's prediction is not enough — the system should also be able to explain why it made that decision.**

---

## 🎓 Education

**B.E. — Artificial Intelligence & Data Science**  
**Don Bosco Institute of Technology, Bengaluru — VTU**  
2023 – 2027 | **CGPA: 8.5**

**PCMC — Class XII**  
Scholars PU College, Bengaluru  
**94.5%**

---

# 🚀 Featured Work

## 🛡️ Retail Banking & AML Transaction Monitoring

**Software Developer Trainee — Commonwealth Bank of Australia**

A full-stack retail banking and Anti-Money Laundering transaction monitoring platform designed around configurable risk detection, explainable alerts, auditability, and reliable transaction processing.

### Engineering highlights

- Configurable AML rule engine
- Large transaction detection
- High-frequency transaction detection
- Structuring / threshold-avoidance detection
- Explainable **0–100 risk scoring**
- Correlated AML alerts
- Role-based authentication and authorization
- Idempotent transaction processing
- Transaction rollback handling
- Full audit logging
- Automated unit and integration testing
- MongoDB-backed transaction and alert workflows
- Node.js / Express backend architecture
- React-based frontend

### Repository

🔗 **[Retail Banking & AML Transaction Monitoring](https://github.com/ayshairam/Retail-Banking-AML-Transaction-Monitoring)**

The repository contains configurable AML rules including `LARGE_TRANSACTION`, `HIGH_FREQUENCY`, and `STRUCTURING`, with rules evaluated dynamically rather than hard-coded into application logic. :chatgpt-content-reference{index="1"}

---

# 🧠 Trinetra — AI Bitcoin Transaction Monitoring

**Smart India Hackathon 2026 — Team Sentinels**

Trinetra is an explainable AI-based transaction monitoring system focused on identifying suspicious Bitcoin transaction activity by connecting blockchain and network-level signals.

### Technical approach

- Blockchain transaction analysis
- Wallet/entity resolution
- Network metadata integration
- IP / ASN / timing signals
- Feature engineering across multiple signal families
- XGBoost-based risk ranking
- Explainable alert generation
- SHAP-based per-alert reasoning
- Dense analytical workflows using DuckDB
- FastAPI service architecture
- Offline and reproducible processing
- Ablation testing across feature families
- Precision@k evaluation
- PR-AUC evaluation
- Comparison against a rules-based baseline
- Automated testing

### Engineering focus

Rather than producing only a binary suspicious/not-suspicious output, the system is designed around an **explainable lead queue**, allowing investigators to understand which evidence contributed to an alert.

🎥 **[Watch the Trinetra Demo](https://www.youtube.com/watch?v=2Mnk-9X66tM)**

---

# 👁️ Real-Time Behavioural Surveillance

**Final-Year Project**

A distributed computer-vision pipeline designed for analysing behavioural patterns across multiple CCTV camera feeds.

### Architecture

```text
CCTV / Camera Streams
        │
        ▼
      Kafka
        │
        ▼
Spark Structured Streaming
        │
        ├──────────────► YOLOv8n
        │                 Object Detection
        │
        └──────────────► MediaPipe BlazePose
                          33 Pose Keypoints
                                │
                                ▼
                         Pose Sequences
                                │
                                ▼
                         2-Layer LSTM
                                │
                                ▼
                     Behaviour Classification
