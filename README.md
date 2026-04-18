# gatac-notebooks

Analysis notebooks for [GATAC](https://github.com/yourusername/GATAC) — the
GPU-accelerated ATAC-seq processing toolkit.

These notebooks are rendered and served as part of the GATAC documentation via
[MyST-NB](https://myst-nb.readthedocs.io/).  They are included as a git
submodule in the main GATAC repository under `notebooks/` at the repo root.

## Running locally

```bash
# Install GATAC (from the GATAC repo root)
uv sync --extra cuda12

# Launch JupyterLab
uv run jupyter lab
```

## Data

Notebooks use the PBMC 5k ATAC-seq dataset from 10x Genomics.  Download
instructions are included at the top of each notebook.

---

## Adding a notebook

1. Create your `.ipynb` under the appropriate directory.
2. Follow the naming convention: `NN_short_description.ipynb`.
3. Add a MyST-formatted markdown cell at the top with title and description.
4. Add the notebook path to `docs/tutorials/index.md` in the GATAC repo (the toctree entry uses `../../notebooks/<filename>`).
5. Clear all outputs before committing (`Edit → Clear All Outputs`).
