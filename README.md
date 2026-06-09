# MD Simulation of Argon

A complete Molecular Dynamics (MD) simulation engine built from scratch in Python to study the behavior of Argon atoms interacting through the Lennard-Jones potential.

This project was developed as part of the course:

**Electronic Structure & Atomistic Modeling of Materials**

---

## Project Overview

The simulation models Argon atoms in a periodic simulation box and investigates the solid-to-liquid phase transition using Molecular Dynamics techniques.

Features implemented include:

- Lennard-Jones (LJ) pair potential
- Periodic Boundary Conditions (PBC)
- Face-Centered Cubic (FCC) lattice generation
- Velocity Verlet time integration
- Verlet Neighbor Lists
- NumPy vectorized force calculations
- Radial Distribution Function (RDF)
- Mean Square Displacement (MSD)
- Diffusion coefficient calculation
- Argon melting study

---

## Physics Implemented

### Lennard-Jones Potential

The interaction between Argon atoms is modeled using the Lennard-Jones potential:

V(r) = 4ε[(σ/r)^12 − (σ/r)^6]

A shifted potential is used to ensure continuity at the cutoff radius.

### Periodic Boundary Conditions

Atoms leaving one side of the simulation box re-enter from the opposite side using the minimum image convention.

### Velocity Verlet Integrator

Time evolution is performed using the Velocity Verlet algorithm, providing good energy conservation and numerical stability.

### Neighbor List Optimization

Verlet neighbor lists are implemented to reduce computational complexity and improve simulation performance.

---

## Analysis

### Radial Distribution Function (RDF)

Used to identify structural ordering and distinguish solid and liquid phases.

### Mean Square Displacement (MSD)

Used to analyze atomic diffusion and calculate diffusion coefficients.

---

## Melting Study

Simulations were performed at:

- T* = 0.2
- T* = 0.4
- T* = 0.6
- T* = 0.8
- T* = 1.0

Results indicate a melting transition near:

T* ≈ 0.6 – 0.8

which agrees with literature values for Lennard-Jones systems.

---

## Technologies Used

- Python
- NumPy
- Matplotlib
- Jupyter Notebook

---

## Repository Structure

├── MD_Simulation_Argon.ipynb
├── MD_Simulation_Report.pdf
├── README.md

---

## Key Outcomes

- Built a complete MD engine from scratch
- Verified energy conservation
- Implemented optimized force calculations
- Observed solid-to-liquid phase transition
- Calculated diffusion coefficients
- Analyzed structural changes using RDF and MSD

---

## Author

Thanumalayaperumal

M.Tech
