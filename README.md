# Deutsch-Jozsa-algorithm
## 1. Overview
his project shows how the Deutsch–Jozsa algorithm lets quantum computers solve certain problems much faster than classical computers.

The problem:

* You are given a black-box function \( f:{0,1}^n \to {0,1} \).
* The function is promised to be either:
  * Constant  always outputs 0 or always 1.
  * Balanced  half outputs are 1 and half are 0 .

Classically, in the worst case, you need to check more than half of all possible inputs to be sure about the nature of the function .
The Deutsch–Jozsa algorithm requires only a single test of the oracle.

In this notebook,to keep  things simple, we use n=1 case.

1. Build quantum circuits for constant and balanced oracles.
2. Run the algorithm on a simulator using Qiskit.
3. Visualize the outcomes with histograms and statevectors.
## 2. Topics Learn
As you go through this notebook, you will learn:

* The difference between constant and balanced oracles.
* How to build the Deutsch–Jozsa circuit using the Qiskit module.
* How quantum interference allows us to distinguish function types in one step.
* How to simulate and visualize results with Qiskit Aer and Matplotlib.
  ## 3. Requirements
* Python 3.10+ (I used 3.11)
* Jupyter Notebook or Jupyter Lab

Python packages:

* qiskit
* qiskit-aer (for simulation)
* matplotlib

Install dependencies:
``` dash
pip install qiskit qiskit-aer matplotlib 
```
## 4. Usage
1. Launch Jupyter Notebook or Lab:
2. Open Deustch-joza algorithm.ipynb.
3. Run all the cells.
4. Observe the following outputs:
  * Circuit diagrams.
  * Histograms showing measurement results.

Expected outcomes:

* Constant oracle → Always measure 0.
* Balanced oracle → Always measure 1.
## 5. Next Steps
* Extend the algorithm to more qubits (\(n > 1\)) to see the exponential speedup.
* Run the algorithm on a real IBM Quantum device instead of a simulator.
* Compare the quantum solution to a classical method to see the efficiency differences.
