# SentinelLLM
"Autonomous Real-Time Insider Threat &amp; Behavioral Anomaly Detection System with LLM-based Risk Reasoning Agent"

💡 Problem Statement

Enterprises generate massive logs:

Login events

File access events

USB usage

Privilege escalation

Off-hour access

Data download spikes

Goal:

1️⃣ Detect behavioral anomaly in real time
2️⃣ Score insider threat probability
3️⃣ Use LLM to explain why risk is high
4️⃣ Agent decides:

Monitor
Alert
Escalate

SYSTEM ARCHITECTURE (Hybrid AI)

Streaming Log Generator
        ↓
Feature Extractor
        ↓
Behavioral ML Model (Isolation Forest / LSTM Autoencoder)
        ↓
Risk Scoring Engine
        ↓
LLM Reasoning Layer
        ↓
Agentic Decision Orchestrator
        ↓
Alert Dashboard (Deployed on HF Spaces)


TECH STACK
ML Core

Isolation Forest (baseline anomaly detection)

LSTM Autoencoder (advanced time-series anomaly detection)

XGBoost for supervised insider classification

GenAI

Llama 3 / Mistral (via HuggingFace Inference API)

Prompt-based risk explanation

Agentic Layer

Rule + LLM hybrid orchestration

Risk severity decision agent

Streaming Simulation

Python async streaming

Kafka-like simulation (local)

Real-time feature extraction

MLOps

MLflow (experiment tracking)

Model versioning

Docker container

HuggingFace Spaces deployment


PROJECT STRUCTURE :

insider_threat_ai/
│
├── data/
├── models/
├── logs/
│
├── src/
│   ├── stream_simulator.py
│   ├── feature_engineering.py
│   ├── anomaly_model.py
│   ├── risk_engine.py
│   ├── llm_reasoner.py
│   ├── agent.py
│
├── app/
│   ├── main.py
│
├── mlruns/
├── Dockerfile
├── requirements.txt
└── README.md





Alert

Escalate
