# 🏥 Hospital Discharge Readiness Intelligence Engine

## AI-Based Healthcare Operations Support System

An AI-powered healthcare operations system designed to estimate **operational discharge readiness** and identify **potential workflow blockers** by combining structured hospital data, clinical text, machine learning, explainable AI, and a Gemini-powered chatbot.

> ⚠️ **Important:** This project is an operations-support system, not a clinical decision-making system. It does not diagnose patients, recommend treatment, or independently decide whether a patient should be discharged.

---

## 📌 Project Overview

Hospitals manage large amounts of information across multiple systems. Information relevant to patient discharge may be distributed across:

- Clinical notes
- Laboratory and test results
- Medication information
- Administrative records
- Patient transfers
- Follow-up instructions

Because discharge readiness is not represented by a single field, identifying potential workflow delays can require reviewing multiple sources of information.

The **Hospital Discharge Readiness Intelligence Engine** addresses this problem by combining structured hospital data and clinical text to estimate an **operational discharge readiness score** and identify potential workflow blockers.

The system uses:

- Data preprocessing
- Feature engineering
- Natural Language Processing (NLP)
- Machine Learning
- Probability Calibration
- SHAP Explainable AI
- Gemini API
- Streamlit

---

# 🎯 Problem Statement

Hospitals need to reduce unnecessary delays in patient discharge. However, operational discharge readiness is not always represented by a single field.

Relevant information may exist across:

- Clinical notes
- Test results
- Medication information
- Administrative records
- Follow-up instructions

Therefore, there is a need for an intelligent system that can combine heterogeneous hospital information, estimate operational discharge readiness, identify potential workflow blockers, and provide understandable explanations.

### Proposed Problem Statement

> To develop an AI-based Hospital Discharge Readiness Intelligence Engine that combines structured hospital data and clinical text to estimate operational discharge readiness and identify potential workflow blockers, while providing explainable and human-readable insights through a Gemini-powered chatbot.

---

# 💡 Proposed Solution

The proposed system combines structured hospital information with clinical-text information and applies machine learning to estimate operational discharge readiness.

```text
                    MIMIC-IV
                       │
                       ▼
                Patient Records
                       │
              ┌────────┴────────┐
              │                 │
              ▼                 ▼
      Structured Data       Clinical Text
              │                 │
              ▼                 ▼
      Feature Engineering       NLP
              │                 │
              └────────┬────────┘
                       ▼
                Feature Fusion
                       │
                       ▼
                   ML Model
                       │
                       ▼
          Operational Readiness Score
                       │
                ┌──────┴──────┐
                ▼             ▼
              SHAP        Blocker Signals
                │             │
                └──────┬──────┘
                       ▼
                  Gemini AI
                       │
                       ▼
              Reason Explanation
                       │
                       ▼
                Streamlit App
