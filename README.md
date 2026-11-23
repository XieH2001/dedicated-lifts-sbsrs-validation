# Dedicated Lifts in Shuttle-Based Storage and Retrieval Systems — Validation Results

This repository provides the supplementary simulation-validation results for the paper:

> **Impact of Dedicated Lifts on Shuttle-Based Storage and Retrieval Systems: Design and Operational Perspectives**

## Overview

The file [`GitHub validation results.xlsx`](<GitHub validation results.xlsx>) contains the **repeated-run results of the simulation validation experiments** reported in the paper.

Owing to the space limitations of the manuscript, only a subset of the runs could be included in the paper. The workbook therefore presents **three repeated runs as a representative example** for each configuration, and compares the simulated throughput time against the corresponding analytical model.

## Data structure

The workbook contains three sheets, one for each total number of main aisles (*M*):

| Sheet  | Number of main aisles (*M*) |
|--------|-----------------------------|
| `M=9`  | 9                           |
| `M=15` | 15                          |
| `M=21` | 21                          |

Each sheet reports, for every combination of the input parameters, the analytical and simulated throughput time and their relative error, followed by three replications of the component-level results.

### Input parameters

| Column | Symbol | Meaning | Values |
|--------|--------|---------|--------|
| The number of main-aisle | *M* | Total number of main aisles | 9, 15, 21 (one per sheet) |
| The order arrival rate | *λ* | Order arrival rate | 0.15, 0.18, 0.21, 0.24 |
| The number of storage positions per tier | *N* | Number of storage positions per tier | 16, 20, 24 |
| Assignment probability | *ps* | Assignment probability | 1.0, 0.9, 0.8, 0.7 |

> Note: the `M=21` sheet does not include the `λ = 0.24` block, so it contains fewer configurations than the `M=9` and `M=15` sheets.

### Throughput-time comparison

| Column | Meaning |
|--------|---------|
| Throughput time (Tr) — Analytical results (A) | Throughput time computed by the analytical model |
| Throughput time (Tr) — Simulation results (S) | Throughput time from the simulation, averaged over the three replications |
| Relative error (ε) | Relative error between the analytical and simulated throughput time |

### Replication columns

For each of **Replication 1**, **Replication 2**, and **Replication 3**, the following six metrics are reported:

1. Throughput time (Tr)
2. Mean waiting time of orders for the same-tier shuttle service
3. Mean service time of the same-tier shuttle
4. Total mean service time of the cross-tier shuttle
5. Mean waiting time of the shutters for the tote-lift
6. Mean service time of the tote-lift loads a tote and transports it to the output point

## Validation accuracy

Across the 132 configurations reported in the workbook, the relative error between the analytical and simulated throughput time is:

| Statistic | Value |
|-----------|-------|
| Mean | 1.6 % |
| Median | 1.3 % |
| 90th percentile | 2.9 % |
| Maximum | 11.1 % |

The simulated throughput time closely matches the analytical model, with the large majority of configurations within a few percent.

## Citation

If you use these results in your work, please cite:

> Impact of Dedicated Lifts on Shuttle-Based Storage and Retrieval Systems: Design and Operational Perspectives
