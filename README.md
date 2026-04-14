This repository is provided to support reproducibility of the experimental results.
# APN CCZ-Equivalence via Graph Isomorphism

## Overview

This repository contains the implementation and experimental data for the paper:

**"Equivalence Determination of APN Functions Based on the I/R Algorithm"**

We propose a framework that reduces the problem of CCZ-equivalence of APN functions to a graph isomorphism problem via associated linear codes and canonical labeling.

---

## Repository Structure
code/ SageMath implementations (graph constructions + invariant computations)
data/ Input APN function sets
results/ Experimental results (tables and logs)

The `code/` directory includes:
- Four graph construction methods
- Additional scripts for computing classical invariants of selected APN functions

---

## Implemented Methods

The repository includes four graph constructions:

- Weighted Graph
- Minimum-Weight Codeword Subgraph
- Incidence Bipartite Graph
- Higher-Order Incidence Bipartite Graph

In addition, we provide scripts for computing values of selected APN functions under certain classical invariants.

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

1. Open SageMath 9.3 with Jupyter Notebook:

sage -n jupyter

3. Load one of the scripts from the `code/` directory.

4. Modify the following parameters in the script:
   
   - Dimension `n`
     
   - List of APN functions

6. Execute the script to generate canonical forms and experimental results.

---

## Experimental Results

All experimental results reported in the paper are included in the `results/` directory.

- `n7_comparison.csv`: Representative comparison for dimension n = 7
  
- Additional datasets for other dimensions

These results demonstrate that the proposed graph-based methods achieve stronger distinguishability than classical invariants in several cases.

---

## Reproducibility

All experiments in the paper can be reproduced using the provided scripts and datasets.

---

## Notes

- Due to the flexibility of SageMath scripts, users are expected to manually adjust parameters (such as dimension and function lists) to reproduce specific experiments.
- The incidence bipartite graph construction provides the best trade-off between efficiency and discriminative power in our experiments.

---

## Contact

If you have any questions, please contact:

- 1215168081@qq.com
