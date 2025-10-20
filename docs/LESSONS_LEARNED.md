# Lessons Learned (Read Before You Build)

These are the mistakes we made so you don’t have to.

1. **COG shifts with water**  
   - Keep the tank as close to the **CG plane** as possible; use a **wide H‑frame stance**.
   - Re‑check balance **full vs empty**.

2. **Brownouts from pump/servos**  
   - Power the sprayer from a **separate BEC/buck**. Do NOT pull from the FCU 5 V rail.

3. **Crosswind instability during spray**  
   - Start at **low flow**, short bursts; increase spray only after attitude stays stable.

4. **Wrong motor order on X8**  
   - Always run **Motor Test** without props first; label pairs with tape.

5. **Autotune with changing mass**  
   - Autotune with **mid‑tank mass**. Retune if payload changes >10%.

6. **Wet electronics**  
   - Route **all tubing downwind**; shield FCU and telemetry with a light splash cover.

7. **Testing too close to glass**  
   - Validate RTL, failsafes, and hover endurance **far from the building** before facade ops.
