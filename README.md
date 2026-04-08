# Agentic AI Learning Path

### 🎯 Project Objective
This repository is a comprehensive, code-first learning journey designed to master the transition from Large Language Models (LLMs) to **Autonomous Agents**. Through a series of specialized modules, it explores the foundations of reasoning, context management, tool integration, and structural control loops required to build production-grade agentic systems.

🔗 **Main Repository**: [balamurugan-shanmuganathan/AgenticAI-LearningPath](https://github.com/balamurugan-shanmuganathan/AgenticAI-LearningPath)

---

## 🏗 Repository Structure

```text
.
├── 01-Foundation/
│   ├── 1-PromptEngineering.ipynb
│   ├── 2-ContextEngineering.ipynb
│   ├── 3-ToolCalling.ipynb
│   └── 4-ReActPattern.ipynb
├── 02-Memory-State/
│   ├── 1-Stateless-vs-Stateful.ipynb
│   ├── 2-In-Context-Memory.ipynb
│   ├── 3-External-Memory.ipynb
│   └── 4-Long-Term-Memory.ipynb
├── README.md
└── requirement.txt
```

### [01. Foundation](./01-Foundation)
The pillar of Agentic AI. Before an agent can act, it must be able to reason and manage its environment accurately.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Prompt Engineering** | Mastering instructions, few-shot prompting, and tone control. | [Notebook](./01-Foundation/1-PromptEngineering.ipynb) |
| **2. Context Engineering** | Managing knowledge, relevance, and information density. | [Notebook](./01-Foundation/2-ContextEngineering.ipynb) |
| **3. Tool Calling** | Bridging LLM logic with Python code. Best practices for schemas. | [Notebook](./01-Foundation/3-ToolCalling.ipynb) |
| **4. ReAct Pattern** | The reasoning core: Thought-Action-Observation loops. | [Notebook](./01-Foundation/4-ReActPattern.ipynb) |

### [02. Memory & State](./02-Memory-State)
The persistence layer. Transitioning from stateless API calls to continuous agentic sessions.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Stateless vs Stateful** | Core differences, manual history management vs. automated memory. | [Notebook](./02-Memory-State/1-Stateless-vs-Stateful.ipynb) |
| **2. In-Context Memory** | Managing "Working Memory" within the prompt context buffer. | [Notebook](./02-Memory-State/2-In-Context-Memory.ipynb) |
| **3. External Memory** | Concept of persistence: Saving history to files or databases. | [Notebook](./02-Memory-State/3-External-Memory.ipynb) |
| **4. Long-Term Memory** | Conceptual intro to Vector databases and semantic search (RAG). | [Notebook](./02-Memory-State/4-Long-Term-Memory.ipynb) |

---

## 🛠 Prerequisites
- Python 3.9+
- Google Gemini API Key
- LangChain Framework
- LangGraph

---

## 🚀 Roadmap
- [x] **01. Foundation** (Prompting, Context, Tools, ReAct)
- [x] **02. Memory & State** (Stateless, Stateful, SQLite Persistence)
- [ ] **03. RAG & Knowledge Systems**
- [ ] **04. Multi-Agent Orchestration**
- [ ] **05. Eval & Observability**
