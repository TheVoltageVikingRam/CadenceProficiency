# CMOS Half Adder Design in Cadence Virtuoso

This repository presents the full-custom design and verification of a **CMOS Half Adder** using **Cadence Virtuoso**. The project includes schematic creation, symbol generation, layout design, DRC/LVS checks, transient simulation, parasitic extraction, and power estimation for one operation cycle.

---

## 📁 Table of Contents  
- [🧩 Schematic](#-schematic)  
- [🎛️ Symbol View](#-symbol-view)  
- [🧪 Testbench Setup](#-testbench-setup)  
- [📈 Transient Simulation](#-transient-simulation)  
- [🧱 Layout](#-layout)  
- [✅ DRC and LVS Checks](#-drc-and-lvs-checks)  
- [🔍 Schematic vs Layout Matching](#-schematic-vs-layout-matching)  
- [🧠 Parasitic Extraction (RCX)](#-parasitic-extraction-rcx)  
- [⚡ Energy Estimation](#-energy-estimation)  
- [🛠️ Tools Used](#-tools-used)  
- [👤 Author](#-author)

---

## 🧩 Schematic  
The half adder circuit is designed using CMOS logic to compute both **SUM** and **CARRY** outputs for two binary inputs.

![Schematic](./Schematic_HA.png)

---

## 🎛️ Symbol View  
A custom symbol view was generated to simplify testbench integration and hierarchical design.

![Symbol](./Symbol_HA.png)

---

## 🧪 Testbench Setup  
The testbench applies all binary combinations of inputs `A` and `B` to validate SUM and CARRY functionality.

![Testbench](./Test_bench_setup_HA.png)

---

## 📈 Transient Simulation  
Transient waveform confirms correct logical behavior of the half adder. SUM and CARRY outputs respond correctly to all input transitions.

![Transient](./Transient_Response_HA.png)

---

## 🧱 Layout  
The full-custom layout of the half adder was implemented using standard 90nm design rules in Cadence Virtuoso.

![Layout](./Layout.png)

---

## ✅ DRC and LVS Checks  

### ✔️ DRC (Design Rule Check)  
The layout passed all DRC checks with no violations, verified using **Assura**.

![DRC](./DRC_Clearance.png)

### ✔️ LVS (Layout vs Schematic)  
The layout matches the schematic functionally and electrically.

![LVS](./LVS_Clearance.png)

---

## 🔍 Schematic vs Layout Matching  
Graphical matching confirms the layout connectivity aligns with the schematic netlist.

![Match](./Layout_and_schematic_match.png)

---

## 🧠 Parasitic Extraction (RCX)  
Post-layout parasitic extraction was performed using Assura RCX to analyze layout-dependent resistive and capacitive effects.

![RCX](./RCX_Run.png)

---

## ⚡ Energy Estimation  
Estimated switching energy for one cycle of half adder operation, based on post-layout simulation.

![Energy](./Energy_one_cycle_HA.png)

---

## 🛠️ Tools Used  
- **Cadence Virtuoso** – Schematic, Layout, and Symbol Design  
- **Spectre** – Transient Simulation  
- **Assura** – DRC, LVS, RCX  
- **ADE L** – Waveform Viewing & Power Estimation

---

## 👤 Author  
**Ram Tripathi**

