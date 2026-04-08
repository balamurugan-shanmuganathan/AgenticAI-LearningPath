# Module 03: RAG & Knowledge Systems

This is the "Data Awareness" layer. We focused on making the agent reliable by grounding its answers in real-world facts and enterprise data.

## 💡 Key Discussion Points & Pro-Tips

### 🛡 Local-First Engineering
- **Hugging Face vs Cloud**: We discussed the massive benefits of using **Local Embeddings** (`sentence-transformers`). Our focus was on **privacy (GDPR compliance)**, cost reduction, and near-zero latency for the search loop.
- **Persistence Architecture**: Discussed how ChromaDB stores vectors on disk (`chroma.sqlite3`) so data remains available without re-embedding.

### 📐 Strategic Chunking
- **Context Preservation**: Discussed why fixed-size splits fail and why **Recursive Character Splitting** is the baseline for production.
- **Semantic Overlap**: The "secret sauce"—we discussed why a 10-20% overlap is mandatory so related sentences aren't cut mid-thought.

### 🎯 Optimization & Re-ranking
- **The Rerank Boost**: Discussed why vector search alone isn't enough. We implemented **LLM Re-ranking** to double-check the top 5 results before feeding them to the AI.
- **Ensemble Search (Hybrid)**: Discussed combining BM25 (keyword) with Vector search to catch technical jargon that embeddings might miss.

### ⚖ Agentic Guardrails
- **Self-Correction**: Discussed the **Corrective RAG** pattern—if the search result is irrelevant, the agent acknowledges the failure instead of hallucinating.
- **Grounding Checks**: Discussed the final "judge" step where the AI evaluates its own answer against the context.
