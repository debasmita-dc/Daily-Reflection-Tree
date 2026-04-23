# Daily Reflection Tree – Design Rationale

## Objective
Design a deterministic end-of-day reflection tool that helps employees surface agency, contribution, and perspective without AI at runtime.

## Design Logic
Each axis uses realistic, experience-based questions with fixed options. Branching is minimal but intentional to preserve clarity and determinism.

## Psychology
- Axis 1: Locus of Control (Rotter), Growth Mindset (Dweck)
- Axis 2: Psychological Entitlement vs Contribution (Campbell, Organ)
- Axis 3: Self-Transcendence (Maslow), Perspective-Taking (Batson)

## AI Guardrails
- AI used only during design
- No free text input
- No LLM calls at runtime
- Fixed routing rules
- Prewritten reflections with interpolation only

## Future Work
Adaptive summaries and deeper Axis 3 branching.
