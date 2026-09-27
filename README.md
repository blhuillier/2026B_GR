# General Relativity — practice notebooks

**Benjamin L'Huillier**\
Department of Physics and Astronomy, Sejong University\
2026 Fall

Jupyter notebooks accompanying the undergraduate course in General Relativity.
Each one follows a chapter of the lecture notes and mixes worked examples with
exercises for you to complete.

## Course outline

**Part I — Flat Spacetime**

1. From Newtonian Physics to Special Relativity
2. Minkowski Spacetime
3. Four-Vectors and Relativistic Dynamics
4. Tensors in Minkowski Spacetime

**Part II — From Special Relativity to Geometry**

5. From Inertia to Geometry

**Part III — The Geometry of Spacetime**

6. Smooth Manifolds
7. Tangent and Cotangent Spaces
8. Tensor Fields on Manifolds
9. The Metric Tensor
10. Covariant Derivatives and Parallel Transport
11. Geodesics
12. Curvature

**Part IV — Einstein Gravity**

13. The Stress-Energy Tensor
14. The Einstein Field Equations
15. The Newtonian and Weak-Field Limits

**Part V — Applications**

16. Schwarzschild Spacetime and Black Holes
17. Cosmology
18. Gravitational Waves

**Appendices**

- A. Topology and Smooth Manifolds
- B. Additional Differential-Geometric Tools

## Notebooks

| Notebook | Chapter | Topic | |
|----------|---------|-------|-|
| `ch04_index_gymnastics.ipynb` | 4 | Raising and lowering indices; symmetric and antisymmetric parts | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blhuillier/2026B_GR/blob/main/ch04_index_gymnastics.ipynb) |
| `ch12_christoffel_riemann.ipynb` | 10, 12 | Christoffel symbols and the Riemann tensor with `einsteinpy` | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blhuillier/2026B_GR/blob/main/ch12_christoffel_riemann.ipynb) |

## Running the notebooks

You can either run them in the browser on Google Colab, or on your own computer.

### Option 1: Google Colab

Click the *Open in Colab* badge next to a notebook. Nothing needs to be
installed; the first cell installs what the notebook needs.

Colab opens a temporary copy. To keep your work, use
*File → Save a copy in Drive* before closing the tab.

### Option 2: on your own computer, with uv

We suggest [uv](https://docs.astral.sh/uv/), a fast Python package and
environment manager. Install it by following the
[installation instructions](https://docs.astral.sh/uv/getting-started/installation/),
then clone this repository and create an environment for it:

```
git clone https://github.com/blhuillier/2026B_GR.git
cd 2026B_GR
uv venv .venv --python=3.14 --prompt 2026B_GR
```

The last command creates a virtual environment in the folder `.venv`, using
Python 3.14 (uv downloads it for you if it is not already installed), and
labels your shell prompt `(2026B_GR)` while the environment is active.

Activate the environment. On macOS or Linux:

```
source .venv/bin/activate
```

On Windows:

```
.venv\Scripts\activate
```

Then install the packages and start Jupyter:

```
uv pip install -r requirements.txt
jupyter lab
```

Next time, you only need to `cd` into the folder, activate the environment,
and run `jupyter lab`. To pick up new notebooks as they are added during the
semester, run `git pull` from the same folder.

## Conventions

Signature $(-,+,+,+)$, so $\eta_{\mu\nu}=\mathrm{diag}(-1,1,1,1)$, and units
with $c=1$ unless stated otherwise — the same as in the lecture notes.

## License

The code in these notebooks is released under the [MIT License](LICENSE). The
text, explanations and exercises are released under
[CC BY 4.0](LICENSE-CONTENT.md): you may reuse and adapt them with credit.
Material adapted from other authors is excepted; it is listed in
[`LICENSE-CONTENT.md`](LICENSE-CONTENT.md).
