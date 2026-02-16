# IQuHack 2025 – IonQ Challenge (MaxCut)

This repository contains our work for the **IonQ iQuHACK 2025 Challenge**, focused on solving **Maximum Cut (MaxCut)** instances using a variational quantum approach (varQITE-style workflow provided in the challenge materials) implemented in **Qiskit**.

## What’s inside

- `IonQuHack2025.ipynb`  
  Main notebook: environment setup, graph construction (NetworkX), ansatz design, and evaluation workflow.
- `IonQuHack2025_mosh-pit_max-cut.pdf`  
  Short report / write-up of our approach and results.

## Problem (quick summary)

**MaxCut**: Given a graph \(G=(V,E)\), partition vertices into two sets such that the number of edges crossing the partition is maximized. It’s a classic NP-hard combinatorial optimization benchmark.

## Approach

- Build and test multiple candidate graphs (cycle, bipartite, regular, planar-ish, random connected, etc.).
- Construct a **parameterized quantum circuit (ansatz)** for a given graph.
- Tune circuit parameters to increase the probability of sampling high-cut solutions.
- Evaluate performance through the challenge workflow.

## Getting started

### 1) Prerequisites
- Python 3.9+ (3.10+ recommended)
- Jupyter Notebook or JupyterLab

### 2) Create a virtual environment (recommended)
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
# .venv\Scripts\activate   # Windows
pip install -U pip
