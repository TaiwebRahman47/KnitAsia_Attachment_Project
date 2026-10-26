# Industrial Problems and Solutions: A Case Study at Knit Asia Ltd.

![Knit Asia Limited](https://img.shields.io/badge/Status-Completed-success)
![Course](https://img.shields.io/badge/Course-IPE%20300%20Industrial%20Practice-blue)
![University](https://img.shields.io/badge/University-BUET-red)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains the comprehensive study, analysis, Matlab simulation scripts, and problem-solving methodologies developed during the industrial attachment at **Knit Asia Ltd.** as part of the course **IPE 300: Industrial Practice** at Bangladesh University of Engineering and Technology (BUET).

---

## 📌 Executive Summary

The primary objective of this project was to apply Industrial and Production Engineering (IPE) principles to real-world garment manufacturing challenges at Knit Asia Ltd. The study covers key operational areas including **Line Balancing**, **HVAC/Ventilation Optimization**, **Facility Layout Design**, **Quality Control (Pareto & Ishikawa Analysis)**, and **Ergonomics**.

### Key Contributions & Results:
- **Sewing Line Balancing:** Eliminated line bottlenecks, achieving the target output of **$75\text{ pcs/hr}$** using time study analysis.
- **Facility Layout Redesign:** Proposed an optimized linear layout for the Washing and Dyeing shop (Plant No. 1), yielding a **$4.54\%$ daily material handling cost reduction**.
- **Ventilation Optimization:** Calculated standard Air Changes per Hour ($\text{ACH} = 25.3$) and proposed an optimized fan/cooler arrangement to eliminate packaging area dead spots.
- **Quality Improvement:** Applied Pareto Charting ($80/20$ rule) and Fishbone (Ishikawa) diagrams to target top defects: **Skipped Stitches**, **Excess Threads**, and **Loose Stitches**.
- **Ergonomics:** Designed a 3D CAD model of an ergonomic, height-adjustable workstation chair in SolidWorks to mitigate lower back pain and static muscular load.

---

## 👨‍💻 Project Authors & Team

| Name | Student ID | Department / Institution |
| :--- | :--- | :--- |
| **Abrar Hamim Masih** | 1908021 | Dept. of IPE, BUET |
| **Narayon Dey Noyon** | 1908029 | Dept. of IPE, BUET |
| **An-Nur Taiweb Rahman** | 1908047 | Dept. of IPE, BUET |
| **Muhammad Shadab Sakib** | 1908050 | Dept. of IPE, BUET |

### Supervision:
* **Dr. Nikhil Ranjan Dhar** — *Professor, Dept. of IPE, BUET*
* **Rashik Ahnaf** — *Lecturer, Dept. of IPE, BUET*
* **Md. Tariqul Islam** — *DGM, HR, Knit Asia Ltd.*
* **Shahin Ahmed** — *Manager, IE, Knit Asia Ltd.*

---

## 🛠 Project Structure & Methodology

```
├── README.md
├── scripts/
│   ├── current_layout_distance.m     # MATLAB script for current layout material handling distance
│   └── proposed_layout_distance.m    # MATLAB script for proposed layout material handling distance
├── docs/
│   ├── KnitAsia_Attachment_Report.pdf
│   └── surveys/
└── assets/
    ├── images/
    └── cad_models/
```

---

## 📊 Summary of Problems & Engineering Solutions

### 1. HVAC & Air Circulation Optimization
* **Problem:** Identified localized dead spots and heat concentration in packaging areas despite high overall CFM.
* **Analysis:**
  * Total CFM Provided = $371,000\text{ CFM}$
  * Floor Volume = $55,000\text{ sq ft} \times 16\text{ ft} = 880,000\text{ cu ft}$
  * $\text{ACH} = \frac{\text{Total CFM} \times 60}{\text{Volume}} = 25.3$ (Exceeds ASHRAE standard recommended range of $6\text{--}12\text{ ACH}$).
  * Required Air Flow for 1,130 workers = $1,130 \times 25\text{ CFM} = 28,250\text{ CFM}$.
* **Solution:** Repositioned ceiling fans, reoriented air coolers toward dead spots, and adjusted exhaust fan placement for uniform flow distribution.

---

### 2. Line Balancing & Bottleneck Removal (Sewing Line 17)
* **Target Output:** $75\text{ pcs/hr}$
* **Problem:** Unbalanced line capacity ranging between $61\text{ pcs/hr}$ and $227\text{ pcs/hr}$, causing flow bottlenecks at tasks like *Side Panel Join*.
* **Solution Strategy:**
  * Merged *Chest Panel Join* and *Pocket Bag Servicing*.
  * Combined *Riser Label Join* and *Side Panel Join*.
  * Added 1 extra floater/operator to overloaded workstations.
  * Reassigned low-performing operators at critical tasks to expert operators.
* **Outcome:** Capacity across all operations successfully met or exceeded $75\text{ pcs/hr}$.

---

### 3. Washing & Dyeing Shop Layout Optimization
* **Problem:** High material handling costs due to long distance between washing and drying areas, alongside cross-contamination risks due to proximity of deep dyeing units.
* **Mathematical Formulation (Material Handling Cost):**

$$C_{\text{batch}} = \sum (D_i \times W_i \times R_i)$$

Where:
* $D_i$ = Distance between processes ($\text{m}$)
* $W_i$ = Average batch weight ($200\text{ kg}$)
* $R_i$ = Handling rate ($\$0.02/\text{kg}\cdot\text{m}$)

#### Layout Comparison Summary:

| Parameter | Current Layout | Proposed Layout | Improvement |
| :--- | :--- | :--- | :--- |
| **Dyeing to Washing Dist.** | $36.42\text{ m}$ | $41.94\text{ m}$ | Machine separation optimized ($\ge 0.5\text{m}$) |
| **Washing to Drying Dist.** | $61.24\text{ m}$ | $51.29\text{ m}$ | Distance reduced by $9.95\text{ m}$ |
| **Handling Cost / Batch** | $\$390.64$ | $\$372.92$ | Saved $\$17.72 / \text{batch}$ |
| **Daily Cost (10 batches)** | $\$3,906.40$ | $\$3,729.20$ | **$4.54\%$ Cost Savings/Day** |

---

### 4. Quality Control & Defect Analysis
A Pareto Analysis was performed on defect counts to isolate the "Vital Few" issues ($80/20$ rule):

```
Defect Distribution (Top 3):
1. Skipped Stitches    [18%] ████████████████████
2. Excess Threads      [15%] ███████████████
3. Loose Stitches      [12%] ████████████
```

* **Root Cause Diagnostics:** Constructed **Ishikawa (Fishbone) Diagrams** analyzing *Man, Machine, Method, Material, Measurement,* and *Environment* for each major defect type.

---

### 5. Ergonomic Workstation Chair Redesign
* **Problem:** High frequency of worker fatigue and lower back pain ($75\%$ reported occupational discomfort in shop floor survey).
* **Design Features (SolidWorks):**
  * **Lumbar Lordosis Support:** Curved backrest to maintain natural spinal geometry.
  * **Pressure Distribution:** Contoured seat pan to reduce intervertebral disc pressure.
  * **Dynamic Mobility & Adjustability:** Swivel base to reduce postural fixity, equipped with pneumatic height adjustment.

---

## 💻 MATLAB Code Execution

The distance calculation scripts for machine placement optimization can be executed in MATLAB as follows:

```matlab
% Example execution snippet for layout optimization script
run('scripts/proposed_layout_distance.m');
```

---

## 📜 References

1. **ASHRAE** (2017). *Ventilation for Acceptable Indoor Air Quality (Standard 62.1)*. Atlanta: ASHRAE.
2. **Ishikawa, K.** (1986). *Guide to Quality Control*. Tokyo: Asian Productivity Organization.
3. **McCormick, E. J.** (1993). *Applied Anthropometry, Work-Space Design, and Seating*. New York: McGraw-Hill.
4. **Niebel, B. W.** (2009). *Methods, Standards, and Work Design*. New York: McGraw-Hill.
5. **Tompkins, J. A.** (2010). *Facilities Planning*. Hoboken: Wiley.

---
*Submitted in partial fulfillment of the requirements for the degree of Bachelor of Science in Industrial and Production Engineering, BUET.*