---
title: "Adaptive traffic signals - GPS probes instead of loop detectors"
excerpt: "One thesis - vehicle GPS can replace buried loop detectors - matured through four implementations, ending on a Raspberry Pi intersection running Webster's formula."
collection: portfolio
order: 7
redirect_from:
  - /portfolio/07-adaptive-traffic-signals/
group: Infrastructure
---

This project tests whether vehicle GPS data can replace buried loop detectors as a traffic signal controller's input. The idea matured through four implementations over 2025-2026:

1. A concept simulation proving the idea end to end.
2. A modular pygame engine (about 1,900 lines) with the controller logic isolated from the visualization.
3. An A/B validation in SUMO microsimulation against a fixed-time baseline.
4. A working Raspberry Pi intersection running Webster's optimal-cycle formula on twelve physical LEDs, with a live Flask web dashboard.

The point of the arc is the discipline: the same idea re-tested at each level of fidelity, ending on hardware you can hold.

**Stack:** Python, pygame, SUMO/TraCI, Raspberry Pi GPIO, Flask.

*Client work; the code is private.*
