# Design of Low-Power Arithmetic and Logic Circuits Using Reversible Logic Gates

## Overview

This repository presents the design, implementation, and performance evaluation of **energy-efficient arithmetic and logic circuits** using **Reversible Logic Gates (RLGs)**. The project focuses on the development of a **Half Adder, Full Adder, 2-to-4 Decoder, and 2×1 Multiplexer**, targeting **low power consumption and reduced propagation delay** for VLSI applications.

Reversible logic is a promising paradigm for low-power and quantum-aware computing systems, as it minimizes information loss and associated heat dissipation. The designs in this project demonstrate significant improvements over conventional CMOS-based implementations.

---

## Key Objectives

* Design arithmetic and logic circuits using reversible logic gates
* Reduce power consumption and propagation delay
* Analyze performance using **Power, Delay, and Power Delay Product (PDP)**
* Compare proposed reversible designs with conventional logic circuits

---

## Circuits Implemented

* **Half Adder**
* **Full Adder**
* **2-to-4 Decoder**
* **2×1 Multiplexer**

Each circuit is designed using combinations of reversible gates such as:

* New Gate (NG)
* Toffoli Gate
* Peres Gate
* Feynman Gate
* URQG Gate
* TR Gate
* CNOT, NOT, and Double Feynman Gates

---

## Reversible Logic Gates Used

Reversible gates maintain a one-to-one mapping between inputs and outputs, ensuring no information loss.

| Gate          | Description                                               |
| ------------- | --------------------------------------------------------- |
| New Gate (NG) | Custom reversible gate optimized for arithmetic functions |
| Toffoli Gate  | Universal reversible gate (CCNOT)                         |
| Peres Gate    | Combines XOR and AND functionality                        |
| Feynman Gate  | Used for signal copying and XOR                           |
| URQG Gate     | Universal reversible quantum gate                         |
| TR Gate       | Controlled-controlled NOT variant                         |
| CNOT / NOT    | Basic reversible primitives                               |

---

## Design Methodology

1. Logical formulation using reversible Boolean expressions
2. Gate-level construction using RLGs
3. Schematic design and simulation
4. Measurement of:

   * Power consumption (µW)
   * Propagation delay (ps)
   * Power Delay Product (fJ)
5. Comparison with conventional logic implementations

---

## Performance Summary

### Half Adder

| Design         | Power (µW) | Delay (ps) | PDP (fJ)  |
| -------------- | ---------- | ---------- | --------- |
| Conventional   | 30.12      | 8.75       | 261.87    |
| Proposed (RLG) | **16.40**  | **5.04**   | **82.65** |

### Full Adder

| Design         | Power (µW) | Delay (ps) | PDP (fJ)   |
| -------------- | ---------- | ---------- | ---------- |
| Conventional   | 45.80      | 15.20      | 696.16     |
| Proposed (RLG) | **22.67**  | **10.48**  | **237.58** |

### 2-to-4 Decoder

| Design         | Power (µW) | Delay (ps) | PDP (fJ)  |
| -------------- | ---------- | ---------- | --------- |
| Conventional   | 10–50      | 1000–5000  | 50–200    |
| Proposed (RLG) | **1.0**    | **1000**   | **30.59** |

### 2×1 Multiplexer

| Design         | Power (µW) | Delay (ps) | PDP (fJ)  |
| -------------- | ---------- | ---------- | --------- |
| Conventional   | 20–50      | 200–1000   | 10–50     |
| Proposed (RLG) | **5.05**   | **435.7**  | **0.067** |

---

## Results & Insights

* ~50% reduction in power consumption
* ~45% reduction in propagation delay
* Significant improvement in Power Delay Product (PDP)
* Demonstrates suitability of reversible logic for **low-power VLSI and future quantum systems**

---

## Tools & Environment

* Digital circuit simulation tool ( CADENCE- Virtuso )
* Waveform analysis for functional verification
* Power and delay extracted from simulation results

---

## Repository Structure (Suggested)

```text
.
├── paper/
│   └── reversible_logic.pdf
├── schematics/
├── simulation_results/
├── waveforms/
└── README.md
```

---

## Applications

* Low-power VLSI design
* Energy-efficient arithmetic units
* Quantum and reversible computing research
* Embedded and portable electronic systems

---

## References

This work is based on and extends prior research in reversible logic and low-power circuit design. Full references are provided in the attached paper.

---

## Author

**[Sayyad Rahiman]**
VLSI / Digital Design Enthusiast
RTL Design | Low-Power Circuits | Reversible Computing

---

## License

This project is intended for **academic and research purposes**. Please cite the original paper when using or extending this work.
