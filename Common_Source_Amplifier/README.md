
# CMOS Common Source Amplifier Design (GPDK 90nm)

This repository documents the design and analysis of a **Common Source Amplifier** implemented using **Cadence Virtuoso** with **GPDK 90nm** technology. It includes schematic capture, layout design, simulation, DRC/LVS/RCX verification, and energy and power analysis.

---

## 📁 Contents

- [Schematic](#schematic)
- [Transient and DC Analysis](#transient-and-dc-analysis)
- [Layout](#layout)
- [DRC & LVS Verification](#drc--lvs-verification)
- [Layout vs Schematic Matching](#layout-vs-schematic-matching)
- [RC Extraction](#rc-extraction)
- [AV Extracted View](#av-extracted-view)
- [Energy and Power Analysis](#energy-and-power-analysis)
- [Tools Used](#tools-used)
- [Author](#author)

---

## 📐 Schematic

The amplifier is implemented using a single NMOS transistor with a resistive load and biasing configured for mid-band gain.

![Schematic](./Common_source_amplifier_schematic.png)

---

## 📊 Transient and DC Analysis

### Transient Response

Simulation confirms gain and signal amplification behavior.

![Transient Response](./Transient_Response_CS_amp.png)

### DC Transfer Characteristics

DC sweep of input vs output highlights gain and operating point.

![DC Response](./dc_response.png)

---

## 🧱 Layout

Full layout created and verified using DRC and LVS tools.

![Layout](./Lyout_CS_Amp.png)

---

## ✅ DRC & LVS Verification

### DRC (Design Rule Check)  
All physical design rules are satisfied.

![No DRC](./No_DRC_CS_amp.png)

### LVS (Layout vs Schematic)

Confirms layout matches schematic netlist.

![LVS](./LVS_Run_CS_Amp.png)

---

## 🧮 Layout vs Schematic Matching

Visual confirmation of layout and schematic net connectivity.

![Layout and Schematic Match](./Layout_and_schematic_match_CS_amp.png)

---

## 📉 RC Extraction

Parasitic elements are extracted to refine post-layout simulation.

![RCX](./RCX_Run_CS_Amp.png)

---

## 🧪 AV Extracted View

The extracted netlist includes parasitics for accurate signal and power estimation.

![AV Extracted View](./AV_Extracted_view_CS_Amp.png)

---

## ⚡ Energy and Power Analysis

### Energy Consumption Estimation

Estimated dynamic energy per input cycle.

![Energy Estimation](./Energy_Estimation_CS_Amp.png)

### Power Curve

Displays power variation over time or input.

![Power Curve](./Power_Curve.png)

---

## 🛠 Tools Used

- **Cadence Virtuoso** (Schematic/Layout/Simulation)
- **GPDK 90nm PDK**
- **Spectre** (Transient and DC Analysis)
- **Assura** (DRC, LVS, RCX)

---

## 👤 Author

**Ram Tripathi**
