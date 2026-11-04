---
title: "Stormwater trash interceptor - IoT fill monitoring (patent pending)"
excerpt: "A load-cell system that tells a crew when a stormwater trash interceptor is actually full, by correlating net drag against stream flow."
collection: portfolio
order: 6
redirect_from:
  - /portfolio/06-iot-trash-interceptor/
group: Infrastructure
---

This system tells a crew when a stormwater trash interceptor's net is actually full. Today interceptors get serviced on a calendar, not on need: too early wastes a crew trip, too late means trash escapes and the device strains the culvert.

The interesting part is not the hardware, it's the disambiguation. Tension alone is ambiguous: a fast-running stream pulls on an empty net as hard as debris pulls on a full one. The device correlates drag against water flow rate to separate the two - normal flow plus high drag raises a maintenance alarm; high flow plus high drag is expected and no action is taken. That correlation is what turns a strain reading into a maintenance decision.

My scope was the software side - Azure IoT Hub ingestion, the time-series data model, threshold alerting, and the monitoring dashboard. It retrofits existing interceptors (it is not the trash trap itself).

**Patent:** "Systems and Methods for IoT Sewer Management" - non-provisional application filed by Ardurra.

**Stack:** Arduino, HX711 load-cell amplification, cellular telemetry, Azure IoT Hub, time-series alerting, monitoring dashboard.
