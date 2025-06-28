
# CMOS AND Gate Design in Cadence Virtuoso

This repository presents the full-custom design flow of a **CMOS AND Gate** using **Cadence Virtuoso**. It includes schematic creation, layout design, simulation results, DRC/LVS checks, and energy estimation.

---

## 📁 Table of Contents  
- [Schematic](#schematic)  
- [Symbol View](#symbol-view)  
- [Testbench](#testbench)  
- [Transient Simulation](#transient-simulation)  
- [Layout](#layout)  
- [DRC and LVS Checks](#drc-and-lvs-checks)  
- [Schematic vs Layout Matching](#schematic-vs-layout-matching)  
- [Energy Estimation](#energy-estimation)  
- [Tools Used](#tools-used)  
- [Author](#author)

---

## 🧩 Schematic  
The AND gate is implemented using CMOS logic, with a PMOS pull-up network and NMOS pull-down network.

![CMOS Schematic](./CMOS_AND_Gate_schematic.png)

---

## 🎛️ Symbol View  
A custom symbol was created for hierarchical testbench integration.

![Symbol](./AND_Gate_Symbol.png)

---

## 🧪 Testbench  
The testbench provides input stimulus (`A`, `B`) and captures the output waveform of the AND gate.

![Testbench](./AND_Gate_tb.png)

---

## 📈 Transient Simulation  
Spectre transient analysis was used to validate correct functionality of the logic gate.

![Transient Waveform](./AND_Gate_transient_waveform.png)

---

## 🧱 Layout  
The layout was drawn manually following GPDK 90nm design rules for fabrication compatibility.

![Layout](./AND_GATE_Layout.png)

---

## ✅ DRC and LVS Checks  

### ✔️ DRC: Design Rule Check  
No DRC violations were found using Assura.

![DRC](./No_DRC_errors_AND.png)

### ✔️ LVS: Layout vs Schematic  
The layout netlist matches the schematic exactly with no mismatches.

![LVS](./LVS_Clearance.png)

---

## 🧩 Schematic vs Layout Matching  
Visually confirms that the physical layout corresponds to the intended circuit schematic.

![Layout vs Schematic Match](./Layout_and_Schematic_Match.png)

---

## ⚡ Energy Estimation  
Post-layout simulation results were analyzed to estimate switching energy of the gate.

![Energy](./Energy_Calculation_AND.png)

---

## 🛠️ Tools Used  
- **Cadence Virtuoso** – Schematic, Symbol, and Layout Design  
- **Spectre Simulator** – Transient Analysis  
- **Assura/Calibre** – DRC and LVS Checks  
- **ADE XL** – Power and Energy Analysis

---

## 👤 Author  

**Ram Tripathi**  
Roll No: 22HEL2231  
B.Tech in Electronics – University of Delhi & IIT Madras  
Samsung Fellow (Grade-1) – India Semiconductor Mission  
Mentor: Prof. Mannoj Saxena

---

## 📄 License  
This project is licensed under the [MIT License](./LICENSE).
