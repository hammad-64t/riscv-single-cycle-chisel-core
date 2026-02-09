### Single-Cycle RISC-V Core in Chisel
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


Start by setting up the working enviroment

### Dependencies

#### JDK 8 or newer

```bash
sudo apt-get install openjdk-11-jdk
sudo apt-get install openjdk-11-jre
```
#### SBT 

SBT is the most common built tool in the Scala community. You can download it [here](https://www.scala-sbt.org/download.html).  

#### VERILATOR
```bash
sudo apt-get install verilator
```

### How to get started

Fork this repository on your own individual profiles. After forking clone the repository and run:

```sh
sbt test
```

You should see a whole bunch of output that ends with something like the following lines
```
[info] Tests: succeeded 1, failed 0, canceled 0, ignored 0, pending 0
[info] All tests passed.
[success] Total time: 5 s, completed Dec 16, 2020 12:18:44 PM
```
If you see the above then...

### It worked!

You are ready to go. Next step is to go inside the `docs/` folder where you will find the labs to perform.

## For quick debugging
If you quickly want to see what verilog is being generated, go to this link  https://bit.ly/3u3zr0e and write Chisel here.

