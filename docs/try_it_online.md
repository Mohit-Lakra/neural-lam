# Try it Online — Colab Graph Visualisation

Spin up the full Neural-LAM graph visualisation workflow directly in your browser. This page simply opens the production-ready `graph_visualisation.ipynb` in Google Colab so you can explore the GraphLAM/HiLAM structure without cloning the repository.

[![Run graph_visualisation.ipynb in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Mohit-Lakra/neural-lam/blob/prototype-2/docs/quickstart/graph_visualisation.ipynb)

## What happens when you click the badge?

1. Colab loads the latest committed version of `docs/quickstart/graph_visualisation.ipynb` from `prototype-2`.
2. The notebook installs `neural-lam`, PyTorch (CPU wheels), Plotly, and gdown automatically.
3. The official `meps_example` dataset (graphs + statics) is downloaded via gdown if it is not already cached for the Colab runtime.
4. All visualisations and histograms render inline with committed outputs, so you can inspect the structure even before running any cells.

```{admonition} Tip: Run All
:class: tip
Use **Runtime → Run all** in Colab to refresh every Plotly figure. The
cells cache tensors, so reruns stay under a couple of minutes even on free-tier runtimes.
```

## Why this matters

- Gives collaborators a zero-setup way to inspect the core graph data structures.
- Ensures the visual narrative stays in sync with the notebook checked into the docs.
- Demonstrates the encode → process → decode pipeline and HiLAM hierarchy with interactive 3D plots.

```{admonition} Data footprint
:class: note
`meps_example` downloads roughly 800 MB of archives before extraction. Colab
runtimes have ample temporary space, but expect the first run to take a few minutes.
```

Need to debug or extend the notebook? Fork Neural-LAM, edit
`docs/quickstart/graph_visualisation.ipynb`, and re-open this Colab link to pick up your changes.
