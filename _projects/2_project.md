---
layout: page
title: Discrete-Adjoint Shape Optimization
description: Adjoint-based aerodynamic shape optimization of a transonic wing and wind-turbine vortex generators
importance: 2
category: Simulation
---

**Goal.** Improve the aerodynamic performance of a wing and of wind-turbine vortex generators with gradient-based shape optimization, at a cost that does not grow with the number of design variables.

**Approach.**

- Used the discrete adjoint method in ANSYS Fluent, with meshes built in ANSYS ICEM.
- Applied it to the ONERA M6 wing and to vortex generators on the NREL S809 airfoil, with and without geometric constraints.
- Ran a RANS simulation and grid-convergence study on the DLR F6 wing-body configuration and validated it against experimental data.

**Results.**

- ONERA M6 wing: lift-to-drag ratio improved by 20.7% (unconstrained) and 13.3% (constrained).
- Vortex generators: lift-to-drag ratio increased by 49.9% at the stall angle.

This was my M.S. thesis at Xi'an Jiaotong University.
