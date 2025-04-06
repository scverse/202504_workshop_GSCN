# Day 1: Introduction to Single-cell RNA-seq Analysis

## Environment setup

```
conda create -y --name workshop_2025 python=3.10
pip install uv
uv pip install jupyterlab notebook 
conda install -y ipykernel conda-forge::python-annoy
uv pip install scikit-misc PhenoGraph celltypist palantir scrublet cellrank pydeseq2 liana gseapy rpy2 anndata2ri scanpy python-igraph pyscipopt decoupler pybiomart adjustText
python -m ipykernel install --user --name workshop_2025
```

## Data

We will work with publicly available data throughout the workshop:
- Please download this folder in your workstation: https://drive.google.com/drive/folders/1fXhGtF4qnaiXDBBHvQGfgxDWc9h45oR5?usp=sharing

## Notebooks

### Morning Session: Basic Analysis Pipeline

1. [Quality Control and Normalization](nb1_qc_normalization.ipynb)
   - Learn how to perform quality control on single-cell RNA-seq data
   - Understand and apply different normalization techniques
   - Identify and filter out low-quality cells

2. [Preprocessing](nb2_preprocessing.ipynb)
   - Explore data preprocessing steps including feature selection
   - Learn about dimensionality reduction techniques
   - Understand how to handle technical artifacts

3. [Batch Correction](nb3_batch_correction.ipynb)
   - Learn about batch effects in single-cell data
   - Apply different batch correction methods
   - Evaluate the effectiveness of batch correction

### Afternoon Session: Advanced Analysis

4. [Downstream Analysis](nb4_downstream_analysis.ipynb)
   - Perform clustering and cell type annotation
   - Conduct differential expression analysis
   - Visualize and interpret results

5. [Trajectory Inference](nb5_trajectory_inference.ipynb)
   - Learn about trajectory inference methods
   - Apply trajectory analysis to understand cell differentiation
   - Visualize and interpret developmental trajectories

