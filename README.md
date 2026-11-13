# <project name>

<One paragraph: the question and the approach.>

## Reproduce

<Steps from a fresh clone to every figure.>

## Layout

| Path | Git | Contents |
| --- | --- | --- |
| `config/` | yes | Parameters and paths, read by every script |
| `environment/` | yes | Environment names and versions, `renv.lock`, exports |
| `workflow/` | yes | Pipeline definitions (Nextflow, targets) |
| `code/lib/` | yes | Project helper functions |
| `code/NN_<stage>/` | yes | Stage scripts, numbered in run order |
| `notebooks/` | yes | Exploration; nothing in `results/` comes from here |
| `data/raw/` | no | Own raw data; symlinks, read-only; listed in `MANIFEST.csv` |
| `data/external/` | no | Public data (GEO, SRA, published tables) |
| `data/processed/` | no | Intermediate objects |
| `data/metadata/` | yes | Sample sheets, libraries |
| `results/NN_<stage>/` | yes | Tables and panel PDFs; mirrors `code/` stages |
| `figures/` | yes | Final multi-panel figures |
| `manuscript/` | yes | Text and references |
| `docs/` | yes | Notes and decisions |
| `temp/` | no | Logs and scratch |
