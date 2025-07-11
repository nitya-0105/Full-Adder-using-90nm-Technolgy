# Full-Adder-using-90nm-Technolgy


This project presents the complete CMOS implementation of a **1-bit Full Adder** using standard digital design techniques. It includes circuit equations, SPICE simulations, schematic, DRC/LVS verification, and layout using industry-grade tools.

---

## 🧠 Objective

To design, simulate, and verify a **1-bit Full Adder** at the transistor level using CMOS technology and to understand key aspects of schematic capture, layout design, parasitic extraction, and physical verification.

---

## 🔗 Boolean Equations

A Full Adder has 3 inputs: `A`, `B`, and `Cin`, and 2 outputs: `Sum` and `Cout`.

**Logic Expressions:**

---

## 📊 Truth Table

| A | B | Cin | Sum | Cout |
|---|---|-----|-----|------|
| 0 | 0 |  0  |  0  |  0   |
| 0 | 0 |  1  |  1  |  0   |
| 0 | 1 |  0  |  1  |  0   |
| 0 | 1 |  1  |  0  |  1   |
| 1 | 0 |  0  |  1  |  0   |
| 1 | 0 |  1  |  0  |  1   |
| 1 | 1 |  0  |  0  |  1   |
| 1 | 1 |  1  |  1  |  1   |

---



## 🧪 Transient Analysis

![Waveform](./fulladder_waveform.JPG)

- Shows time-domain response of `Sum` and `Cout` for all input combinations.
- Propagation delay and output validity confirmed.
- Glitches checked and minimized.

---

## 🧭 Schematic Design

![Schematic](./fulladder_schematic.JPG)

- XOR, AND, and OR gates implemented using CMOS logic.
- Inputs: A, B, Cin
- Outputs: Sum, Cout
- Design captured in Cadence Virtuoso with proper pin labels.

---

## ✅ DRC Report

- DRC (Design Rule Check) completed with **zero violations** under 90nm rules.
- Layout designed considering minimum width, spacing, and enclosure rules.

---

## 🧾 LVS Verification

![LVS](./fulladder_lvs.JPG)

- Layout vs Schematic (LVS) completed.
- Netlist matched with schematic.
- All device instances and pins verified.

---

## 🧱 Layout View

![Layout](./fulladder_layout.JPG)

- Compact layout of Full Adder optimized for area and routing.
- Metal layers, poly, diffusion, and contacts clearly defined.
- GDSII file ready for tape-out.

---

## 🧩 Tips & Techniques

1. **Use hierarchy** in design (half adder blocks).
2. Minimize series transistors in critical paths for better speed.
3. Use **minimum-sized inverters** for buffering non-critical nodes.
4. Keep **symmetric layout** for matched delay paths.
5. Carefully handle **parasitic loading** by checking RC extraction.
6. Always check **input pin drive strength** during simulation.

---

## 📚 References

- CMOS VLSI Design by Weste & Harris
- Digital IC Design Notes – SGSITS VLSI Internship
- IEEE Papers on Low Power Full Adders

---



## 🚀 Future Scope

- 4-bit Ripple Carry Adder design  
- Low-power full adder using transmission gates  
- Dynamic CMOS version for high-speed applications  
- Integration into ALU design


