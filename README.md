# 🚀 RV32I Single-Cycle Processor (SystemVerilog Implementation)

This project implements a **single-cycle (non-pipelined) datapath** for the **RV32I subset** of the **RISC-V Instruction Set Architecture** using **SystemVerilog**. It focuses on the fundamental components needed to execute RISC-V integer instructions and includes a complete suite of testbenches for instruction-level and module-level verification.

---

## 🧠 Project Overview

- 🖥️ **Architecture**: RISC-V RV32I base ISA (Integer-only, 32-bit).
- 🛠️ **Design Style**: Single-cycle (non-pipelined) implementation.
- 💻 **Language**: SystemVerilog (Hardware Description Language).
- 🧪 **Verification**: Included testbenches for unit and integration testing.

---

---

## 🧩 Core Components

- **ALU**: Performs arithmetic and logical operations based on instruction opcode.
- **Control Unit**: Decodes instructions and generates control signals.
- **Register File**: 32 general-purpose 32-bit registers.
- **Instruction Memory**: Stores machine code instructions.
- **Data Memory**: Load/store support for memory-related instructions.
- **Immediate Generator**: Decodes and sign-extends immediate values.
- **PC Logic**: Program counter update logic with branching support.

---

## ✅ Supported Instructions

The processor supports all **RV32I base instructions**, including:

- **R-type**: `add`, `sub`, `sll`, `slt`, `sltu`, `xor`, `srl`, `sra`, `or`, `and`
- **I-type**: `addi`, `andi`, `ori`, `lw`, `jalr`
- **S-type**: `sw`
- **B-type**: `beq`, `bne`, `blt`, `bge`
- **U-type**: `lui`, `auipc`
- **J-type**: `jal`

---

## 🧪 Verification

Testbenches are provided for:

- Individual modules like ALU and Register File.
- Full datapath verification with sample instruction sequences.
- Memory access and control signal validation.

---

## 🧾 How to Run

1. Open your preferred SystemVerilog simulator.
2. Compile the design and testbench files.
3. Run the simulation and inspect waveforms or output logs for correctness.
