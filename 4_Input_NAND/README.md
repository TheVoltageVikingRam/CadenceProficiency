# NAND4 Gate Design in Cadence Virtuoso

This repository demonstrates the **full-custom VLSI design** of a **4-input NAND (NAND4) Gate** using **Cadence Virtuoso**. It includes the **schematic, symbol, layout, extracted view, testbench, LVS, and verification results**.

---
## Table of Contents
- [Schematic](#schematic)
- [Symbol](#symbol)
- [Testbench](#testbench)
- [Prelayout Transient](#prelayout-transient)
- [Layout](#layout)
- [DRC Clean Layout](#drc-clean-layout)
- [Extracted View](#extracted-view)
- [LVS Results](#lvs-results)
- [Design Methodology](#design-methodology)
- [Tools Used](#tools-used)
- [Author](#author)

---
## Schematic
The NAND4 schematic designed using **Cadence Virtuoso**.

![Schematic](NAND4_SCHEMATIC.png)

---
## Symbol
Custom symbol created for use in the testbench.

![Symbol](nand4_symbol.png)

---
## Testbench
Testbench used to verify logic and transient behavior.

![Testbench](NAND4_TB.png)

---
## Prelayout Transient
Prelayout transient simulation using Spectre.

![SRAM Simulation](SRAM_Cadence_Simulation_Prelayout.png)

---
## Layout
Initial layout of the NAND4 gate.

![Layout](Layout_NAND4.png)

---
## DRC Clean Layout
Layout after fixing all **Design Rule Check (DRC)** violations.

![DRC Clean Layout](NAND_4_Layout_No_DRC.png)

---
## Extracted View
Extracted layout used for post-layout simulation.

![Extracted View](av_extracted_view_nand4.png)

---
## LVS Results
Layout vs Schematic (LVS) verification.

### LVS Comparison Window
![LVS Comparison](layout_vs_schematic_comparison.png)

### LVS Match – No Mismatch
![LVS Match](nand4_no_Lvs_mismatch.png)

### Layout and Schematic Comparison at Switching
![Minimal Differences](nand4_schematic_vs_layout_very_minimal_difference.png)

---

## Design Methodology

This NAND4 gate follows proper **full-custom VLSI design principles**, with attention to key device-level and layout-level considerations:

<details>
<summary><strong>Transistor Sizing Strategy</strong></summary>

### NMOS Network (Series Stack)
- For a 4-input NAND, **NMOS devices are in series**, increasing effective resistance.
- Each NMOS is sized **larger than minimum width** to avoid excessive resistance and maintain fast pull-down.
- Series stack resistance = n × R_single, requiring compensation through upsizing.

### PMOS Network (Parallel)
- PMOS devices are in **parallel**, providing multiple low-resistance paths to VDD.
- PMOS widths are increased to balance rise/fall times, compensating for:
  - High resistance of the series NMOS stack
  - Lower hole mobility (~2.5× slower than electrons)
- Typical sizing: W_pmos ≈ 2-2.5 × W_nmos for symmetric propagation delays
- **Balanced propagation delay** (tpLH ≈ tpHL)
- Clean logic switching with minimal overshoot/undershoot
- Strong **noise margins** (NM_H, NM_L > 30% VDD)
- Optimized input capacitance for minimal loading on previous stages

</details>

<details>
<summary><strong>Layout Quality & Optimization</strong></summary>

### Area Efficiency
- **Shared diffusions** between adjacent transistors reduce total area
- Devices arranged in linear topology to minimize routing complexity
- Compact layout reduces die cost and improves yield

### Parasitic Minimization
- Short diffusion regions minimize junction capacitance (C_j)
- Minimal metal routing lengths reduce interconnect RC delay
- Strategic via/contact placement lowers series resistance
- Post-layout extraction shows minimal delay degradation compared to schematic

### Design Rule Compliance
- All metal width, spacing, and enclosure rules strictly followed
- Proper **well spacing** and **well-tap placement** prevent latchup
- Contact density meets foundry requirements for reliability
- Symmetric device placement ensures **predictable performance across process corners**

</details>

<details>
<summary><strong>Electrical Robustness</strong></summary>

### Signal Integrity
- Input devices placed close to routing channels to minimize gate resistance
- Adequate decoupling through proper VDD/VSS rail sizing

### Performance Consistency
- Matched device orientation reduces mismatch effects
- Uniform device spacing maintains thermal symmetry
- Conservative design margins ensure functionality across PVT corners (Process, Voltage, Temperature)

</details>

<details>
<summary><strong>Verification Strength</strong></summary>

### Pre-Silicon Validation
- **Prelayout simulation:** Functional correctness with ideal devices
- **Post-layout (extracted) simulation:** Includes all parasitics (R, C, CC)
- Both simulations match closely, validating layout quality

### Physical Verification
- **DRC-clean:** Zero design rule violations, ensuring manufacturability
- **LVS-matched:** Topological equivalence between schematic and layout confirmed
- All nets, devices, and parameters verified for correctness

</details>

---

These design choices collectively create a **robust, optimized, and electrically reliable NAND4 gate** suitable for custom logic or digital cell libraries.

---

## Tools Used
- **Cadence Virtuoso** – Schematic & Layout Editor
- **Assura** – DRC & LVS Verification
- **Spectre** – Simulation & Analysis
- **GPDK 90nm** – Process Design Kit

---
## Author
**Ram Tripathi (22HEL2231)**  
BSc (Hons.) Electronics – Final Year Project
