# arXiv GR-QC Collaboration Network Analysis

**Network analysis of 5,242 authors and 14,496 collaborations** from the arXiv General Relativity and Quantum Cosmology category.

### Project Overview
As part of a **2-person team** for the Data Analytics course (USI, Università della Svizzera Italiana), we performed a complete exploratory and hypothesis-driven analysis of the GR-QC scientific collaboration graph.

We investigated whether influence is concentrated among a small elite or distributed across the community, using graph theory, centrality measures, and similarity metrics.

### Key Findings
- **Hypothesis 1 rejected**: Influence is *not* concentrated — top 5% of authors account for only **16.3%** of total PageRank (vs. predicted >30%).
- **Hypothesis 2 rejected**: Top researchers do *not* form tight clusters — mean Jaccard similarity among top 10 authors is only **0.0375**.
- The network shows a **healthy, egalitarian, bridge-builder topology**: leading authors connect diverse research communities rather than isolated groups.
- Influence depends more on **collaboration quality** (PageRank) than sheer quantity (degree).

### Technologies Used
- **Python** • NetworkX • pandas • NumPy • Matplotlib • seaborn
- PageRank centrality • Jaccard similarity • Degree distribution analysis
- Hypothesis testing & scientific visualization

### Repository Contents
- `notebooks/` → Full reproducible Jupyter notebook
- `data/` → Original `ca-GrQc.txt` edge list
- `report/` → Final 5-page PDF report
- `figures/` → All key plots (global network, ego networks, PageRank vs degree, Jaccard heatmap, etc.)

### How to Reproduce
```bash
git clone https://github.com/YOURUSERNAME/arxiv-grqc-collaboration-network-analysis.git
cd arxiv-grqc-collaboration-network-analysis
pip install -r requirements.txt
jupyter notebook
