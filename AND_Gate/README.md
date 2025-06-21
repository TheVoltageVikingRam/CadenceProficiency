
# CMOS AND Gate Design in Cadence Virtuoso

This repository documents the complete **CMOS AND Gate** design flow in **Cadence Virtuoso**, covering schematic creation, layout, simulation, verification (DRC/LVS), and power analysis.

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

## 📐 Schematic  
The AND gate is implemented using CMOS logic with pull-up PMOS and pull-down NMOS networks.

![CMOS Schematic](./CMOS_AND_Gate_schematic.png)

---

## 🔣 Symbol View  
A symbol was generated from the schematic for hierarchical testbench connection.

![Symbol](./AND_Gate_Symbol.png)

---

## 🧪 Testbench  
The testbench is used to provide input stimulus and observe output response.

![Testbench](./AND_Gate_tb.png)

---

## 📊 Transient Simulation  
Transient simulation validates the functionality of the AND gate under dynamic conditions.

![Transient Waveform](./AND_Gate_transient_waveform.png)

---

## 🧱 Layout  
The full custom layout of the AND gate was drawn following foundry design rules.

![Layout](./AND_GATE_Layout.png)

---

## ✅ DRC and LVS Checks

- ✅ **No DRC Errors:**  
  Verified using DRC tool — no design rule violations.

  ![DRC](./No_DRC_errors_AND.png)

- ✅ **LVS Clean:**  
  The layout matches the schematic with no mismatches.

  ![LVS](./LVS_Clearance.png)

---

## 🔄 Schematic vs Layout Matching  
A visual confirmation of netlist and connectivity matching between schematic and layout.

![Layout vs Schematic Match](./Layout_and_Schematic_Match.png)

---

## ⚡ Energy Estimation  
Post-layout transient waveform was used to estimate switching energy consumption.

![Energy](./Energy_Calculation_AND.png)

---

## 🧰 Tools Used  
- **Cadence Virtuoso** – Schematic, Symbol, and Layout Design  
- **Spectre** – Transient Simulation  
- **Assura** – DRC and LVS  
- **ADE XL** – Waveform analysis and power estimation  

---

## 👨‍💻 Author  
**Ram Tripathi**

