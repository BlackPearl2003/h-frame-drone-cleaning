# Quickstart

This is the **fast path** to understand and reuse the H‑frame cleaning UAV.

## 1) What this repo gives you
- A proven **H‑frame X8** layout for bulky, shifting payloads (sprayer tank).
- A **sprayer module** using a diaphragm pump, 1 L tank, and **servo‑swept** nozzles.
- Baseline **flight modes**: Loiter / AltHold / RTL on Pixhawk 2.4.8 (ArduPilot).

For all background and evaluation, open `docs/B-08 Final Report.pdf`.

## 2) Minimum parts (starter BOM)
- **Frame:** H‑frame (custom or equivalent 550–650 class), carbon tubes
- **Motors/ESCs:** 8× matched BLDC + ESC for X8 coaxial
- **FCU:** Pixhawk 2.4.8 (ArduPilot)
- **Radio/GPS:** Telemetry link + GNSS
- **Battery:** High‑C LiPo
- **Sprayer:** 1 L tank, diaphragm pump (~5 L/min), 2× micro servos, 2× fan‑nozzles
- **Misc:** Mounts, dampers, wiring, power distribution

> See `docs/BOM.csv` for a lightweight template to fill with your exact choices.

## 3) Build in 60 minutes (overview)
1. Assemble H‑frame and mount the **X8 coaxial** propulsion.
2. Install **Pixhawk**, GPS, telemetry; verify arrow orientation.
3. Wire **power**: battery → PDB → ESCs; separate BEC for servos/pump if needed.
4. Install **sprayer**: tank → pump → T‑split → nozzles on a **servo sweep** bracket.
5. Flash **ArduPilot**, run radio/ESC calibrations, set **X8** motor order & directions.
6. Do a **tethered throttle test** without props → then with props (outdoors).

## 4) First flights (safe recipe)
- Start **AltHold** at 2–3 m AGL, no water.
- Check attitude/oscillations, voltage sag, GPS lock.
- Add **0.3–0.5 L** water → repeat.
- Validate **RTL** and failsafes before any facade job.

## 5) Results you can expect (baseline)
- Demonstrated **~6 min** with **3.5 kg payload** (AUW ~6 kg).
- Stable **3 m AGL** autonomous hover and manual window cleaning demo.
- See `docs/RESULTS.md` for plots to replicate with your logs.

## 6) Reuse & cite
If you use this, please cite the report and credit the authors.
