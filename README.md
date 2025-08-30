# PageRank on the Congressional Twitter Network

This repo implements the **PageRank algorithm from scratch** (both **unweighted** and **weighted** versions) on the **Congressional Twitter network**.  
It also includes scripts to reproduce figures related to **Viral Centrality** and the **edge-weight distribution** from the referenced papers.

---

## What's Inside

- `PageRank_Twitter_Congress.ipynb` — end-to-end notebook implementing PageRank (unweighted + weighted), ranking nodes, and comparing top-k results.
- `congress.edgelist` — weighted, directed edge list (NetworkX format).
- `congress_network_data.json` — adjacency lists with weights and username mapping.
- `compute_vc.py` — computes Viral Centrality (VC) using `viral_centrality.py`.
- `histogram_weights.py` — plots the distribution of edge weights.
- `viral_centrality.py` — VC implementation used by `compute_vc.py`.

> If you only want PageRank, the **notebook** is the main entry point.

---

## Quick Start
```bash

1) Create an environment & install deps

python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -U pip
pip install jupyter numpy pandas matplotlib networkx tqdm

2) Run the notebook
jupyter notebook PageRank.ipynb

