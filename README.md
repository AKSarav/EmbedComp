# EmbedComp 🔍

> Benchmark and compare embedding models on **your own data** — not just standard leaderboards.

EmbedComp notebook is to validate the HF embedding model with your choice of dataset on various parameters - the notebook runs a full retrieval benchmark across multiple embedding models and renders an interactive Plotly dashboard covering latency, throughput, recall, and cosine quality — all in a single Jupyter notebook.

---

## Metrics

| Metric | What it measures | Target |
|---|---|---|
| Encode throughput | Documents embedded per second | ⬆ Higher |
| Query latency mean | Avg time from query to results (ms) | ⬇ Lower |
| Query latency p95 | Worst-case latency for 95% of queries | ⬇ Lower |
| Query latency p99 | Tail latency — slowest 1 in 100 queries | ⬇ Lower |
| Recall@1 | Top result was relevant | ⬆ Higher · ideal 1.0 |
| Recall@3 | Relevant doc found in top 3 | ⬆ Higher · ideal 1.0 |
| Recall@5 | Relevant doc found in top 5 | ⬆ Higher · ideal 1.0 |
| MRR | Relevant doc's average rank position | ⬆ Higher · ideal 1.0 |
| Cosine distribution | Similarity score spread across top-K hits | ⬆ Mean · ↔ narrow spread |


