# Build & Setup Guide

## Frame & layout
- H‑frame gives better **payload placement** and **COG margin** than a compact X‑frame.
- Keep noisy / wet components (pump, tubing) **downwind** of the flight controller.

## Motor mixing (ArduPilot)
1. In Mission Planner → **Frame Type** → select **X8**.
2. Verify motor numbers and directions using the **Motor Test** tool **without props**.
3. Coaxial pairs counter‑rotate; top/bottom prop pitch must match the rotation.

## Sprayer wiring
- Use a **separate BEC** (or buck) for servos/pump to avoid brownouts.
- Pump via a MOSFET or relay module; test current draw at max flow.
- Servo sweep on **AUX** outputs; set PWM min/mid/max and sweep frequency.

## Tuning essentials
- Start with default PIDs for 10–13" prop class; log **ATT, CTUN, RCOU, BAT**.
- Increase D‑term cautiously if you see overshoot; avoid oscillations with a full tank.
- Re‑autotune when payload mass **changes by >10%**.

## Failsafes
- **RTL** on RC loss and low battery.
- **Geo‑fence** around the test area; land mode as backup.
- Add a **physical arming switch** and **prop guards** when testing near people/windows.
