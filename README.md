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
