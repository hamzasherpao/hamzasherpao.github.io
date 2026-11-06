---
layout: page
title: Soft-Foil Proprioception
description: Reconstructing the dynamic shape of a soft foil in flow from its own embedded PVDF signals
importance: 1
category: Sensing
---

**Goal.** Let a soft body sense its own deformation. The PVDF film that harvests energy is also used as a sensor to reconstruct the body's midline shape while it moves in flow.

**Approach.**

- Built a multi-channel PVDF soft-body platform with a servo-actuated excitation rig in a water channel.
- Designed a 4-channel unity-gain buffer front end (OPA4134) that removes multiplexer crosstalk between high-impedance PVDF channels on a single-ADC DAQ (NI USB-6210).
- Automated hardware-synchronized acquisition in Python (NI-DAQmx and a Basler camera), so each camera frame is aligned with the PVDF voltage stream. The camera trigger is opto-isolated (PC817) to keep mains noise and ground loops out of the DAQ.
- Benchmarked five reconstruction models in MATLAB: kernel SVR, ARX, GRU, LSTM, and BiLSTM.

**Results.**

- The BiLSTM reconstructed the dynamic midline to 0.69 mm RMSE (R² = 0.83) on test flow conditions.
- The trailing-edge error was 0.62% of the body length.

A manuscript on this work is under review.
