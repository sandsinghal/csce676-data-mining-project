# CSCE 676 Data Mining Project — Twitch Gamers Graph Analysis

Semester project for CSCE 676 (Data Mining) at Texas A&M University, Spring 2026.

## Overview

This project analyzes the **Twitch Gamers Social Network** (168K nodes, 6.8M edges)
using both classical graph mining techniques from the course syllabus and cutting-edge
heterophilic graph neural network methods from the KDD 2025 Best Paper (H2GB).

## Dataset

- **Source:** [SNAP — Twitch Gamers](https://snap.stanford.edu/data/twitch_gamers.html)
- **Paper:** Rozemberczki & Sarkar (2021). [arXiv:2101.03091](https://arxiv.org/abs/2101.03091)
- **Used in:** KDD 2025 Best Paper — [H2GB](https://github.com/junhongmit/H2GB)
- **Size:** 168,114 nodes, 6,797,557 edges
- **Tasks:** Churn prediction, language classification, view count estimation, and more

## Course Techniques Applied

- Graph Mining: Centrality, PageRank
- Community Detection: Louvain, Girvan-Newman
- Graph Embeddings: node2vec, DeepWalk
- Clustering: k-means, DBSCAN on embeddings
- Anomaly Detection: LOF, Isolation Forest
- Large-Scale ML: Random Forest, XGBoost ensembles

## Beyond-Course Techniques

- Heterophilic Graph Transformers (H2G-former) from KDD 2025 Best Paper
- Heterophilic message passing for node classification

## Project Structure

```
├── notebooks/
│   ├── checkpoint1_eda.ipynb
│   ├── checkpoint2_rqs.ipynb
│   ├── checkpoint3_deep_dive.ipynb
│   └── checkpoint4_showcase.ipynb
├── src/
│   ├── graph_utils.py
│   └── visualization.py
├── figures/
├── data/               (not tracked — download via notebook)
├── requirements.txt
└── README.md
```

## Setup

```bash
pip install -r requirements.txt
# Data is auto-downloaded in the notebooks
```

## References

- Rozemberczki, B., & Sarkar, R. (2021). Twitch Gamers. arXiv:2101.03091.
- Lin, J., et al. (2025). H2GB. KDD 2025 (Best Paper Award).
