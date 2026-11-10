---
layout: page
title: Tube-Launched MAV
description: Design and analysis of a miniature air vehicle with foldable wings, launched from a tube
importance: 3
category: Simulation
---

**Goal.** Design a miniature air vehicle that stows in a 127-mm (5-inch) launch tube and deploys foldable wings and twin tails after launch.

**Approach.**

- Sized the aircraft with a thrust-to-weight and wing-loading (T/W–W/S) study over nine design points, and matched the motor, battery and propeller.
- Estimated the aerodynamics, weights and performance, and defined the flight envelope (load factors +5/−2).
- Designed a pneumatic tube launcher and modeled the launch dynamics.
- Designed a roll controller and a lateral-directional stability augmentation system in MATLAB/Simulink, using stability derivatives from the Tornado vortex-lattice code.
- Modeled the aircraft in CATIA and analyzed the external flow in ANSYS Fluent.

**Results.**

- The sizing study showed that the thrust-to-weight ratio should rise from 0.59 to 1.3.
- The launcher needs 4.6 bar to reach an exit speed of about 20 m/s at a 30° launch angle.
- The stability augmentation system stabilizes the roll rate and roll attitude.

This was my B.S. thesis at the Institute of Space Technology, Islamabad.
