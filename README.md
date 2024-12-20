# Forklift Leasing and Dock Management Optimization

## Project Overview

This repository contains the **Engineering Optimization Project** focused on optimizing forklift leasing and dock management for retail distribution centers. The objective is to minimize the cost of leasing forklifts and ensure efficient unloading schedules for shipments while adhering to time constraints.

### Files in the Repository

1. **Report:** [Enginerring_Optimization_Project.pdf](Enginerring_Optimization_Project.pdf)  
   This document provides a detailed explanation of the project, including:
   - Problem definition
   - Mixed-Integer Linear Programming (MILP) model formulation
   - Constraints and objective function
   - Methodology and performance metrics
   - Shipment data and dock management details

2. **Code:** `forklift_optimization.py`  
   Python code that implements the MILP model using the `PuLP` library.

### Requirements

- **Python 3.12.4** or later
- **PuLP Library** for solving optimization problems

Install `PuLP` using the following command:

```bash
pip install pulp
```

### Code Execution

To run the optimization, execute the script with:

```bash
python forklift_optimization.py
```

### Code Description

The code defines and solves the MILP problem with the following elements:

- **Forklift Types:**  
  - Type 1: €150 per lease  
  - Type 2: €120 per lease  
  - Type 3: €25 per lease

- **Decision Variables:**  
  - Number of each type of forklift leased.  
  - Binary variables indicating shipment assignments to docks and hours.

- **Objective:**  
  Minimize the total leasing cost and unloading time.

### Sample Output

```
Status: Optimal
Objective Value: 243.25
Type 1 Forklifts: 0.0
Type 2 Forklifts: 0.0
Type 3 Forklifts: 7.0
T[1] (Unloading Time): 1.75
T[17] (Unloading Time): 0.875
T[21] (Unloading Time): 2.625
...
Shipment 22 assigned to Dock 5 at Hour 4
Shipment 23 assigned to Dock 5 at Hour 3
Shipment 13 assigned to Dock 2 at Hour 4
Shipment 15 assigned to Dock 1 at Hour 3
```

### References

- [Supply Chain Optimization Using Linear Programming](https://towardsdatascience.com/supply-chain-process-optimization-using-linear-programming-b1511800630f)
- [PuLP Library Documentation](https://coin-or.github.io/pulp/)

---

This README provides a clear overview for users to understand, install, and run the project.
