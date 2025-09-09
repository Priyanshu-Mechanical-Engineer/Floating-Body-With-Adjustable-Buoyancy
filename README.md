# 🛶 Floating Body With Adjustable Buoyancy

> An experimental prototype that demonstrates dynamic buoyancy control and floating body stability using a dual-pump PVC system. Applicable to marine and defense industries for intelligent submerged systems.

---

## 📌 Project Overview

This project demonstrates the stability of floating bodies and real-time adjustable buoyancy using a dual-pump system inside a sealed PVC pipe structure. The setup allows precise submersion control between 10% to 90% of the body’s volume.

Designed for experimental, marine, and defense applications such as:
- 🛳️ Ships and underwater vehicles
- 🛡️ Torpedoes, naval mines, and autonomous aquatic drones

---

## 🎯 Motivation

Understanding and demonstrating concepts like **metacentric height**, **center of gravity**, and **Archimedes’ Principle** is crucial for both academic and industrial marine design.

This project bridges theoretical understanding and practical implementation of:
- Controlled buoyancy systems
- Submersion dynamics and fluid stability
- Structural design for floating systems

---

## 🧪 Project Goals

- ✅ Design and build a floating cylindrical body with sealed ends
- ✅ Implement a pump-driven system to control the internal water level (i.e., weight)
- ✅ Maintain and measure stability at different submerged states
- ✅ Experimentally calculate the **metacentric height (GM)** and observe its effects on stability

---

## 🧱 Experimental Design

### 🔧 Materials Used
| Component        | Description                                      |
|------------------|--------------------------------------------------|
| **PVC Pipe**     | Ø16cm, Length: 27cm — Main structure              |
| **Acrylic Sheets** | Ø16cm — Sealed ends for waterproofing          |
| **Araldite**     | Waterproof adhesive to secure acrylic ends       |
| **Pumps**        | 1 inlet + 1 outlet submersible DC pumps          |
| **Miscellaneous**| Valves, tubing, mounting frame, manual switch   |

### 📐 Volume Calculations
- **Volume of Cylinder**:  
  \( V = \pi R^2 h = 3.14 \times 0.08^2 \times 0.27 = 5.4 \, L \)
- **Pipe Density**: 1330 kg/m³  
- **Buoyant Force**: Calculated via Archimedes' Principle \( F_b = \rho V g \)

---

## ⚙️ Working Mechanism

- 💧 **Water Intake** increases weight → more submersion  
- 💨 **Water Drainage** reduces weight → less submersion  
- 🧠 System is manually controlled via switchboard interface connected to pumps

<details>
<summary>🖼 Click to view setup and mechanism visuals</summary>

![Design Diagram]([docs/design_diagram.png](https://github.com/user-attachments/assets/70bcc30e-4117-438e-bf2a-729d912dfbd3))  
![Prototype Setup](https://github.com/user-attachments/assets/42f2f616-7cdb-45d4-b936-3ac8d98dff50)  
![Working Mechanism](docs/working_mechanism.gif)

</details>

---

## 📊 Experimental Results

### 🧃 Filling Timings:

| Submersion % | Time Taken (s) |
|--------------|----------------|
| 25%          | 6.00           |
| 50%          | 9.12           |
| 75%          | 6.17           |
| 100%         | 2.71           |

### 🌊 Emptying Timings:

| From → To (%) | Time Taken (s) |
|---------------|----------------|
| 100 → 75      | 60             |
| 75 → 50       | 70             |
| 50 → 25       | 85             |
| 25 → 0 (2.5cm) | 45             |

![Graph](media/submersion_graphs.png)

---

## 🧠 Stability Analysis

**Metacentric Height (GM):**
- Stable when M > G → Body returns to upright position
- Unstable when G > M → Tendency to capsize

Observed experimentally using tilt method and plotted:
- Tilt angle vs displacement of center of buoyancy
- Restoration behavior based on metacenter location

![Stability Test](media/metacentric_experiment.png)

---

## 💡 Key Features

- ✅ Real-time submersion adjustment (10%–90%)
- ✅ Accurate observation of restoring torque
- ✅ Visualization of fluid dynamics and stability theory
- ✅ Portable and modular setup for future iterations

---


---

## 🌍 Applications

### 🛳️ Marine Engineering:
- Buoyancy-controlled floats
- Ship stability modeling
- Smart mooring systems

### 🛡️ Defense:
- Torpedoes & underwater drones
- Smart naval mines
- Research submersibles

---

## 🚀 Future Improvements

- Integrate ultrasonic water level sensors  
- Automate pump control using PID feedback system  
- Wireless data logging for real-time analysis  
- CFD modeling for further performance prediction  

---

## ✍️ Authors

- **Priyanshu Rao** – Mechanical Engineering @ [IIT ROPAR]  
- **Faculty/Guide Name** – Chandra Shekhar Sharma (IIT ROPAR)

---



