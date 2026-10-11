# LDLR-analysis

PCA of molecular dynamics simulations of the low-density lipoprotein receptor (LDLR) embedded in a membrane, used to assess how missense variants affect conformation and intramolecular interactions.

## Contents

| File | Description |
|---|---|
| `PCA-LDLr-gmf.ipynb` | PCA conformer plots (PC1 and PC2), clustered conformational states and trajectory motions |

## Method

Backbone atoms of each MD frame were extracted and aligned with `trj_selection_dl.py` and
`trj_align.py` (Schrödinger Suite 2021v.2). Individual simulations were merged into a single
trajectory and CMS file with `trj_merge.py`, and principal components were computed with
`trj_essential_dynamics.py`. PCA conformer plots (PC1 × PC2, states and motions) are
generated in the notebook with Matplotlib, Seaborn, NumPy and pandas.

## Requirements

Python 3 with Jupyter and the libraries listed below. Trajectories and
Schrödinger Suite outputs are **not** included in this repository.

```bash
pip install jupyter numpy pandas matplotlib seaborn
```

## Author

**Glaucio Monteiro Ferreira** — Research Associate, Institute of Chemistry, University of São Paulo (IQ-USP) · [LIBNM · Ferreira Lab](https://ferreiralab.com.br) · [ORCID](https://orcid.org/0000-0002-1952-9428) · [FAPESP profile](https://bv.fapesp.br/pt/pesquisador/703612/glaucio-monteiro-ferreira/) · [gmf@usp.br](mailto:gmf@usp.br)
