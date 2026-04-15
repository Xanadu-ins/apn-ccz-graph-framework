This repository is provided to support reproducibility of the experimental results.

# APN CCZ-Equivalence via Graph Isomorphism

## Overview

This repository contains the implementation and experimental data for the paper:

**"Equivalence Determination of APN Functions Based on the I/R Algorithm"**

We propose a framework that reduces the problem of CCZ-equivalence of APN functions to a graph isomorphism problem via associated linear codes and canonical labeling.

---

## Repository Structure

code/ SageMath implementations (graph constructions + invariant computations)

results/ Experimental results (tables and logs)

list_of_APN_functions_for_different_n/ APN function lists for different n


### `code/` directory
- Four graph construction methods:
  - Weighted Graph
  - Minimum-Weight Codeword Subgraph
  - Incidence Bipartite Graph
  - Higher-Order Incidence Bipartite Graph
- Additional scripts for computing classical invariants of selected APN functions  
  (organized by `n = 5, 6, 7`)

### `results/` directory
- For each graph construction:
  - One `.xlsx` file containing all results (multi-sheet, organized by `n`)
  - Corresponding `.csv` files extracted from each sheet for direct preview on GitHub
- For invariant computations:
  - Subdirectories `n5/`, `n6/`, `n7/` containing the corresponding computed results

### APN function lists
- The file `list_of_APN_functions_for_different_n` provides the APN functions used in experiments for different values of `n`

---

## Requirements

- SageMath 9.3
- Jupyter Notebook (recommended)
- Nauty (for canonical labeling)
- Python package: `psutil` (for memory monitoring)

---

## Initial Setup (First-Time Use)

Before running the scripts, please complete the following setup steps.

### 1. Install Nauty

Open **SageMath Shell** and run:

cd ~
wget http://pallini.di.uniroma1.it/nauty2_9_1.tar.gz

tar zxvf nauty2_9_1.tar.gz

cd nauty2_9_1

./configure

make


If the executable `dreadnaut` is generated successfully, the installation is complete.

---

### 2. Install `psutil`

Open **SageMath Shell** and run:

sage -pip install psutil


This package is used to monitor memory usage during experiments.

---

## How to Run

1. Open SageMath with Jupyter Notebook:

sage -n jupyter


2. Load a script from the `code/` directory.

3. Modify the following parameters:
   - Dimension `n`
   - List of APN functions (see provided list)

4. Execute the script to generate results.

---

## Experimental Results

All experimental results are provided in the `results/` directory.

- `.xlsx` files: complete datasets (multi-sheet, grouped by `n`)
- `.csv` files: extracted per-`n` results for direct GitHub preview

A representative comparison (e.g., for `n = 7`) is included in the paper, while full datasets are available here.

---

## Reproducibility

All experiments in the paper can be reproduced using the provided scripts, APN function lists, and datasets.

---

## Notes

- Users are expected to manually adjust parameters (such as `n` and function lists) in the scripts.
- The incidence bipartite graph construction provides the best trade-off between efficiency and discriminative power in our experiments.

---

## Contact

If you have any questions, please contact:

- 1215168081@qq.com
