# Deloitte Australia – Data Analytics Job Simulation (Forage)

This repository contains my completed work for the **Deloitte Australia Data Analytics Job Simulation** on [Forage](https://www.theforage.com/). The program simulates real-world tasks performed by Deloitte's Data Analytics team and covers both **data analysis** and **forensic technology** work streams.

---

## Project Overview

The client, **Daikibo Industrials**, is a global manufacturer of heavy machinery operating four factories across the world. As part of a digital transformation initiative, Daikibo installed telemetry devices on every machine to monitor operational health in real time.

Deloitte was engaged to:
1. Build a **dashboard** that shows machine downtime across factories and device types.
2. Investigate an **internal equality/fairness** concern using HR data.

---

## Task 1 — Data Analysis: Daikibo Telemetry Dashboard

**Objective:** Help the client visualize how much time each machine spends in an unhealthy (downtime) state, broken down by factory and by device type.

**Tool used:** Tableau Desktop Public Edition

**Dashboard views:**
- **Downtime Per Factory** — bar chart comparing total unhealthy time across the four Daikibo factories (Berlin, Meiyo, Seiko, Shenzhen).
- **Downtime Per Machine** — bar chart comparing total unhealthy time across device types (AirWrench, CNC, ConveyorBelt, Furnace, HeavyDutyDrill, LaserCutter, LaserWelder, MetalPress, SpotWelder).
- **Daikibo Telemetry Dashboard** — combined dashboard view.

**Key findings:**
- **daikibo-factory-seiko** and **daikibo-shenzhen** account for the majority of downtime.
- **LaserCutter** and **LaserWelder** are by far the most problematic machine types, suggesting maintenance efforts should prioritize these devices.

---

## Task 2 — Forensic Technology: Equality Classification

**Objective:** Classify equality scores across factories and job roles to flag potentially discriminatory patterns in HR data.

**Tool used:** Microsoft Excel

**Logic applied** (nested IF formula):
```excel
=IF(ABS(C2)<=10,"Fair",IF(ABS(C2)<=20,"Unfair","Highly Discriminative"))
```

**Classification rules:**
| Equality Score (absolute) | Classification |
|---|---|
| 0 – 10 | Fair |
| 11 – 20 | Unfair |
| > 20 | Highly Discriminative |

**Key findings:** Several roles at **Daikibo Factory Meiyo** and **Daikibo Factory Seiko** were flagged as *Highly Discriminative*, warranting further investigation by Deloitte's forensic team.

---

## How to Open the Files

- **`Project.twb`** — open with [Tableau Desktop](https://www.tableau.com/products/desktop) or the free [Tableau Public](https://public.tableau.com/).
- **`Deloitte_Australia.pdf`** — open with any PDF reader to view the final submission screenshots.

---

## Certificate

Completed via [Forage – Deloitte Australia Data Analytics Job Simulation](https://www.theforage.com/simulations/deloitte-au/data-analytics-s5zy).

---

## Contact

Feel free to connect with me on LinkedIn or open an issue if you have any questions about the project!
[LinkedIn](https://www.linkedin.com/in/mdabdullah-amin)
