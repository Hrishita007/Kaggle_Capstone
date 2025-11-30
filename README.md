# 🌾 **Sarvagya Smart Farming Agent — MVP**

### *A Multi-Agent Farming Intelligence System (Capstone Submission)*

---

## 📌 **Overview**

**Sarvagya** is a **multi-agent smart farming assistant** demonstrating how AI can support farmers in day-to-day decisions.
This MVP is specially designed to satisfy the **Google AI Agents Capstone** requirements.

It simulates:

* 🌱 Soil & weather–based advisory
* 📈 Market price analysis
* 🛡 Fraud detection for traders
* 🧪 Inventory & fertilizer stock monitoring
* 🧠 Session memory for recent farm activity
* ⏱ Long-running weather monitoring
* 🔄 Agent-to-agent communication
* 🌐 Deployment-like API wrapper

The entire project is presented through a **guided Colab Notebook**.

---

## 🎯 **Core Features**

### 🧠 Multi-Agent Architecture

* Advisory Agent
* Market Analytics Agent
* Fraud Detection Agent
* Inventory/Stock Agent

### 🧰 Tools

* ML model (fraud detection)
* Rule-based reasoning (advisory + inventory)
* Custom long-running weather monitor

### 🗄 Memory

* Rolling session memory storing last 5 interactions

### 📜 Logging

* Agent-level execution logs for observability

### ⏳ Long-Running Operations

* Weather loop monitors irrigation alerts in real time

### 🔗 Agent-to-Agent (A2A)

* Example of agents communicating internally

### 🌐 Deployment Simulation

* API-styled wrapper for agent execution

---

## 🧩 **Notebook Structure**

1. **Introduction** — Purpose and high-level overview
2. **Setup** — Imports + logging config
3. **Synthetic Data Generation** — Soil, weather, market, trader, inventory
4. **Agents** — Advisory, Market, Fraud, Inventory
5. **Memory System** — Rolling buffer
6. **Evaluation** — Fraud ML model accuracy
7. **Weather Monitor** — Long-running loop with alerts
8. **Pipeline Execution** — Runs all agents in sequence
9. **Memory Viewer** — Shows last few outputs
10. **A2A Protocol (Optional)** — Agent-to-agent messaging
11. **Deployment Wrapper (Optional)** — Simulated API interface
12. **Final Summary** — Highlights capstone requirement coverage

---

## 📐 **Architecture**

```
                    ┌──────────────────────────┐
                    │   Multi-Agent Pipeline   │
                    └──────────────┬───────────┘
                                   │
      ┌────────────────────────────┼────────────────────────────┐
      │                            │                            │
┌──────────────┐          ┌──────────────────┐        ┌───────────────────┐
│ Advisory     │          │ Market Agent     │        │ Fraud Agent       │
│ Agent        │          │                  │        │ (ML)              │
└──────────────┘          └──────────────────┘        └───────────────────┘
                                   │
                                   ▼
                          ┌──────────────────┐
                          │ Inventory Agent  │
                          └──────────────────┘
                                   │
                                   ▼
                          ┌──────────────────┐
                          │   Memory Store   │
                          └──────────────────┘
```

---

## 🧪 **Concepts Demonstrated (Capstone Requirements ✔)**

| Concept                 | Implemented                          |
| ----------------------- | ------------------------------------ |
| Multi-agent system      | ✔ Advisory, Market, Fraud, Inventory |
| Tools                   | ✔ ML, rule-based engine, monitors    |
| Memory                  | ✔ Rolling session memory             |
| Long-running operations | ✔ Weather monitor                    |
| Sessions & state        | ✔ Memory + agent logs                |
| Observability           | ✔ Logging for each agent             |
| Agent evaluation        | ✔ Fraud model accuracy               |
| A2A Protocol            | ✔ Simple agent-to-agent messaging    |
| Deployment              | ✔ API-like wrapper                   |

---

## 🧪 **How to Run**

```bash
# Clone the repository
git clone https://github.com/yourusername/Kaggle_Capstone
cd Kaggle_Capstone

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook
```

Run all cells in order.

---

## 🚀 **Future Enhancements**

* Real-time APIs for weather, IoT sensors, and market data
* Multilingual voice interface for farmers
* Drone & rover integration with agritech hardware partners
* Mobile app version for field deployment
* Pest & disease prediction models

---

## 📄 **Disclaimer**

This MVP uses **synthetic data and simulated agents**.
It is strictly for **educational and capstone demonstration purposes**—not real-world agricultural decision-making.

---
