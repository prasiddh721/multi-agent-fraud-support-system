# multi-agent-fraud-support-system
Enterprise-grade 5-Agent E-commerce Fraud &amp; Support Orchestrator built in
# 🧠 AI Multi-Agent E-Commerce Fraud & Customer Support Orchestrator

A fully functional **5-Agent enterprise-grade AI system** built using pure Python.  
No external APIs required.  
Designed for **real-world e-commerce customer support**, fraud detection, and ticket escalation.

---

## 🖼 System Architecture Diagram

![AI Multi-Agent Architecture] (Architecture.png)

---

## 🚀 Features

### 🔹 1. Intent Classification Agent
Understands user intent such as:
refund, cancellation, billing issue, delivery issue, fraud report, login issue, general help, feedback.

### 🔹 2. Sentiment Analysis Agent
Detects emotional tone:
very_angry, frustrated, neutral, positive, very_positive.

### 🔹 3. Fraud Detection Agent
Interpretable risk scoring based on:
keywords, metadata, account age, IP mismatch, prior chargeback.

### 🔹 4. Reply Agent
Generates tone-adjusted, urgency-aware, fraud-sensitive responses.

### 🔹 5. Escalation Agent
Decides escalation:
normal queue / priority_support / fraud_team.

### 🔹 6. Memory System
Maintains short conversation history with timestamps.

---

## 🧩 System Pipeline (How It Works)

User Message
|
v
Intent Agent ─────► intent + urgency
|
v
Sentiment Agent ─► sentiment label + score
|
v
Fraud Agent ─────► fraud risk + reasons
|
v
Reply Agent ─────► AI-generated reply
|
v
Escalation Agent ► escalation decision
|
v
Coordinator ─────► combined output + memory update




---

## 📊 Example Output

```json
{
  "intent": "fraud_report",
  "sentiment": "very_angry",
  "fraud_risk": "high",
  "reply": "I completely understand how frustrating...",
  "escalation": {
     "escalate": true,
     "queue": "fraud_team"
  }
}

