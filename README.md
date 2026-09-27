# General Relativity — practice notebooks

Jupyter notebooks for the undergraduate General Relativity course
(Physics & Astronomy, Sejong University, Fall 2026).

The notebooks run in the browser on Google Colab, with nothing to install.
Click a badge to open one:

| Notebook | Topic | |
|----------|-------|-|
| `einsteinpy.ipynb` | Metrics with `einsteinpy`; index gymnastics in Minkowski spacetime | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blhuillier/2026B_GR/blob/main/einsteinpy.ipynb) |

Colab opens a copy for you. To keep your work, use *File → Save a copy in
Drive*; otherwise your changes are lost when you close the tab.

## Running locally instead

```
pip install -r requirements.txt
jupyter lab
```

## Conventions

Signature $(-,+,+,+)$, so $\eta_{\mu\nu}=\mathrm{diag}(-1,1,1,1)$, and units
with $c=1$ unless stated otherwise — the same as in the lecture notes.
