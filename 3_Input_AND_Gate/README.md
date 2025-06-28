
# CMOS 3-Input AND Gate Design in Cadence Virtuoso

This repository showcases the complete design flow of a **CMOS 3-Input AND Gate** using **Cadence Virtuoso**, including schematic, symbol creation, testbench setup, transient simulation, layout drawing, and verification using **Assura**.

---

## 📁 Table of Contents  
- [Schematic](#schematic)  
- [Symbol View](#symbol-view)  
- [Testbench](#testbench)  
- [Transient Simulation](#transient-simulation)  
- [Layout](#layout)  
- [DRC and LVS Checks](#drc-and-lvs-checks)  
- [Schematic vs Layout Matching](#schematic-vs-layout-matching)  
- [Tools Used](#tools-used)  
- [Author](#author)

---

## 🧩 Schematic  
The 3-input AND gate is implemented using CMOS logic with pull-up PMOS and pull-down NMOS networks.

![Schematic](./3_Input_AND_Schematic.png)

---

## 🎛️ Symbol View  
A symbol was generated from the schematic to enable hierarchical design and testbench integration.

![Symbol](./3_Input_AND_Symbol.png)

---

## 🧪 Testbench  
The testbench applies input combinations (`A`, `B`, and `C`) to verify functional correctness.

![Testbench](./3_Input_AND_tb.png)

---

## 📈 Transient Simulation  
Transient simulation verifies the logical behavior under dynamic input changes. Output goes HIGH only when all inputs are HIGH.

![Transient Waveform](./3_input_AND_Transient_Waveform.png)

---

## 🧱 Layout  
The full-custom layout was created following 90nm design rules to ensure proper transistor placement and routing.

![Layout](./XOR_Layout.png)

---

## ✅ DRC and LVS Checks  

### ✔️ DRC: Design Rule Check  
No design rule violations were detected during DRC using **Assura**.

![DRC](./No_DRC_Errors.png)

### ✔️ LVS: Layout vs Schematic  
The layout matches the schematic netlist without any mismatches.

![LVS](./LVS_Run.png)

---

## 🔍 Schematic vs Layout Matching  
A visual check confirming that the layout matches the schematic both topologically and functionally.

![Match](./Layout_and_schematic_match.png)

---

## 🛠️ Tools Used  
- **Cadence Virtuoso** – Schematic, Symbol, Layout Design  
- **Spectre** – Transient Simulation  
- **Assura** – DRC and LVS Verification  
- **ADE L** – Waveform Analysis

---

## 👤 Author  
**Ram Tripathi**
