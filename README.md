# Percolation on the Square Lattice

## Project Overview

This project focuses on the study of percolation in two dimensions, specifically the site percolation model. The goal is to estimate the critical probability $p_c$ that determines the percolation threshold and to calculate several critical exponents that describe the fractal properties of the system near the percolation transition.

## What is Percolation?

Percolation refers to the process by which a substance or connection propagates through a medium or system. In the context of this project, we explore site percolation, where a grid is randomly populated with filled (occupied) or empty sites according to a probability $p$. As $p$ increases, clusters of occupied sites grow and eventually form a spanning cluster that connects one side of the system to the other, marking the percolation threshold.

### Applications of Percolation

- **Oil Extraction:** Studying how oil filters through porous rocks.
- **Traffic Flow:** Understanding the transition from free-flowing traffic to congestion.
- **Forest Fires:** Analyzing the spread of wildfires.

## Project Objectives

- **Estimate the Percolation Threshold $p_c$:** Determine the critical probability at which a spanning cluster first appears in the system.
- **Calculate Critical Exponents:**
  - **Fractal Dimension ($D$):** Describes the fractal nature of the percolating cluster.
  - **Correlation Length Exponent ($\nu$):** Related to the correlation length near the percolation threshold.
  - **Order Parameter Exponent ($\beta$):** Associated with the density of the percolating cluster.
  - **Susceptibility Exponent ($\gamma$):** Related to the average cluster size.

## Methodology

### Site Percolation Model

- A grid of size $L \times L$ is randomly populated with occupied sites based on a probability $p$.
- Clusters of connected sites are identified using neighbor connectivity (sites are neighbors if they share an edge).
- The percolation threshold $p_c$ is estimated by analyzing the probability of a spanning cluster forming as $p$ varies.

### Finite-Size Scaling

Given the computational limitations of simulating large systems, finite-size scaling is used to estimate critical exponents. The behavior of various quantities, such as the size of the percolating cluster and the average cluster size, is analyzed as a function of the system size $L$ and the distance from the critical probability.

## Results

- **Percolation Threshold ($p_c$):** Estimated at approximately 0.5919 for a grid of size 1500x1500, with a relative error of 0.13% compared to the theoretical value for an infinite system.
- **Fractal Dimension ($D$):** Calculated as \( 1.86 \pm 0.02 \).
- **Correlation Length Exponent ($\nu$):** Calculated as \( 1.30 \pm 0.02 \).
- **Order Parameter Exponent ($\beta$):** Calculated as \( 0.14 \pm 0.01 \).
- **Susceptibility Exponent ($\gamma$):** Calculated as \( 2.37 \pm 0.10 \).

## How to Run the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/SquareLatticePercolation.git
   cd SquareLatticePercolation
2. **Set Up the Environment**:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `.\env\Scripts\activate`
   pip install -r requirements.txt
3. **Run the Simulation**:
   Use the Jupyter notebook Percolation.ipynb to run the percolation simulation and analyze the results.

