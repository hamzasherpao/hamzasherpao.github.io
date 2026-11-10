---
layout: page
title: Discrete-Adjoint Shape Optimization
description: Adjoint-based aerodynamic shape optimization of a transonic wing and wind-turbine vortex generators
importance: 2
category: Simulation
---

**Goal.** Improve the aerodynamic performance of a wing and of wind-turbine vortex generators with gradient-based shape optimization, at a cost that does not grow with the number of design variables.

**Approach.**

- Built the optimization workflow around the discrete adjoint solver in ANSYS Fluent, with mesh morphing to update the geometry after each adjoint solution.
- Generated structured meshes in ANSYS ICEM, refined to y+ ≈ 0.9 at the wall.
- Validated both cases against wind-tunnel data before optimizing.
- **ONERA M6 transonic wing** (Mach 0.84, Re 12 million, k-ε model): optimized once without constraints and once with only the upper surface free to change.
- **Counter-rotating vortex generators on the NREL S809 wind-turbine airfoil** (Re 1 million, SST k-ω model): one pair of vortex generators with periodic sides, on a 5.6-million-cell mesh chosen from a six-grid independence study, optimized at the 14° stall angle.

**Results.**

- ONERA M6, unconstrained: drag reduced by 16.0%, lift-to-drag ratio increased by 20.7%.
- ONERA M6, upper-surface constraint: drag reduced by 9.6% at unchanged lift, lift-to-drag ratio increased by 13.3%.
- Vortex generators at stall: drag reduced by 29.5% and lift increased by 5.7%, raising the lift-to-drag ratio by 49.9% (from 25.1 to 37.7).

This was my M.S. thesis at Xi'an Jiaotong University.
