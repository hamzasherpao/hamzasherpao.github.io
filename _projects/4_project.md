---
layout: page
title: Underwater Wake Sensing and Localization
description: Estimating the upstream wake and the body's position behind a bluff body from embedded PVDF signals, in real time
importance: 2
category: Sensing
---

**Goal.** Use the same soft PVDF body to sense its surroundings: the scale of an upstream wake and the body's streamwise and lateral position relative to the upstream bluff body.

**Approach.**

- Recorded PVDF signals behind bluff bodies over a range of positions and flow speeds in a water channel.
- Benchmarked six estimators: linear, kernel, random forest, MLP, LSTM, and TCN.
- Tested generalization to unseen conditions, flow speeds, and measurement sessions, and found the best sensor placement through ablation.
- Deployed the estimator for live, causal inference on the streaming sensor data.

**Results.**

- Real-time estimation at about 36 ms per update in live water-channel tests.
- The estimates tracked flow-speed changes and followed streamwise repositioning within about 4 s.

This work is in progress, and a manuscript is in preparation.
