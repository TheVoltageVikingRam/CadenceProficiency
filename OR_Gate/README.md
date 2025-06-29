
# CMOS OR Gate Design in Cadence Virtuoso

This repository contains the full-custom design and simulation of a **CMOS OR Gate** implemented using **Cadence Virtuoso**. It covers schematic design, layout, DRC/LVS verification, post-layout RC extraction, transient analysis, and energy estimation for a single cycle.

---

## 📁 Table of Contents  
- [🧩 Schematic](#-schematic)  
- [🧪 Testbench](#-testbench)  
- [📈 Transient Simulation](#-transient-simulation)  
- [🧱 Layout](#-layout)  
- [✅ DRC and LVS Checks](#-drc-and-lvs-checks)  
- [🔍 LVS Match View](#-lvs-match-view)  
- [🧠 Parasitic Extraction (RCX)](#-parasitic-extraction-rcx)  
- [🧾 AV Extracted View](#-av-extracted-view)  
- [⚡ Energy Estimation](#-energy-estimation)  
- [🛠️ Tools Used](#-tools-used)  
- [👤 Author](#-author)

---

## 🧩 Schematic  
The OR gate is designed using complementary CMOS logic. It outputs HIGH if either input is HIGH.

![Schematic](./Schematic_OR.png)

---

## 🧪 Testbench  
The testbench applies all input combinations (`A`, `B`) to validate the gate’s logical behavior.

![Testbench](./OR_Gate_testbench.png)

---

## 📈 Transient Simulation  
Transient waveform confirms that the OR gate functions correctly under all possible input transitions.

![Transient](./OR_Gate_transient_waveform.png)

---

## 🧱 Layout  
The layout was created in Cadence Virtuoso following 90nm design rules and optimized transistor placement.

![Layout](./OR_Layout.png)

---

## ✅ DRC and LVS Checks  

### ✔️ DRC (Design Rule Check)  
No design rule violations were found. Verified using **Assura DRC**.

![DRC](./DRC_Clearance.png)

### ✔️ LVS (Layout vs Schematic)  
The layout netlist matches the schematic functionally and topologically.

![LVS Run](./LVS_run.png)

---

## 🔍 LVS Match View  
Graphical view confirming the net-to-net match between the schematic and layout.

![LVS Match](./LVS_Match.png)

---

## 🧠 Parasitic Extraction (RCX)  
RC parasitic extraction was performed to include interconnect resistance and capacitance in simulations.

![RCX](./RCX_Run.png)

---

## 🧾 AV Extracted View  
The Annotated View highlights parasitic R and C components mapped on the layout nets.

![AV Extracted View](./AV_Extracted_view.png)

---

## ⚡ Energy Estimation  
Estimated energy consumption for a complete OR gate switching cycle using post-layout simulation.

![Energy](./Energy_one_cycle_OR.png)

---

## 🛠️ Tools Used  
- **Cadence Virtuoso** – Schematic, Layout  
- **Spectre** – Transient Simulation  
- **Assura** – DRC, LVS, RCX  
- **ADE L** – Testbench Simulation & Power Estimation

---

## 👤 Author  
**Ram Tripathi**
