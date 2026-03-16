# DLD Labs — Digital Logic Design Projects

A collection of Digital Logic Design (DLD) lab projects implemented and simulated using **Proteus Design Suite**. These labs cover fundamental combinational-circuit concepts including logic gates, multiplexers, and data selectors from the 74LS TTL IC family.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Lab Projects](#lab-projects)
  - [NAND Gate](#nand-gate)
  - [Lab 1 — 2-to-1 Multiplexer (74LS257)](#lab-1--2-to-1-multiplexer-74ls257)
  - [Lab 4 — 2-to-1 Multiplexer (74LS257)](#lab-4--2-to-1-multiplexer-74ls257)
  - [Lab 5 — 8-to-1 Multiplexer (74LS151)](#lab-5--8-to-1-multiplexer-74ls151)
- [Tools & Requirements](#tools--requirements)
- [How to Open a Project](#how-to-open-a-project)
- [Project Structure](#project-structure)
- [Contributors](#contributors)

---

## Overview

This repository contains Proteus simulation projects for a university-level Digital Logic Design course. Each lab focuses on a core topic in combinational circuit design, progressing from basic logic gates to multi-input data selectors. All circuits are designed, simulated, and verified in Proteus before physical implementation.

---

## Lab Projects

### NAND Gate

**File:** `NAND Gate.pdsprj`

Implements a 2-input NAND gate circuit using discrete TTL components. The lab explores the universal property of the NAND gate — that any Boolean function can be realized using only NAND gates — and documents the complete truth table verifying all input/output combinations.

| A | B | Output (A NAND B) |
|---|---|:-----------------:|
| 0 | 0 | 1                 |
| 0 | 1 | 1                 |
| 1 | 0 | 1                 |
| 1 | 1 | 0                 |

---

### Lab 1 — 2-to-1 Multiplexer (74LS257)

**File:** `Lab 1.pdsprj`

Implements a quadruple 2-line to 1-line data selector/multiplexer using the **74LS257** IC. The 74LS257 provides four independent 2-to-1 multiplexer channels with tri-state outputs, controlled by a common Select line and Output-Enable line.

**Key concepts covered:**
- Multiplexing / data selection
- Tri-state logic and bus driving
- Boolean expression for a 2-to-1 MUX: `Y = (A · S̄) + (B · S)`

---

### Lab 4 — 2-to-1 Multiplexer (74LS257)

**Files:**
- `Lab 4(2024-csre-008).pdsprj`
- `Lab 4(2024-csre-009).pdsprj`
- `LAB 4(2024_csre_009).pdsprj`
- `Lab 4(2024-csre-009.).pdsprj`

An extended study of the **74LS257** quadruple 2-to-1 multiplexer, with individual student simulation files for roll numbers `2024-csre-008` and `2024-csre-009`. The lab reinforces data-selection concepts and tri-state output behaviour explored in Lab 1.

**Key concepts covered:**
- Multi-channel multiplexing
- Output-enable (OE) control for bus sharing
- Comparison of outputs across multiple input combinations

---

### Lab 5 — 8-to-1 Multiplexer (74LS151)

**Files:**
- `Lab 5(2024_csre_008).pdsprj`
- `Lab 5(2024_csre_009).pdsprj`
- `Lab 5(2024_csre_009) - Copy.pdsprj`
- `Lab 5(2024_csre_009) - Copy (2).pdsprj`
- `Lab 5(2024_csre_009) - Copy (3).pdsprj`
- `Lab 5(2024_csre_009) - Copy (4).pdsprj`

Implements an 8-line to 1-line data selector/multiplexer using the **74LS151** IC. Three binary select inputs (A, B, C) choose one of eight data inputs to route to the output, making this an ideal building block for function generators and data routing networks.

**Key concepts covered:**
- 3-variable address decoding
- Implementing arbitrary Boolean functions using an 8-to-1 MUX
- Complementary outputs (`Y` and `Ȳ`)

**74LS151 Pin Summary:**

| Pin Group | Description                          |
|-----------|--------------------------------------|
| D0 – D7   | Eight data inputs                    |
| A, B, C   | Select inputs (address lines)        |
| Y         | Non-inverted output                  |
| Ȳ (W)    | Inverted output                      |
| /E        | Active-low enable input              |

---

## Tools & Requirements

| Tool | Version | Purpose |
|------|---------|---------|
| [Proteus Design Suite](https://www.labcenter.com/) | 8.x or later | Circuit schematic design and simulation |

> **Note:** `.pdsprj` files are Proteus project archives. They cannot be opened with general text editors or other EDA tools without conversion.

---

## How to Open a Project

1. Install **Proteus Design Suite** (version 8.x or later recommended).
2. Clone or download this repository:
   ```bash
   git clone https://github.com/muhammad-asif10/DLD_Labs.git
   ```
3. Launch Proteus and choose **File → Open Project**.
4. Navigate to the cloned folder and select the desired `.pdsprj` file.
5. Run the simulation via **Debug → Start/Restart Debugging** (or press **F12**).

---

## Project Structure

```
DLD_Labs/
│
├── NAND Gate.pdsprj                      # Lab: 2-input NAND gate circuit
├── Lab 1.pdsprj                          # Lab 1: 74LS257 2-to-1 MUX
│
├── Lab 4(2024-csre-008).pdsprj           # Lab 4: 74LS257 MUX (student 008)
├── Lab 4(2024-csre-009).pdsprj           # Lab 4: 74LS257 MUX (student 009)
├── LAB 4(2024_csre_009).pdsprj           # Lab 4: 74LS257 MUX (alternate)
├── Lab 4(2024-csre-009.).pdsprj          # Lab 4: 74LS257 MUX (revision)
│
├── Lab 5(2024_csre_008).pdsprj           # Lab 5: 74LS151 8-to-1 MUX (student 008)
├── Lab 5(2024_csre_009).pdsprj           # Lab 5: 74LS151 8-to-1 MUX (student 009)
├── Lab 5(2024_csre_009) - Copy.pdsprj    # Lab 5: backup copy
├── Lab 5(2024_csre_009) - Copy (2).pdsprj
├── Lab 5(2024_csre_009) - Copy (3).pdsprj
└── Lab 5(2024_csre_009) - Copy (4).pdsprj
```

---

## Contributors

| Name | Roll Number | Labs |
|------|-------------|------|
| Muhammad Asif | 2024-CSRE-008 | Lab 1, Lab 4, Lab 5 |
| Aqsa Amjad | 2024-CSRE-009 | Lab 4, Lab 5, NAND Gate |

---

*Department of Computer Systems & Robotics Engineering*
