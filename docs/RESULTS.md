# Results & How to Replicate

## What we measured
- **Hover test** at 3 m AGL
- **Manual facade/window cleaning**
- Logs: GPS track, altitude, voltage, pitch/roll/yaw, airspeed

## Key numbers (from the report)
- ~**6 min** flight with **3.5 kg** payload (AUW ~6 kg)
- Stable attitude in hover; moderate cleaning effectiveness (prototype sprayer)

## How you can reproduce
1. Enable logs: `LOG_BITMASK` → default + ATTITUDE, CTUN, BAT.
2. Fly 2–3 short hovers with increasing water mass.
3. Download logs (`.bin`) → Mission Planner → **Review a Log** → export CSV.
4. Plot: altitude vs time, voltage vs time, roll/pitch/yaw vs time, GPS track.

> You can drop your plots as PNGs into `/images` and link them here.
