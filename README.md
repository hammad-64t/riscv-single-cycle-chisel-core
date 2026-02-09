# Single-Cycle RISC-V Core in Chisel
This project implements a **single-cycle RISC-V (RV32I) processor core** using **Chisel**, a modern hardware construction language embedded in Scala.  
The design follows a modular and readable structure, making it suitable for learning computer architecture as well as experimenting with RISC-V cores.

---

## 📌 Overview

The processor implements a **single-cycle datapath**, where each instruction completes in one clock cycle.  
It follows the standard RISC-V architecture principles and is written entirely in **Scala using Chisel 3**.

---

## ✨ Features

- RV32I instruction set (subset)
- Single-cycle (non-pipelined) architecture
- Modular and readable Chisel design
- Separate instruction and data memory
- Synthesizable RTL
- Easy to extend (pipeline, hazards, etc.)

---

## 🧠 Supported Instructions (Example)

- **R-type**: `ADD`, `SUB`, `AND`, `OR`, `XOR`, `SLT`
- **I-type**: `ADDI`, `LW`
- **S-type**: `SW`
- **B-type**: `BEQ`
- **U-type**: `LUI`
- **J-type**: `JAL`

---

## 🧩 Processor Components

- Program Counter (PC)
- Instruction Memory
- Control Unit
- Register File
- ALU
- Immediate Generator
- Data Memory
- ALU Control
- JALR

---

## 🛠️ Tools & Technologies

- **Scala**
- **Chisel 3**
- **SBT (Scala Build Tool)**
- **Verilator** (optional, for simulation)

---

