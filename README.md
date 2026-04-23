# Daily-Reflection-Tree
# Daily Reflection Tree — Part A

This repository contains 
a **fully deterministic decision tree** for an end-of-day employee reflection tool.

The tree guides an employee through a structured reflection across three psychological axes:
1. **Locus** — Victim vs Victor  
2. **Orientation** — Entitlement vs Contribution  
3. **Radius** — Self-Centrism vs Altrocentrism  

The product is the **tree itself**, represented as structured data.  
No LLM or AI model is used at runtime.

---


---

## 🧠 Design Principles

- **Deterministic**: Same answers always lead to the same path and reflections  
- **No free text**: All questions use fixed, predefined options  
- **No LLM at runtime**: AI was used only during design, not execution  
- **Psychologically grounded**: Based on established research (Rotter, Dweck, Maslow, Organ)  
- **Non-judgmental tone**: The tree encourages awareness, not moral scoring  

---

## 🌳 Tree Overview

- **Total Nodes**: 30+
- **Question Nodes**: 9
- **Decision Nodes**: 4
- **Reflection Nodes**: 6
- **Bridge Nodes**: 4
- **Axes Covered**: All three, in sequence
- **State Tracking**: Axis-level signals (internal/external, contribution/entitlement, self/other)

The tree is stored in `reflection-tree.tsv` and can be walked by any simple engine that:
- Reads node definitions
- Routes deterministically based on answers
- Accumulates signals
- Interpolates predefined reflection text

---

## 🤖 AI Usage & Guardrails

AI tools were used only to:
- Brainstorm question wording
- Stress-test options against different personas
- Validate psychological alignment

**Guardrails implemented:**
- No generative text at runtime
- No probabilistic decisions
- No sentiment analysis or inference
- All logic encoded explicitly in the tree structure

---

## 🚀 Future Extensions 

- Runtime agent (CLI or web UI)
- Weekly or longitudinal summaries
- Cross-axis pattern reflections
