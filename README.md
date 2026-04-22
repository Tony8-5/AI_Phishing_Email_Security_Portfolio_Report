# 🏛️ AI Regulatory Compliance — Relational Graph Automation Artefact

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)
[![Python](https://img.shields.io/badge/Python-3.10%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An interactive, touch-friendly knowledge graph that maps relationships between major AI regulatory frameworks and real-world compliance artefacts. Built as a Jupyter Notebook, it is designed to run in Google Colab or any local Jupyter environment.

---

## 📋 Overview

This artefact visualises the regulatory landscape across four frameworks:

| Framework | Coverage |
|---|---|
| **EU AI Act** | 11 articles: Art 9, 10, 11, 12, 13, 14, 15, 16, 17, 26, 51 |
| **UK GDPR** | 3 articles: Art 5 (Principles), Art 22 (Automated Decisions), Art 35 (DPIA) |
| **UK AI White Paper** | 4 principles: Safety, Transparency, Fairness, Accountability |
| **NIST AI RMF** | 4 functions: Govern, Map, Measure, Manage |
| **Automation Artefacts** | 5: Risk Register, Conformity Checklist, HITL Workflow, DPIA, Incident Report |
| **AI Systems** | 2: Phishing/Email Security, Fraud Monitoring |

### Use Cases Covered

- 🔒 **AI Phishing & Email Security System**
- 💳 **AI-Driven Bank Transaction Fraud Monitoring**
- 🌍 **EU AI Act High-Risk Provider Requirements**

---

## 🚀 Getting Started

### Option A — Google Colab (Recommended)

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Go to **Runtime → Run all** (or press `Ctrl+F9`)
3. The interactive graph will render inline in the notebook

### Option B — Local Jupyter

```bash
# 1. Clone the repository
git clone https://github.com/your-username/ai-regulatory-graph.git
cd ai-regulatory-graph

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook AI_Regulatory_Graph_Artefact.ipynb
```

---

## 🗂️ Notebook Structure

| Step | Description |
|---|---|
| Step 1 | Install Dependencies |
| Step 2 | Define Graph Data (Nodes & Edges) |
| Step 3 | Build NetworkX Graph |
| Step 4 | Render Interactive yFiles Graph |
| Step 5 | Subgraph Views (filter by law or use-case) |
| Step 6 | Centrality Analysis & Visualisation |
| Step 7 | Automation Artefact Content (Risk Register, HITL Workflow, Conformity Checklist) |
| Step 8 | Export All Artefacts |

---

## 📊 Interactive Graph Features

- **Click any node** to read its details in the sidebar
- **Drag nodes** to reposition — touch and mouse both supported
- **Use subgraph cells** to isolate a specific law or use-case
- **Hover over edges** to see the relationship type

---

## 📤 Exported Artefacts

Running Step 8 generates the following files:

| File | Format | Description |
|---|---|---|
| `risk_register.yaml` | YAML | AI Risk Register mapped to EU AI Act Art 9/17 and NIST RMF |
| `hitl_workflow.yaml` | YAML | Human-in-the-Loop Review Workflow (Art 14 / UK GDPR Art 22) |
| `conformity_checklist.json` | JSON | EU AI Act High-Risk Conformity Checklist (Art 16/17) |
| `regulatory_graph_data.json` | JSON | Full node and edge data for the knowledge graph |
| `centrality_analysis.png` | PNG | NetworkX centrality analysis chart |

---

## 🔑 Key Compliance Insights

1. **EU AI Act Art 16** is the highest-centrality node — it is the gateway to all provider obligations and connects to all Chapter 2 articles.
2. **UK GDPR Art 22** is the critical data-protection pinch-point for both AI systems deployed in employment and financial contexts.
3. **The HITL Workflow artefact** simultaneously satisfies Art 14 (EU AI Act human oversight) and Art 22 (UK GDPR automated decisions) — a single governance control with dual regulatory effect.
4. **Art 17 QMS** bridges internal quality governance and regulatory compliance, linking to both NIST Govern and EU Art 9.
5. The **UK AI White Paper** principles-based approach creates alignment gaps with the binding EU Act — particularly significant for UK organisations with EU market exposure.

---

## 📦 Dependencies

See [`requirements.txt`](./requirements.txt) for the full list. Key packages:

- [`yfiles-jupyter-graphs`](https://github.com/yWorks/yfiles-jupyter-graphs) — interactive graph rendering widget
- [`networkx`](https://networkx.org/) — graph construction and centrality analysis
- [`pyyaml`](https://pyyaml.org/) — YAML artefact serialisation
- [`matplotlib`](https://matplotlib.org/) — centrality visualisation

---

## 📚 References

- EU AI Act (Regulation 2024/1689)
- UK General Data Protection Regulation (UK GDPR)
- Data Protection Act 2018
- UK AI White Paper — DSIT (2023)
- NIST AI Risk Management Framework (2023)

---

*Artefact built for: Cyber Security Legal, Regulatory & Human Dimensions — Portfolio Assessment*
