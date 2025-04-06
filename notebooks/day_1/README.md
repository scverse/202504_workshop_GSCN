# Day 1: Introduction

## Environment setup

```
conda create -y --name workshop_2025 python=3.10
pip install uv
uv pip install jupyterlab notebook 
conda install -y ipykernel conda-forge::python-annoy
uv pip install scikit-misc PhenoGraph celltypist palantir scrublet cellrank pydeseq2 liana gseapy rpy2 anndata2ri scanpy python-igraph pyscipopt decoupler pybiomart
python -m ipykernel install --user --name workshop_2025
```
