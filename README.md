# Agentic AI Learning Path

### 🎯 Project Objective
This repository is a comprehensive, code-first learning journey designed to master the transition from Large Language Models (LLMs) to **Autonomous Agents**. Through a series of specialized modules, it explores the foundations of reasoning, context management, tool integration, and structural control loops required to build production-grade agentic systems.

🔗 **Main Repository**: [balamurugan-shanmuganathan/AgenticAI-LearningPath](https://github.com/balamurugan-shanmuganathan/AgenticAI-LearningPath)

---

## 🏗 Repository Structure

```text
.
├── 01-Foundation/
│   ├── 01-Prompt-Engineering.ipynb
│   ├── 02-Context-Engineering.ipynb
│   ├── 03-Tool-Calling.ipynb
│   └── 04-ReAct-Pattern.ipynb
├── 02-Memory-State/
│   ├── 01-Stateless-vs-Stateful.ipynb
│   ├── 02-In-Context-Memory.ipynb
│   ├── 03-External-Memory.ipynb
│   └── 04-Long-Term-Memory.ipynb
├── 03-RAG-Knowledge-Systems/
│   ├── 01-Introduction-to-RAG.ipynb
│   ├── 02-Chunking-Strategies.ipynb
│   ├── 03-Vector-Storage-Essentials.ipynb
│   ├── 04-Retrieval-Optimization.ipynb
│   └── 05-Agentic-RAG-Patterns.ipynb
├── 04-Agent-Orchestration/
│   ├── 01-Single-Agent-State-Machine.ipynb
│   ├── 02-Sequential-Multi-Agent-Handoffs.ipynb
│   ├── 03-Multi-Agent-Supervisor.ipynb
│   ├── 04-Collaborative-Research-Team.ipynb
│   └── 05-Hierarchical-Orchestration.ipynb
├── 05-Agentic-Design-Patterns/
│   ├── 01-Reflection-Pattern.ipynb
│   ├── 02-Refraction-Pattern.ipynb
│   ├── 03-Self-Healing-Pattern.ipynb
│   ├── 04-Human-in-the-Loop.ipynb
│   └── 05-Plan-and-Execute-Pattern.ipynb
├── 06-Eval-Observability/
│   ├── 01-Introduction-to-Evaluation.ipynb
│   ├── 02-Observability-with-LangSmith.ipynb
│   ├── 03-Trajectory-Evaluation.ipynb
│   └── 04-Automated-Benchmarking.ipynb
├── README.md
└── requirement.txt
```

### [01. Foundation](./01-Foundation)
The pillar of Agentic AI. Before an agent can act, it must be able to reason and manage its environment accurately.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Prompt Engineering** | Mastering instructions, few-shot prompting, and tone control. | [Notebook](./01-Foundation/01-Prompt-Engineering.ipynb) |
| **2. Context Engineering** | Managing knowledge, relevance, and information density. | [Notebook](./01-Foundation/02-Context-Engineering.ipynb) |
| **3. Tool Calling** | Bridging LLM logic with Python code. Best practices for schemas. | [Notebook](./01-Foundation/03-Tool-Calling.ipynb) |
| **4. ReAct Pattern** | The reasoning core: Thought-Action-Observation loops. | [Notebook](./01-Foundation/04-ReAct-Pattern.ipynb) |

### [02. Memory & State](./02-Memory-State)
The persistence layer. Transitioning from stateless API calls to continuous agentic sessions.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Stateless vs Stateful** | Core differences, manual history management vs. automated memory. | [Notebook](./02-Memory-State/01-Stateless-vs-Stateful.ipynb) |
| **2. In-Context Memory** | Managing \"Working Memory\" within the prompt context buffer. | [Notebook](./02-Memory-State/02-In-Context-Memory.ipynb) |
| **3. External Memory** | Concept of persistence: Saving history to files or databases. | [Notebook](./02-Memory-State/03-External-Memory.ipynb) |
| **4. Long-Term Memory** | Conceptual intro to Vector databases and semantic search (RAG). | [Notebook](./02-Memory-State/04-Long-Term-Memory.ipynb) |

### [03. RAG & Knowledge Systems](./03-RAG-Knowledge-Systems)
Extending an agent's knowledge. Connecting LLMs to external data sources reliably.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Intro to RAG** | Basic ETL flow: Load, Split, Embed, Store. | [Notebook](./03-RAG-Knowledge-Systems/01-Introduction-to-RAG.ipynb) |
| **2. Chunking Strategies** | Semantic, Similarity, and Recursive splitting for accuracy. | [Notebook](./03-RAG-Knowledge-Systems/02-Chunking-Strategies.ipynb) |
| **3. Vector Storage** | Working with ChromaDB and FAISS for semantic search. | [Notebook](./03-RAG-Knowledge-Systems/03-Vector-Storage-Essentials.ipynb) |
| **4. Retrieval Optimization** | Multi-Query, Compression, and Re-ranking techniques. | [Notebook](./03-RAG-Knowledge-Systems/04-Retrieval-Optimization.ipynb) |
| **5. Agentic RAG** | Self-correction, Routing, and Evaluation loops. | [Notebook](./03-RAG-Knowledge-Systems/05-Agentic-RAG-Patterns.ipynb) |

### [04. Agent Orchestration](./04-Agent-Orchestration)
Coordinating multiple agents into specialized teams. Mastering state machines and multi-agent loops.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. State Machine** | The Bridge: Re-implementing a single agent as a Graph. | [Notebook](./04-Agent-Orchestration/01-Single-Agent-State-Machine.ipynb) |
| **2. Agent Handoffs** | Passing the baton: Sequential Multi-Agent flows. | [Notebook](./04-Agent-Orchestration/02-Sequential-Multi-Agent-Handoffs.ipynb) |
| **3. Supervisor** | The Management Pattern: Centralized delegation. | [Notebook](./04-Agent-Orchestration/03-Multi-Agent-Supervisor.ipynb) |
| **4. Collaborative Team** | Shared state and peer-to-peer agent interaction. | [Notebook](./04-Agent-Orchestration/04-Collaborative-Research-Team.ipynb) |
| **5. Hierarchies** | Scaling to enterprise: Hierarchical Team Orchestration. | [Notebook](./04-Agent-Orchestration/05-Hierarchical-Orchestration.ipynb) |

### [05. Agentic Design Patterns](./05-Agentic-Design-Patterns)
Bridging the gap between basic orchestration and production-grade architectures.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Reflection Pattern** | Internal self-correction and drafting loops. | [Notebook](./05-Agentic-Design-Patterns/01-Reflection-Pattern.ipynb) |
| **2. Refraction Pattern** | Evaluating past trajectories and external environment failures. | [Notebook](./05-Agentic-Design-Patterns/02-Refraction-Pattern.ipynb) |
| **3. Self-Healing** | Autonomous recovery from execution or tool error tracebacks. | [Notebook](./05-Agentic-Design-Patterns/03-Self-Healing-Pattern.ipynb) |
| **4. Human-in-the-Loop** | Graph breakpoints requiring explicit human approval. | [Notebook](./05-Agentic-Design-Patterns/04-Human-in-the-Loop.ipynb) |
| **5. Plan & Execute** | Breaking down complex queries into structured checklists before execution. | [Notebook](./05-Agentic-Design-Patterns/05-Plan-and-Execute-Pattern.ipynb) |

### [06. Eval & Observability](./06-Eval-Observability)
Measuring agent performance and debugging complex multi-step reasoning trajectories.

| Topic | Description | Code |
| :--- | :--- | :--- |
| **1. Introduction to Eval** | Understanding LLM-as-a-judge and heuristic evaluation metrics. | [Notebook](./06-Eval-Observability/01-Introduction-to-Evaluation.ipynb) |
| **2. LangSmith Observability** | Tracing multi-agent interactions, tool calls, and latency. | [Notebook](./06-Eval-Observability/02-Observability-with-LangSmith.ipynb) |
| **3. Trajectory Evaluation** | Assessing the reasoning path of an agent across multiple steps. | [Notebook](./06-Eval-Observability/03-Trajectory-Evaluation.ipynb) |
| **4. Benchmarking** | Creating and running automated test suites for continuous improvement. | [Notebook](./06-Eval-Observability/04-Automated-Benchmarking.ipynb) |

---

## 🛠 Prerequisites
- Python 3.9+
- Google Gemini API Key
- LangChain Framework
- LangGraph
- LangGraph-Checkpoint-Sqlite
- ChromaDB & FAISS
- Hugging Face sentence-transformers (Local Embeddings)

---

## 🚀 Roadmap
- [x] **01. Foundation** (Prompting, Context, Tools, ReAct)
- [x] **02. Memory & State** (Stateless, Stateful, SQLite Persistence)
- [x] **03. RAG & Knowledge Systems** (Semantic Chunking, Vector DBs, Multi-Query)
- [x] **04. Agent Orchestration** (State Machines, Supervisor, Multi-Agent Teams)
- [x] **05. Agentic Design Patterns** (Reflection, Refraction, HITL, Plan & Execute)
- [ ] **06. Eval & Observability**
