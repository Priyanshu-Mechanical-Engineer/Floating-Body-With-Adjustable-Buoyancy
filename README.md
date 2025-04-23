# 🛶 Floating Body with Adjustable Buoyancy

> A smart buoyancy-control system using a dual-pump mechanism for precision water displacement.

## 📌 Overview

This project demonstrates the **design and implementation** of a **floating body with adjustable submersion levels**, controlled in real-time using a water intake and drainage system. The system applies principles from **fluid mechanics** and **buoyancy** using **PVC-based construction**, **arduino-pump control**, and **metacentric height testing**.

> Developed as part of the ME303 Thermo-Fluid Lab.

---

## 🎯 Objectives

- 🔧 Design a sealed cylindrical floating body using PVC and acrylic
- 📉 Implement a dual-pump system to dynamically control buoyancy
- 🧪 Analyze stability using metacenter (M) and center of gravity (G) relationships
- 🧠 Apply Archimedes' principle to determine equilibrium

---

## ⚙️ Components Used

| Component        | Description                                      |
|------------------|--------------------------------------------------|
| **PVC Pipe**     | Ø16cm, Length: 27cm — Main body                  |
| **Acrylic Sheets** | Ø16cm — Seals at both ends                     |
| **Pumps**        | 1 inlet + 1 outlet submersible DC pump           |
| **Adhesive**     | Araldite — Waterproof bonding                    |
| **Controller**   | Arduino Uno with manual switch interface         |

---

## 🔬 Working Mechanism

The floating body contains a **hollow chamber** to manage water volume. Two pumps:
- 🟢 *Inlet pump* increases weight → more submersion
- 🔴 *Outlet pump* reduces water → less submersion

<details>
<summary>Click to view full working animation and experiment setup images</summary>

![Design Diagram](docs/design_diagram.png)  
![Full Setup](media/full_setup_photo.jpg)  
![Working Mechanism](docs/working_mechanism.gif)

</details>

---

## 📈 Experimental Observations

### Filling Time Analysis:

| Submersion % | Time (s) |
|--------------|----------|
| 25%          | 6        |
| 50%          | 9.12     |
| 75%          | 6.17     |
| 100%         | 2.71     |

### Emptying Time Analysis:

| From (%) | To (%) | Time (s) |
|----------|--------|----------|
| 100      | 75     | 60       |
| 75       | 50     | 70       |
| 50       | 25     | 85       |

![Submersion Time Graph](media/submersion_graphs.png)

---

## 📐 Metacentric Height (Stability Test)

- ✅ *Stable:* When M > G → Restoring torque observed
- ❌ *Unstable:* When G > M → Capsizing behavior

![Stability Setup](media/metacentric_experiment.png)

---

## 💡 Learnings & Future Work

- Precision in **GM calculations** is crucial for marine design
- Enhance control via **automatic feedback loops (water sensor + Arduino PID)**
- Miniaturize design for **underwater ROVs, sensor platforms**

---

## 📁 Project Files

- [`floating_body_project_report.pdf`](report/floating_body_project_report.pdf)
- [`arduino_pump_controller.ino`](src/arduino_pump_controller.ino)

---

## 🛠️ Setup Instructions

1. Connect pumps to Arduino via relays
2. Use switches or serial input to activate fill/empty
3. Monitor submersion visually or via ultrasonic sensor (future upgrade)

---

## 📜 License

MIT License — Feel free to adapt for research or academic use!

---

## ✍️ Authors

- **[Your Full Name]** — Mechanical Engineering @ [Your Institute]
- **Mentor/Guide** (if applicable)

---

## 🤝 Contributions

Pull requests are welcome for improvements or alternative control algorithms!

