# 🧩 Week 2 – BabySoC Fundamentals & Functional Modelling  
### **Part 1 – Conceptual Understanding**

---

## 📑 **Table of Contents**

1. [What is a System-on-Chip (SoC)?](#1-what-is-a-system-on-chip-soc)  
2. [Main Building Blocks of an SoC](#2-main-building-blocks-of-an-soc)  
3. [Purpose of the BabySoC Model](#3-purpose-of-the-babysoc-model)  
4. [Importance of Functional Modelling in SoC Design](#4-importance-of-functional-modelling-in-soc-design)  
5. [Summary](#5-summary)  
6. [Deliverable](#6-deliverable)  
7. [References](#7-references)

---

## 1. What is a System-on-Chip (SoC)?

A **System-on-Chip (SoC)** is an integrated circuit that combines the core elements of a computer system—such as a processor, memory, input/output interfaces, and control logic—onto a **single silicon chip**.  

This integration enables **smaller size, higher speed, lower power consumption, and faster communication** compared to multi-chip systems.  

SoCs are the foundation of most modern electronics including **smartphones, embedded controllers, and IoT devices**, where they bring together **hardware, firmware, and communication logic** in one compact unit.

---

## 2. Main Building Blocks of an SoC

An SoC is composed of several major subsystems that communicate via an internal interconnect network.

### **a. Processor / CPU Core**
- Acts as the **central control unit** of the SoC.  
- Executes program instructions and manages overall chip operations.  
- Common architectures include **RISC-V**, **ARM**, and **MIPS**.  
- Contains the ALU, control logic, and register files.

### **b. Memory Subsystem**
- Stores both instructions and data.  
- Typically includes:  
  - **Volatile memory (SRAM/DRAM)** – temporary storage for runtime operations.  
  - **Non-volatile memory (ROM/Flash)** – used for boot code and configuration data.

### **c. Peripheral Interfaces**
- Allow the SoC to communicate with the external world.  
- Examples include **UART**, **SPI**, **I²C**, **Timers**, **GPIO**, and **ADC/DAC** modules.  
- Enable interaction with sensors, actuators, and communication devices.

### **d. Interconnect / Bus Fabric**
- Serves as the **data highway** connecting CPU, memory, and peripherals.  
- Common protocols: **AMBA (AHB/APB)** and **Wishbone**.  
- Handles signal timing, arbitration, and data flow management.

### **e. Clock and Reset Circuits**
- The **clock** synchronizes all sequential operations.  
- The **reset** brings every module into a defined startup state, ensuring reliable operation after power-up.

---

## 3. Purpose of the BabySoC Model

The **BabySoC** is a **simplified educational model** of a full-fledged SoC, used in the VSD learning journey to demonstrate essential system-level interactions.  

**Why it’s valuable for learners:**
- Clearly illustrates how CPU, memory, and peripherals exchange data.  
- Removes unnecessary design complexity such as multi-core or pipeline logic.  
- Works seamlessly with **open-source EDA tools (Icarus Verilog and GTKWave)**.  
- Encourages hands-on learning through simulation of clocks, resets, and data signals.  

This simplified SoC bridges theory with practice and helps students build confidence before moving toward RTL or physical design.

---

## 4. Importance of Functional Modelling in SoC Design

**Functional Modelling** is carried out **before RTL implementation and layout** to ensure that every block in the system behaves as intended.

### **Goals**
- Verify the **logical correctness** of the design.  
- Catch communication or integration errors **early in the workflow**.  
- Use waveform analysis to study clock, reset, and data transitions.  
- Ensure the SoC architecture performs correctly before synthesis.

### **Tools Used**
- **Icarus Verilog (iverilog):** open-source Verilog compiler and simulator.  
- **GTKWave:** waveform viewer that reads `.vcd` (Value Change Dump) files to visualize signal transitions.

### **Typical Workflow**
1. Compile the BabySoC Verilog files using `iverilog`.  
2. Run the simulation to produce a `.vcd` file.  
3. Open the waveform in `gtkwave` to inspect reset, clock, and data flow.  

This stage acts as a **checkpoint between conceptual and RTL design**, validating design logic before physical implementation.

---

## 5. Summary

The **BabySoC** experiment provides an excellent foundation to understand:
- The structural organization of a typical SoC (CPU, memory, and peripherals).  
- The timing and synchronization between modules.  
- The significance of verifying functional behavior with **open-source tools**.  

By mastering BabySoC fundamentals, students establish a strong base to progress into **RTL design**, **synthesis**, and **physical design**, gaining a complete perspective of the SoC workflow.

---

## 6. Deliverable

Upload this conceptual report to your GitHub repository as both Markdown (`.md`) and optional PDF (`.pdf`) files.

### **Required Sections**
- Overview of SoC fundamentals  
- Explanation of SoC components  
- Purpose of the BabySoC model  
- Role of functional modelling prior to RTL/physical design  

---

## 7. References

1. **Hemanth Kumar D M**, *SFAL-VSD SoC Journey – Fundamentals of SoC Design (BabySoC)*  
   🔗 [https://github.com/hemanthkumardm/SFAL-VSD-SoC-Journey](https://github.com/hemanthkumardm/SFAL-VSD-SoC-Journey)

2. **VLSI System Design (VSD) Initiative** – *BabySoC Learning Modules and Simulation Framework*  
   🔗 [https://www.vlsisystemdesign.com/](https://www.vlsisystemdesign.com/)

3. **Open-Source Tool Documentation:**  
   - [Icarus Verilog Manual](https://steveicarus.github.io/iverilog/)  
   - [GTKWave User Guide](https://gtkwave.sourceforge.net/)

