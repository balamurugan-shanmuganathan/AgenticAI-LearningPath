# Module 05: Agentic Design Patterns

Welcome to **Module 05: Agentic Design Patterns**.

While Module 04 focused on Orchestration (how multiple agents communicate), this module focuses on the actual **Design Patterns** that make individual agents or small networks of agents highly reliable, robust, and autonomous in a production setting.

In modern Agentic AI (2024-2025), building an agent extends beyond simple prompt loops involving tools. Real-world systems require advanced structures to ensure they do not fail silently, hallucinate indefinitely, or become stuck in infinite execution loops.

## Core Concepts Covered

This module explores the most impactful Agentic Design Patterns, particularly focusing on the pillars of **Reflection, Planning, and Tool Verification**.

1. **Reflection Pattern**: The art of teaching an agent to critique its own output. Instead of generating a final response in one go, the agent reflects on its draft, identifies flaws, and iteratively improves it.
2. **Plan & Execute Pattern**: Breaking down a massive, complex goal into a discrete list of smaller, manageable sub-tasks. The agent generates a plan first, then systematically executes it, updating the plan dynamically if sub-tasks fail.
3. **Self-Healing Pattern**: Building fault tolerance into your agents. When a tool fails (e.g., Python code crashes or an API throws an error), the agent intercepts the error trace, diagnoses the problem, and attempts to write a fix autonomously.

## 📁 Notebooks in this Module

*   **[`01-Reflection-Pattern.ipynb`](./01-Reflection-Pattern.ipynb)**: Implement an Editor/Reviewer agentic loop that generates code, reflects on it, and issues self-corrections.
*   **[`02-Plan-and-Execute-Pattern.ipynb`](./02-Plan-and-Execute-Pattern.ipynb)**: Build an agent that creates an execution plan, steps through it, and manages a shared scratchpad of intermediate results.
*   **[`03-Self-Healing-Pattern.ipynb`](./03-Self-Healing-Pattern.ipynb)**: Create a rugged agent that executes code and uses error logs to self-heal and write functional scripts without human intervention.

## 💡 Pro-Tips

*   **LLM Choice Matters**: Reflection and Planning heavily tax an LLM's reasoning capabilities. While a fast model (like Gemini 1.5/2.5 Flash) is great for execution, you may want to use a larger reasoning model (like Gemini 1.5/2.5 Pro) for the Planning or Crititique nodes.
*   **The Cost of Autonomy**: Reflection and Self-Healing loops consume significantly more tokens than simple zero-shot queries. Always implement strong `recursion_limit` controls when building these loops.
*   **Structured Outputs are Mandatory**: In Plan & Execute, the planner MUST output a structured list of steps. Always use `with_structured_output` inside the Planner node.
