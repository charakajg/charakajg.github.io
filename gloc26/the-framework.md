---
layout: gloc26
permalink: /gloc26/the-framework/
---

# 🧩 Block 2 — The Framework

An **LLM-augmented multi-agent architecture** built on **LangGraph** coordinates six agents over a shared typed state.

### Four deterministic agents

1. **Data preprocessing** — TROPOMI CH₄ and Sentinel-2 via Google Earth Engine.
2. **Emission detection** — DBSCAN clustering of anomalies above the 95th percentile.
3. **Land-use simulation** — Random Forest classification fed into CA-Markov 2030 projections.
4. **Integration & reporting** — Emission-factor overlay producing scenario-specific CH₄ totals.

### Two LLM-driven components on top

- **Reasoning Agent** — produces structured hotspot attributions, mitigation recommendations, and executive summaries.
- **Supervisor** — adaptively routes the pipeline, re-running preprocessing on QA failure or spawning focused scenarios when needed.
