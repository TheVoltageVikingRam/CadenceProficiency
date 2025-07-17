# SR Latch using NAND Gates (CMOS Design in Cadence Virtuoso)

This project showcases the design and implementation of an **SR (Set-Reset) Latch** using two cross-coupled **NAND gates**, created using Cadence Virtuoso. It includes all necessary stages: schematic design, symbol generation, testbench simulation, layout creation, verification (DRC/LVS), RC parasitic extraction, and energy analysis.

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `SR_NAND_Schematic.png` | Circuit schematic of SR latch using NAND gates |
| `SR_using_NAND_symbol.png` | Symbol view used for hierarchical simulation |
| `SR_Using_NAND_Tb.png` | Testbench used to verify functional behavior |
| `SR_Latch_using_NAND_Transient.png` | Output waveform showing latch behavior |
| `Layout_and_schematic_match_SR_Latch_NAND.png` | Match verification between schematic and layout |
| `No_DRC_Errros.png` | Confirmation of no DRC violations |
| `LVS_Run_SR_Latch_Using_NAND.png` | Successful LVS run |
| `AV_extracted_view_SR_Latch_NAND.png` | Extracted layout view (with parasitics) |
| `RCX_run_SR_Latch_Using_NAND.png` | RCX extraction run result |
| `SR_Latch_Energy_Estimation.png` | Estimated energy for one cycle |
| `README.md` | Project documentation |

---

## 🔧 Schematic

The latch is implemented using two 2-input NAND gates connected in a cross-coupled manner. Inputs are **S (Set)** and **R (Reset)**.

![Schematic](./SR_NAND_Schematic.png)

---

## 🧩 Symbol View

A clean symbol was generated to allow hierarchical design usage.

![Symbol](./SR_using_NAND_symbol.png)

---

## ⚙️ Testbench

A testbench was created to verify the latch behavior across various S and R input combinations.

![Testbench](./SR_Using_NAND_Tb.png)

---

## 📈 Transient Response

The transient simulation confirms correct operation:
- Q is set when S = 0, R = 1
- Q is reset when S = 1, R = 0
- Invalid state at S = 0, R = 0

![Transient](./SR_Latch_using_NAND_Transient.png)

---

## 🧱 Layout

The layout of the SR latch was drawn following GPDK 90nm design rules.

![Layout Match](./Layout_and_schematic_match_SR_Latch_NAND.png)

---

## ✅ DRC and LVS

- **DRC**: No design rule violations.
  ![No DRC Errors](./No_DRC_Errros.png)

- **LVS**: Layout matches the schematic.
  ![LVS Run](./LVS_Run_SR_Latch_Using_NAND.png)

---

## 📦 RCX Extraction

RC parasitics were extracted for accurate post-layout simulation and power estimation.

![RCX](./RCX_run_SR_Latch_Using_NAND.png)

![AV Extracted View](./AV_extracted_view_SR_Latch_NAND.png)

---

## ⚡ Energy Estimation

The energy consumed in one transition cycle was calculated based on the extracted netlist simulation.

![Energy](./SR_Latch_Energy_Estimation.png)

---

## 🛠️ Tools Used

- **Cadence Virtuoso** – Schematic & Layout Design  
- **Assura / Calibre** – DRC, LVS, and Parasitic Extraction  
- **Spectre ADE L/XL** – Simulation and Energy Estimation  
- **Technology** – GPDK 90nm

---

## 👤 Author

**Ram Tripathi**  
*BSc (H) Electronics, Deen Dayal Upadhyaya College (University of Delhi)*  

