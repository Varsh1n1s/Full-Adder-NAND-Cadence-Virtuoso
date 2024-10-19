# Full-Adder-NAND-Cadence-Virtuoso

---

# Full Adder Using NAND Gates in Cadence Virtuoso

This project implements a **Full Adder** using only **NAND gates**, designed and simulated in **Cadence Virtuoso**. A Full Adder is a fundamental digital circuit that performs binary addition on three inputs: two significant bits and one carry bit from the previous stage. This project explores how the universal NAND gate can be used to build a Full Adder circuit.

## Project Overview

- **Tool**: Cadence Virtuoso
- **Design Type**: CMOS Design using NAND gates
- **Simulation**: Spectre

### Features
- Design and schematic implementation of a Full Adder using only NAND gates.
- Functional verification of Sum and Carry outputs through circuit simulation.
- Layout design for efficient power and area usage.
- Power and performance optimization using Spectre simulations.

## Design Details

- **Inputs**: A, B, Cin (all 1-bit binary inputs)
- **Outputs**:
  - **Sum** = (A NAND B NAND Cin) combined with intermediate NAND logic.
  - **Carry** = Derived using multiple stages of NAND gates based on Full Adder logic.

The Full Adder is designed using a minimal number of NAND gates. The schematic and layout are optimized for area and power efficiency using standard CMOS design techniques.

### Logic Implementation

The Full Adder's Sum and Carry equations using only NAND gates are derived from the basic XOR and AND operations, which are expressed through combinations of NAND gates.

- **Sum** = ((A NAND A) NAND (B NAND B) NAND (Cin NAND Cin)) NAND ...
- **Carry** = (A NAND (B NAND Cin)) NAND ...

## Getting Started

### Prerequisites
- Cadence Virtuoso suite (Schematic Editor, Layout Editor, Spectre Simulator)

### Steps to Run the Project
1. Clone the repository:  
   `git clone https://github.com/Varsh1n1s/Full-Adder-NAND-Cadence-Virtuoso.git`
   
2. Open **Cadence Virtuoso** and load the schematic and layout files.

3. Inspect the **schematic**, which is constructed using only NAND gates for the Full Adder logic.

4. Run **Spectre simulations** to verify the functionality of the Sum and Carry outputs.

5. Proceed to **layout design** and perform DRC and LVS checks for validation.

6. Perform power, delay, and performance analysis.

## Results
- The **Sum** and **Carry** outputs are verified to work correctly.
- The layout is designed to be optimized for power and area, with proper design rules followed for CMOS logic.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
