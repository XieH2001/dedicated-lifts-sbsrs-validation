# Dedicated Lifts in Shuttle-Based Storage and Retrieval Systems — Validation Results

This repository provides the supplementary simulation-validation results for the paper:

> **Impact of Dedicated Lifts on Shuttle-Based Storage and Retrieval Systems: Design and Operational Perspectives**

## Overview

The file [`GitHub validation results.xlsx`](<GitHub validation results.xlsx>) contains the **repeated-run results of the simulation validation experiments** reported in the paper.

Owing to the space limitations of the manuscript, only a subset of the runs could be included in the paper. The workbook therefore presents **three repeated runs as a representative example** for each configuration.

## Data structure

The workbook contains three sheets, one for each total number of aisles (*M*):

| Sheet  | Total number of aisles (*M*) |
|--------|------------------------------|
| `M=9`  | 9                            |
| `M=15` | 15                           |
| `M=21` | 21                           |

Key columns:

| Column                          | Meaning                                                        |
|---------------------------------|----------------------------------------------------------------|
| `区域到达率 λ/Z`                 | Area arrival rate of a zone (0.05, 0.06, 0.07, 0.08)                   |
| `层数 T`                        | Number of tiers                                       |
| `总巷道数量 M`                  | Total number of aisles                                         |
| `货架储位数 N`                  | Number of storage locations per aisle (16, 20, 24)             |
| `ps`                            | Load / service factor (1.0, 0.9, 0.8, 0.7)                     |
| `Tr`                      | Analytical model results      |
| `Queue4`, `same tier`, `different tier`, `Qs`, `combiner`, `bottom tier` | Simulation results from Flexsim |

For each configuration, the simulation results are reported over **three repeated runs**, which appear as three adjacent blocks of the same set of columns.

## Citation

If you use these results in your work, please cite:

> Impact of Dedicated Lifts on Shuttle-Based Storage and Retrieval Systems: Design and Operational Perspectives
