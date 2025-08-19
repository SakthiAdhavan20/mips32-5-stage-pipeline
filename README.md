# Design of 5-Stage Pipelined MIPS32 RISC Processor

This repository contains the details and Verilog implementation of a MIPS32 ISA-based RISC Processor, designed with a 5-stage pipelined architecture.

---

## Table of Contents
1. [Abstract](#abstract)  
2. [Introduction](#introduction)  
3. [Design and Implementation](#design-and-implementation)  
   - [ISA Overview](#isa-overview)  
   - [Datapath Diagrams](#datapath-diagrams)  
   - [Modules](#modules)  
4. [Results and Verification](#results-and-verification)  
5. [Conclusion](#conclusion)  
6. [How to Run](#how-to-run)  
7. [References](#references)  

---

## Abstract
The objective of this project is to design and implement a 32-bit processor using Icarus Verilog and GTKWave, based on the Microprocessor with Interlocked Pipeline Stages (MIPS) instruction set. The processor follows the properties of the original MIPS architecture and demonstrates pipelined instruction execution with improved throughput.

---

## Introduction
- Motivation for pipelining in processors.  
- Overview of the MIPS32 Instruction Set Architecture used.  
- Objective of this project.

---

## Design and Implementation

### ISA Overview
- Supported instructions include arithmetic, logic, load/store, branch, and jump instructions.  
- Instruction formats: R-type, I-type, and J-type.  

### Datapath Diagrams
- Non-pipelined datapath diagram.  
- 5-stage pipelined datapath diagram.

### Modules
- Control Unit  
- Register File  
- ALU  
- Pipeline Registers  
- Data Memory  
- Forwarding and Hazard Detection Units  

---

## Results and Verification
- Simulation results for key instructions (ADD, SUB, LW, SW, BEQ, JUMP).  
- Waveform snapshots for verification.  
- Console output showing register and memory updates.

---

## Conclusion
- Achievements of the project.  
- Limitations, if any.  
- Possible future improvements such as branch prediction, exception handling, or supporting more instructions.

---

## How to Run

### Requirements
- Icarus Verilog  
- GTKWave  

### Steps
```bash
# Compile
iverilog -o mips32_sim.out top_module.v testbench.v

# Run simulation
vvp mips32_sim.out

# View waveforms
gtkwave dump.vcd

```
## References

Computer Organization and Design – Patterson & Hennessy

NPTEL & IIT KGP lecture notes on Verilog and hardware design

Other online resources and research papers

