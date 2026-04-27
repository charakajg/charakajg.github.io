---
layout: gloc26
permalink: /gloc26/ablation-benchmark/
---

# 📊 Block 4 — Ablation Benchmark & Takeaways

A live **16-cell ablation** (2 regions × 4 modes × 2 models) across **28 OpenAI API calls** costing just **$0.0483 total** revealed:

- The **LLM Reasoning Agent** delivers clean, **model-independent perfect attribution (F1 = 1.000)** on unambiguous taxonomies like Sri Lanka's paddy belt.
- It produces a **reproducible over-reasoning failure** on Mato Grosso, where both models substitute pre-clearing LULC labels for the post-clearing reference.

### Takeaways

- **Model selection is region-conditional.** GPT-4o-mini matches GPT-4o at roughly **15× lower cost** on easy regions, while harder taxonomies require the larger model.
- **Deterministically reproducible.** The full pipeline is reproducible via **SHA-1-keyed JSON caching** of every LLM response.
