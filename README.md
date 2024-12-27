# Digital IC Design of 4-bit ALU Using Cadence

This project involves designing and simulating a **4-bit Arithmetic Logic Unit (ALU)** using **Cadence Virtuoso**. The ALU is a fundamental component in digital systems, capable of performing arithmetic and logical operations. The design includes modular circuit components, such as multiplexers, gates, and combinational logic, integrated to perform 4-bit arithmetic and logical operations.

---

## Project Structure

The project folder contains the following directories and files:

```plaintext
.
├── .oalib           # Cadence design library information
├── 16to4MUX         # Design and schematic for 16-to-4 multiplexer
├── 2to1MUX          # Design and schematic for 2-to-1 multiplexer
├── 4to1AND          # Design and schematic for 4-input AND gate
├── 8to4MUX          # Design and schematic for 8-to-4 multiplexer
├── AND              # AND gate circuit design and verification
├── cdsinfo.tag      # Cadence metadata for library
├── data.dm          # Design and simulation data
├── NAND             # NAND gate circuit design and verification
├── NOR              # NOR gate circuit design and verification
├── NOT              # NOT gate circuit design and verification
├── OR               # OR gate circuit design and verification
└── XOR              # XOR gate circuit design and verification
```

---

## Features of the Design

1. **Arithmetic and Logical Operations**:
   - **Arithmetic**: Addition, Subtraction.
   - **Logical**: AND, OR, XOR, NAND, NOR.
   - Support for 4-bit wide operations.

2. **Modular Design**:
   - Implemented using hierarchical design methodology.
   - Reusable components like multiplexers and gates.

3. **Scalable and Optimized**:
   - Efficient logic implementation for speed and minimal power consumption.

4. **Verification and Simulation**:
   - Thorough testing using Cadence ADE-L for functional correctness.
   - Layout verification for DRC and LVS compliance.

---

## How to Use the Project

### 1. Prerequisites
- **Cadence Virtuoso**: Installed and configured for digital IC design.
- **Cadence ADE-L/ADE-XL**: For simulation and verification.
- **Technology Library**: Set up according to your design node.

### 2. Setting Up the Environment
1. Load the project in **Cadence Virtuoso**:
   - Open Virtuoso and load the provided library (`.oalib`).
   - Ensure the `cdsinfo.tag` is correctly referenced in your Cadence environment.

2. Import the components:
   - Each folder (`AND`, `OR`, etc.) contains circuit schematics.
   - Open these designs to view, modify, or simulate individual components.

3. Compile and link the library:
   - Use the **Library Manager** in Cadence to view the hierarchical design.
   - Ensure all cells (MUXes, gates) are compiled correctly.

### 3. Simulating the Design
1. Use **ADE-L** to configure the simulation:
   - Load the **4-bit ALU top-level design**.
   - Apply input vectors to test various operations.

2. Verify functionality:
   - Check waveform results to validate logical correctness.
   - Test for all possible 4-bit input combinations.

3. Perform DRC and LVS:
   - Run **DRC** (Design Rule Check) to ensure layout compliance.
   - Perform **LVS** (Layout vs Schematic) to verify the design matches the schematic.

### 4. Design Hierarchy
- **Logic Gates**:
  - Basic gates such as AND, OR, NOT, NAND, XOR, and NOR.
- **Multiplexers**:
  - Multi-bit MUX designs (`16to4MUX`, `8to4MUX`, etc.) for selecting operations.
- **Top-Level ALU**:
  - Combines logic gates and multiplexers to form the 4-bit ALU.

---

## Design Components

| **Component**  | **Description**                               |
|-----------------|-----------------------------------------------|
| `AND`          | 2-input AND gate.                            |
| `OR`           | 2-input OR gate.                             |
| `NOT`          | Single-input NOT gate.                       |
| `XOR`          | 2-input XOR gate.                            |
| `NAND`         | 2-input NAND gate.                           |
| `NOR`          | 2-input NOR gate.                            |
| `2to1MUX`      | Multiplexer with 2 inputs and 1 output.       |
| `4to1AND`      | Combines 4-input AND functionality.           |
| `8to4MUX`      | Multiplexer with 8 inputs and 4 outputs.      |
| `16to4MUX`     | Multiplexer with 16 inputs and 4 outputs.     |
---

**Author**: Eyad Gad  
**Contact**: [egad@uwo.ca](mailto:egad@uwo.ca)
