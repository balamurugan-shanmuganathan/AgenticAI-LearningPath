# Module 02: Memory & State

This module transitions the agent from a "one-off" responder to a continuous, self-aware assistant. We focus on how to maintain state across complex, multi-turn conversations.

## 💡 Key Discussion Points & Pro-Tips

### 🧠 Short-Term Context Management
- **The "Context Buffer" Dilemma**: We discussed why you can't just send the entire chat history forever. Mastering **windowing** and **pruning** is key to keeping costs down and maintaining model focus.
- **System Instructions for Memory**: Discussed how to prompt the model to "remember" specific user preferences while ignoring "noise."

### 💾 Persistence & Scaling
- **Moving to SQLite**: Discussed why production agents cannot rely on in-memory lists. We implemented a **SQLite-backed persistence layer** to ensure the agent survives script restarts.
- **Session IDs**: The importance of segregating memory by User/Thread ID to prevent "context leakage" between different users.

### 🔍 Semantic Memory (Conceptual)
- **Recall vs. Exact Match**: Discussed the shift from searching for exact words to searching for **meanings** using vectors—the foundation for long-term agent "life" experience.
