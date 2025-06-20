# CMOS Buffer Design in Cadence Virtuoso

This project demonstrates the complete **CMOS buffer** design using **Cadence Virtuoso**, including schematic, symbol, testbench circuit, layout, simulation waveforms, DRC/LVS checks, and post-layout extracted view.

## Table of Contents  
- [Schematic](#schematic)  
- [Symbol View](#symbol-view)  
- [Testbench](#testbench)  
- [Transient and DC Response](#transient-and-dc-response)  
- [Layout](#layout)  
- [LVS and DRC Verification](#lvs-and-drc-verification)  
- [Post-Layout (RCX) View](#post-layout-rcx-view)  
- [Tools Used](#tools-used)  
- [Author](#author)

---

## Schematic  
The CMOS buffer was designed using the **schematic editor** in Cadence Virtuoso.

![Schematic](./Buffer_Schematic.png)

---

## Symbol View  
A custom symbol was created for hierarchical design and testbench connection.

![Symbol View](./Symbol.png)

---

## Testbench  
The testbench was developed to analyze both **static and dynamic** behavior of the buffer.

![Testbench](./buffer_tb.png)

---

## Transient and DC Response  

- **Transient Response:** Shows the time-domain signal propagation through the buffer.  
- **DC Response:** Indicates the voltage transfer characteristic (VTC).

![Transient Response](./Buffer_Transient.png)  
![DC Response](./Buffer_DC_response.png)

---

## Layout  
The layout of the buffer was created following standard design rules.

![Layout](./Layout.png)

---

## LVS and DRC Verification  

- ✅ **DRC Passed**: No design rule violations were found.  
- ✅ **LVS Passed**: The layout matches the schematic with no mismatches.

![No DRC](./No_DRC.png)  
![LVS Report](./LVS%20with%20No%20mismatch.png)

---

## Post-Layout (RCX) View  
The extracted view includes parasitic capacitance and resistance using **RCX (Parasitic Extraction)**.

![Extracted View](./AV_Extracted_View.png)  
![RCX Run](./RCX_Run.png)

---

## Tools Used  
- **Cadence Virtuoso** – For schematic and layout design  
- **Spectre** – For transient and DC simulations  
- **Assura/Calibre** – For DRC & LVS verification  
- **RCX** – For post-layout parasitic extraction  

---

## Author  
**Ram Tripathi**
