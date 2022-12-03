# Implementation of the MDP Order Dispatch Policy

This repository contains the implementation of the paper [Large-Scale Order Dispatch in On-Demand Ride-Hailing Platforms: A Learning and Planning Approach](https://dl.acm.org/doi/10.1145/3219819.3219824) in Python. Specifically, it creates a synthetic environment to simulate the ridesharing marketplace according to Section 6.1 of the paper and applies the MDP order dispatch policy developed in the paper to this example. Please refer to `Demonstration.ipynb` for the detailed implementation. 

## Summary of the Algorithm

The algorithm consists of two steps:

* **Policy Evaluation**: Apply temporal difference learning to the historical data to learn the value function
* **Order Dispatch**: Implement the order dispatch policy by maximizing the value function

Illustration of the policy evaluation step:

<img align="center" src="policy_evaluation.png" alt="drawing" width="700">

Pseudocode:

<img align="center" src="pe_pseudocode.png" alt="drawing" width="700">

The order dispatch step:

<img align="center" src="MDP.png" alt="drawing" width="700">

Simulation results and comparison against other baseline policies: 
