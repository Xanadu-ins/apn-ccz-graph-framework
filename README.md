# APN CCZ-Equivalence via Graph Isomorphism

## Overview

This repository contains the implementation and experimental data for the paper:

**"Equivalence Determination of APN Functions Based on the I/R Algorithm"**

We propose a framework that reduces the problem of CCZ-equivalence of APN functions to a graph isomorphism problem via associated linear codes and canonical labeling.

---

## Repository Structure
code/ SageMath implementations of graph constructions
data/ Input APN function sets
results/ Experimental results (tables and logs)


---

## Implemented Methods

The repository includes four graph constructions:

- Weighted Graph
- Minimum-Weight Codeword Subgraph
- Incidence Bipartite Graph
- Higher-Order Incidence Bipartite Graph

Each method is implemented as an independent SageMath script.

---

## Requirements

- SageMath 9.3
- Jupyter Notebook (recommended for running Sage)

---

## How to Run

1. Open SageMath 9.3 with Jupyter Notebook:

3. Load one of the scripts from the `code/` directory.

4. Modify the following parameters in the script:
- Dimension `n`
- List of APN functions

4. Execute the script to generate canonical forms and experimental results.

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
