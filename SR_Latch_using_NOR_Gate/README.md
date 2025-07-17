
# CMOS SR Latch Using NOR Gates in Cadence Virtuoso

This repository presents the design and simulation of a **Set-Reset (SR) Latch** using **NOR gates** in **Cadence Virtuoso**, based on the **GPDK 90nm** CMOS technology. The project includes schematic creation, symbol view, testbench simulation, layout drawing, verification (DRC & LVS), parasitic extraction, and energy estimation.

---

## Table of Contents  
- [Schematic](#schematic)  
- [Symbol View](#symbol-view)  
- [Testbench](#testbench)  
- [Transient Simulation](#transient-simulation)  
- [Layout](#layout)  
- [DRC and LVS Checks](#drc-and-lvs-checks)  
- [Schematic vs Layout Matching](#schematic-vs-layout-matching)  
- [Parasitic Extraction (RCX)](#parasitic-extraction-rcx)  
- [AV Extracted View](#av-extracted-view)  
- [Energy Analysis](#energy-analysis)  
- [Tools Used](#tools-used)  
- [Author](#author)

---

## Schematic  
The schematic of the SR Latch is constructed using two cross-coupled NOR gates.

![Schematic](./SR_Latch_using_NOR_Schematic.png)

---

## Symbol View  
A custom symbol view for the SR Latch enables easy hierarchical design integration.

![Symbol](./SR_Latch_using_NOR_Gates.png)

---

## Testbench  
The testbench applies various combinations of Set (S) and Reset (R) inputs to verify latch behavior.

![Testbench](./SR_Latch_using_NOR_Tb.png)

---

## Transient Simulation  
The transient response confirms the expected SR latch behavior under different input conditions.

![Transient](./SR_Latch_using_NOR_Transient.png)

---

## Layout  
A compact layout of the SR Latch was created using standard layout techniques for 90nm CMOS.

![Layout](./LAYOUT_SR_Latch_using_NOR.png)

---

## DRC and LVS Checks

### DRC: Design Rule Check  
The layout passed all design rule checks (DRC) successfully.

![DRC Clearance](./NO_DRC_SR_LATCH_usimg_NOR.png)

### LVS: Layout vs Schematic  
LVS confirms the layout is electrically equivalent to the schematic.

![LVS Run](./LVS_RUN_SR_Latch_using_NOR.png)

---

## Schematic vs Layout Matching  
Visual confirmation of schematic and layout netlist alignment.

![Match View](./Layout_and_schematic_match_SR_Latch_using_NOR_Gate.png)

---

## Parasitic Extraction (RCX)  
Assura RCX was used to extract parasitic elements for accurate post-layout simulation.

![RCX Run](./RCX_Run_SR_Latch_using_NOR.png)

---

## AV Extracted View  
The AV view includes parasitics, allowing accurate back-annotated simulation.

![AV Extracted View](./AV_Extracted_view_SL_Latch_using_NOR.png)

---

## Energy Analysis  
Post-layout simulation estimates the energy consumption per transition cycle in the **femtojoule (fJ)** range, reflecting a power-efficient latch design.

![Energy Draw](./Energy_estimation_SR_Latch_using_NOR.png)

---

## Tools Used  
- **Cadence Virtuoso** – Schematic and Layout Design  
- **Assura** – DRC, LVS, and RCX Parasitic Extraction  
- **Spectre / ADE L/XL** – Transient Simulation and Energy Analysis  

---

## Author  
**Ram Tripathi**
