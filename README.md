# Foil and Darrieus OpenFOAM Simulations

This repository contains the basic files allowing the CFD simulation of a Darrieus turbine and a fixed airfoil on `OpenFOAM v2106`.

## What is this repository for?

- Basic files for openfoam simulation
- OpenFoam Versions : v2106plus

## Description of cases:

- These are unsteady 2D URANS simulations with a k-omega SST turbulence model.
- The folders contain the meshes and the solver settings (discretization scheme, pimple algorithm, time step, etc.).

### Darrieus

- The turbine employed is the one tested by [Li et al., 2016](https://www.sciencedirect.com/science/article/abs/pii/S0360544216303334).
-  It is H-rotor Darrieus turbine. 
-  Below are some of these characteristics:


| Parameter           | Value     |
| -----------        | -----------|
| blade number     | 2          |
| Radius R (m)        |  0.85       |
| Chord c (m)        | 0.225      |
| c/R                | 0.265      |
| pitch angle $\beta$ (°) | 6          |
| Blade Profil     | NACA 0015   |
| Tip-Speed-Ratio                | 2.29       |


### Foil

- This is a 2D fixed airfoil simulation.
- This profile has been obtained by the authors by applying a conformal mapping to a NACA 0015 profile.
- It has a camber of 4.87%. 
- This simulation is done at a Reynold number $Re = 1.56\times 10^5$ and an angle of attack AoA = 12°.
