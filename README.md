# Design of 5-Stage Pipelined MIPS32 RISC Processor

This repository contains the details and Verilog implementation of a **MIPS32 ISA based RISC Processor**, designed with a **5-stage pipelined architecture**.

---

##  Table of Contents
1. [Abstract](#abstract)  
2. [Introduction](#introduction)  
3. [Design & Implementation](#design--implementation)  
   - [ISA Overview](#isa-overview)  
   - [Datapath Diagrams](#datapath-diagrams)  
   - [Modules](#modules)  
4. [Results & Verification](#results--verification)  
5. [Conclusion](#conclusion)  
6. [How to Run](#how-to-run)  
7. [References](#references)  

---

## 🔹 Abstract
*A short summary (3–4 lines) about what the project is, why it’s important, and the outcomes.*  

---

## 🔹 Introduction
- Motivation for pipelining in processors.  
- Overview of the **MIPS32 Instruction Set Architecture** used.  
- Objective of this project.  

---

## 🔹 Design & Implementation  

### ISA Overview  
Brief explanation of supported instructions and their formats.  

### Datapath Diagrams  
- Non-pipelined datapath diagram.  
- Pipelined 5-stage datapath diagram.  

### Modules  
- Control Unit  
- Register File  
- ALU  
- Pipeline Registers  
- Data Memory  
- Forwarding & Hazard Detection Units (if implemented)  

---

## 🔹 Results & Verification  
- Waveform simulation results for key instructions:  
  - ADD, SUB, LW, SW, BEQ, JUMP, etc.  
- Console output snapshots (register & memory updates).  
- Verification of hazard handling (Forwarding & Stalling).  

---

## 🔹 Conclusion  
- ✅ Achievements of the project.  
- ⚠️ Limitations (if any).  
- 🚀 Future improvements (branch prediction, more instructions, exception handling).  

---

## 🔹 How to Run  

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

