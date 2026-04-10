# Module 05: Agentic Design Patterns

Welcome to **Module 05: Agentic Design Patterns**.

While Module 04 focused on Orchestration (how multiple agents communicate), this module focuses on the actual **Design Patterns** that make individual agents or small networks of agents highly reliable, robust, and autonomous in a production setting.

In modern Agentic AI (2024-2025), building an agent extends beyond simple prompt loops involving tools. Real-world systems require advanced architectures to ensure they do not fail silently, hallucinate indefinitely, or become stuck in infinite execution loops.

## 📁 The 5 Core Architectures

This module explores the 5 most impactful architectural patterns used by AI engineers to build advanced cognitive loops.

1. **[01. Reflection Pattern](./01-Reflection-Pattern.ipynb)**
   - **The Concept:** Teaching an agent to critique its own output internally. The LLM generates a draft, then a strictly prompted "Reflector" node evaluates it against standard guidelines, forcing the actor to rewrite until approved.
   - **Why it matters:** Radically improves the baseline quality of zero-shot outputs without needing external feedback.

2. **[02. Refraction Pattern (Reflexion)](./02-Refraction-Pattern.ipynb)**
   - **The Concept:** Learning from *external* environmental failures. The Refraction Agent attempts a task (e.g., executing code or searching), observes the failure, and writes a discrete "lesson learned" into its working memory before trying again entirely.
   - **Why it matters:** Unlike Reflection (internal critique), Refraction alters the trajectory of the agent based on physical world/tool interaction, preventing runaway loops.

3. **[03. Self-Healing Pattern](./03-Self-Healing-Pattern.ipynb)**
   - **The Concept:** Fault tolerance and autonomous debugging at the tool level. Unsafe operations (like executing generated Python code) are wrapped in `try/except` blocks.
   - **Why it matters:** When a stack trace is thrown, it acts as a direct feedback loop. The LLM diagnoses the Python error and re-writes the logic to bypass it autonomously.

4. **[04. Human-in-the-Loop (HITL) Pattern](./04-Human-in-the-Loop.ipynb)**
   - **The Concept:** Introducing explicit human governance. The LangGraph stops execution dynamically using breakpoints right before an irrevocable or risky tool is fired (e.g., sending an email or dropping a database).
   - **Why it matters:** Essential for enterprise-grade autonomous safety.

5. **[05. Plan & Execute Pattern](./05-Plan-and-Execute-Pattern.ipynb)**
   - **The Concept:** Task decomposition for massive goals. Instead of fumbling through a request linearly, a Planner Agent dictates an explicit step-by-step checklist. Executors complete one step, and a Replanner evaluates if the overarching goal requires more steps.
   - **Why it matters:** Solves the context-drift problem that plagues traditional ReAct agents when faced with multi-faceted user prompts.

## 💡 Pro-Tips

*   **The Cost of Autonomy:** Complex state machines like Plan-and-Execute or Refraction consume vastly more tokens and compute time than single-shot prompts. Always use graph `recursion_limit` controls.
*   **Mix and Match:** In production, these patterns are rarely mutually exclusive. You will often see a Supervisor Agent (from Module 04) delegate to a Worker who uses a Self-Healing Tool setup (from Module 05) before passing the draft through an internal Reflection loop.
