# Input Inverter Design in Cadence Virtuoso

This repository demonstrates the **full-custom VLSI design** of an **Input Inverter** using **Cadence Virtuoso**. It includes the **schematic, symbol, layout, extracted view, testbench, LVS, and verification results**.

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
- [Waveform Comparison](#waveform-comparison)
- [Design Methodology](#design-methodology)
- [Tools Used](#tools-used)
- [Author](#author)

---
## Schematic
The input inverter schematic designed using **Cadence Virtuoso**.

![Schematic](input_inverter_schematic.png)

---
## Symbol
Custom symbol created for use in the testbench.

![Symbol](input_inverter_symbol.png)

---
## Testbench
Testbench used to verify logic and transient behavior.

![Testbench](input_inverter_testbench.png)

---
## Prelayout Transient
Prelayout transient simulation using Spectre.

![Prelayout Transient](input_inervter_transient_response.png)

---
## Layout
Initial layout of the input inverter.

![Layout](input_inverter_layout.png)

---
## DRC Clean Layout
Layout after fixing all **Design Rule Check (DRC)** violations.

![DRC Clean Layout](inp_inverter_layout_No_DRC.png)

---
## Extracted View
Extracted layout used for post-layout simulation.

![Extracted View](av_extracted_view_inp_inverter.png)

![Input Inverter Extracted View](input_inverter_av_extracted_view.png)

---
## LVS Results
Layout vs Schematic (LVS) verification.

### LVS Comparison Window
![LVS Comparison](layout_vs_schematic.png)

### LVS Match – No Mismatch
![LVS Match](No_LVS_Mismatch_inp_inverter.png)

---
## Waveform Comparison
Comparison of schematic and layout simulation waveforms.

### Schematic vs Layout Waveform
![Waveform Comparison](input_inverter_schematic_vs_layout_waveform_comparison.png)

### Delay Estimation
![Delay Estimation](inverter_schematic_vs_layout_waveform_comparison_delay_estimation.png)

---

## Design Methodology

This input inverter follows proper **full-custom VLSI design principles**, with attention to key device-level and layout-level considerations:

<details>
<summary><strong>Transistor Sizing Strategy</strong></summary>

### NMOS and PMOS Sizing
- PMOS width is typically **2-3× NMOS width** to compensate for lower hole mobility
- Balanced sizing ensures symmetric rise and fall times
- Proper sizing provides:
  - Equal propagation delays (tpLH ≈ tpHL)
  - Strong output drive capability
  - Good noise margins
  - Optimal switching threshold (VTH ≈ VDD/2)

</details>

<details>
<summary><strong>Layout Quality & Optimization</strong></summary>

### Area Efficiency
- **Shared diffusion** between NMOS and PMOS where applicable
- Compact layout minimizes parasitic capacitances
- Efficient device placement reduces overall cell area

### Parasitic Minimization
- Minimal interconnect lengths reduce RC delay
- Strategic contact and via placement
- Short diffusion regions minimize junction capacitance
- Post-layout extraction validates minimal delay degradation

### Design Rule Compliance
- All spacing, width, and enclosure rules strictly followed
- Proper **well contacts** and **substrate ties** prevent latchup
- Symmetric layout ensures predictable performance

</details>

<details>
<summary><strong>Electrical Robustness</strong></summary>

### Signal Integrity
- Clean input-to-output transition with minimal overshoot/undershoot
- Strong drive capability for capacitive loads
- Low input capacitance for minimal loading on previous stages

### Performance Consistency
- Matched device orientation for reduced mismatch
- Conservative design margins across PVT corners
- Robust operation under supply voltage variations

</details>

<details>
<summary><strong>Verification Strength</strong></summary>

### Pre-Silicon Validation
- **Prelayout simulation:** Functional verification with ideal components
- **Post-layout (extracted) simulation:** Includes all parasitics (R, C, CC)
- Waveform comparison shows close matching between schematic and layout

### Physical Verification
- **DRC-clean:** Zero design rule violations
- **LVS-matched:** Complete topological equivalence confirmed
- All nets and devices verified for correctness

</details>

---

These design choices collectively create a **robust, optimized, and electrically reliable inverter** suitable for input buffering, signal conditioning, or use in digital cell libraries.

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
