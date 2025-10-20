# H-Frame Drone for Cleaning Solar Panels and High-Rise Buildings

**Authors:** Chaya R, Mohit Mohan, Venu V Muthyala  
**Institution:** Nitte Meenakshi Institute of Technology (NMIT), Bengaluru  
**Advisor:** Dr. Murthy M  
**Academic Year:** 2024–25

> Portfolio-ready repository for my final-year project. This repo includes a polished README, the full project report (PDF), and pointers to results and future work.

---

## 🔎 Abstract (short)
We designed and built an **H-frame, coaxial-quad (X8) UAV** with an integrated **sprayer module** to clean **high‑rise building facades** and **solar panels**. The platform uses a **Pixhawk 2.4.8** flight controller, supports **pilot-in-the-loop** assisted modes (Loiter, Alt‑Hold, RTL), and carries a **1 L tank** with a **diaphragm pump** (~**5 L/min**) and **servo‑swept nozzles** for wide coverage. In testing, the system achieved **~6 minutes** flight time with a **3.5 kg payload** (total takeoff mass ~**6 kg**). We validated autonomous hover and manual window‑cleaning missions, demonstrating feasibility of aerial cleaning with H‑frame stability and payload distribution advantages.

> Full details and evaluation are in **`/docs/B-08 Final Report.pdf`**.

## 🧰 Tech Stack
- **Airframe:** H‑frame, coaxial‑quad (X8)
- **FCU:** Pixhawk 2.4.8 (ArduPilot stack)
- **Propulsion:** BLDC + ESCs (X8 coaxial layout)
- **Payload:** 1 L tank, diaphragm pump (~5 L/min), dual sweeping servos
- **Comms/GCS:** Mission Planner
- **Onboard Algorithms:** PID/EKF (ArduPilot), motor‑mixing for X8
- **Materials:** Carbon‑fiber tubes, custom frame components

## 📌 Key Specifications
| Subsystem | Spec |
|---|---|
| Frame | H‑frame (industrial stability & payload distribution) |
| Configuration | Coaxial X8 |
| Flight Controller | Pixhawk 2.4.8 |
| Battery | High‑C LiPo (per report BOM) |
| Payload | Sprayer: 1 L tank + diaphragm pump (~5 L/min) + 2× servos |
| Tested Flight Time | ~6 min at 3.5 kg payload (≈6 kg AUW) |
| Modes | Loiter, Alt‑Hold, RTL failsafe |
| Mission Types | Autonomous hover, manual facade cleaning |

## 🧪 Results (from the report)
- **Autonomous hover:** Stable at **3 m AGL** with GPS lock.  
- **Manual window clean:** Demonstrated sweeping spray coverage and attitude stability.  
- **Logs:** GPS track, altitude, voltage, attitude over time, and airspeed plots.

(See the *Results and Analysis* chapter in the PDF for figures and tables.)

## 🧭 Why H‑frame?
H‑frames offer **better payload placement and stability** (especially with bulky or sliding loads) and handle **COG shifts** and **crosswinds** more gracefully than compact X‑frames—ideal for cleaning tasks where the sprayer mass and fluid dynamics change during flight.

## 📂 Repository Structure
```
h-frame-drone-cleaning/
├─ README.md                 # You are here
├─ docs/
│  └─ B-08 Final Report.pdf  # Full thesis/report
└─ images/                   # Add photos & figures here (optional)
```

## 🚀 How to Use
1. Open the report in **`docs/B-08 Final Report.pdf`** for the full design, math, and tests.
2. Add your flight photos/short clips to **`/images`** and embed them in the README.
3. (Optional) Add a short **demo video** link (YouTube/Drive).

## 🔗 Citation
If you reference this work, please cite the report (see *Publication Details* section inside the PDF).

## 👤 About Me
I’m **Mohit Mohan** (GitHub: [BlackPearl2003](https://github.com/BlackPearl2003)) — UAV and embedded‑systems engineer focused on **industrial drones** (cleaning, inspection) and **education hardware**.

## 📜 License
MIT License © 2025 Mohit Mohan
