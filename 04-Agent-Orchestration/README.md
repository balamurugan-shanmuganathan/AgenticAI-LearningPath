# Module 04: Agent Orchestration

This module mastes the art of coordinating agents within a state machine. We transition from simple single-agent scripts to **Autonomous Agentic Teams** that can delegate, review, and collaborate to solve complex enterprise problems.

## 💡 Key Discussion Points & Pro-Tips

### 🌉 The "Bridge" for Beginners
- **State Machine Architecture**: We start by re-building our single agent as a **Graph** (LangGraph). This is the best way for beginners to understand how steps, decisions, and outcomes are logically separated.
- **The Graph Mindset**: Moving from code-only logic to a mapping of Nodes (Workers) and Edges (Logic).

### 🤝 Orchestration Patterns
- **The Supervisor Pattern**: Discussed why a central "Manager/Supervisor" is often more reliable than a swarm of peer agents for complex business tasks.
- **Handoffs vs. Collaboration**: Strategic choice between passing a task like a relay race (Handoff) or agents working on a shared board (Global State).

### 🔄 The Evaluator-Optimizer Loop
- **Multi-Agent Quality Control**: Discussed implementing a mandatory "Reviewer" agent that must sign off on a "Coder" agent's work before it is finalized.

### 🏢 Hierarchical Coordination
- **Scaling Agents**: Discussed the "Team of Teams" architecture for high-complexity enterprise applications where specialized squads report to a master orchestrator.

## 📦 Requirements
Ensure you have the latest versions of:
- `langgraph`
- `langchain-google-genai`
- `pydantic`
