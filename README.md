# Evaluation of Constrained Classical Optimizers for Noisy Variational Quantum Circuits

**Author:** Vipul Sharma (IISER Bhopal) **Date:** April 24, 2025 

## Project Overview

This project evaluates the performance of classical optimization techniques on noisy variational quantum circuits under practical constraints. It investigates how different optimizers handle limitations like circuit depth, output fidelity, and cost function variance in a simulated NISQ environment.

## Experimental Setup

**Circuit:** 4-qubit ansatz with depth-2, using parameterized RY gates and CNOT entanglement.


 
**Hamiltonian:** 2-local Hamiltonian interacting qubit system (Z_0Z_1 + ...).


 
**Backend:** Qiskit Aer simulator with shot-based sampling (1024 shots).


 
**Constraints:** Circuit depth, fidelity thresholds, and variance limits.



## Optimizers Compared

The study benchmarks six algorithms:

* Gradient Descent
* Adam
* Momentum-based Gradient Descent
* COBYLA
* SPSA
* Simulated Annealing

## Key Findings

* 
**Noise Resilience:** COBYLA and Simulated Annealing demonstrated the strongest resilience against noise and achieved higher fidelity solutions.


* 
**Convergence:** Gradient-based optimizers (Adam, Momentum-GD) converged faster but were prone to local minima and instability in high-noise settings.



## Dependencies

* Python
* Qiskit (Aer)
* NumPy/SciPy
