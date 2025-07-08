# CMOS 4×1 MUX Implementation Using 2×1 MUX Modules in Cadence Virtuoso

This repository documents the hierarchical design, layout, and verification of a **4×1 Multiplexer** built using multiple **2×1 MUX** units. The implementation is performed in **Cadence Virtuoso**, covering schematic design, symbol creation, testbench simulation, layout drawing, verification (DRC/LVS), RC parasitic extraction, and energy analysis.

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
The 4×1 multiplexer is implemented using **three 2×1 multiplexers** in a tree structure. This modular approach is beneficial for hierarchical and reusable digital design.

![Schematic](./4X1MUX_Using_2X1MUX_Schematic.png)

---

## Symbol View  
A symbol was generated for the 4×1 MUX to allow hierarchical connectivity in the testbench and layout.

![Symbol](./SYMBOL_4X1_MUX_USING_2X1_MUX.png)

---

## Testbench  
The testbench applies all combinations of select lines and inputs to verify the MUX functionality.

![Testbench](./TB_4X1_MUX_USING_2X1_MUX.png)

---

## Transient Simulation  
The waveform shows that the output of the 4×1 MUX correctly follows the selected input based on select signals, validating functionality.

![Transient](./trasnsient_waveform_4X1MUXusing2X1MUX.png)

---

## Layout  
The full layout was created in Cadence Virtuoso, adhering to 90nm design rules and optimized for area and performance.

![Layout](./Layout_4X1_MUX_using_2X1_MUX.png)

---

## DRC and LVS Checks

### DRC: Design Rule Check  
The design passed all DRC rules successfully, ensuring fabrication readiness.

![DRC Clearance](./No_DRC_Erros_MUX4X1with2X1.png)

### LVS: Layout vs Schematic  
LVS verification confirms that the physical layout accurately reflects the schematic netlist.

![LVS Run](./LVS_Run_4X1MUX_using_2X1MUX.png)  
![LVS Info](./No_extraction_erros_4X1MUX_using_2X1_MUX.png)

---

## Schematic vs Layout Matching  
A graphical match confirms structural alignment between schematic and layout levels.

![Match View](./Layout_and_schematic_match.png)

---

## Parasitic Extraction (RCX)  
RC extraction using Assura provides parasitic resistance and capacitance for accurate post-layout simulation.

![RCX Run](./RCX_Run_4X1_MUX_using_2X1_MUX.png)

---

## AV Extracted View  
The AV view shows extracted netlists including parasitic values for back-annotation and simulation refinement.

![AV Extracted View](./AV_Extracted_view_4X1MUX_using_2X1_MUX.png)

---

### Energy Analysis  
The post-layout simulation shows that the 4×1 MUX consumes approximately **75.65 femtojoules (fJ)** per switching cycle.  
This value is well within expected bounds for a design implemented in **GPDK 90nm** technology. It reflects an efficient design with minimal parasitic effects and optimized switching activity. Such low energy consumption makes this implementation suitable for low-power digital systems and educational benchmarking.


![Energy Draw](./Energy_draw_for_one_cycle.png)

---

## Tools Used  
- **Cadence Virtuoso** – Schematic and Layout Design  
- **Assura** – DRC, LVS, and RCX Parasitic Extraction  
- **Spectre / ADE L/XL** – Transient Simulation and Energy Analysis  

---

## Author  
**Ram Tripathi**

