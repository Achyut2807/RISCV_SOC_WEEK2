# Week 2 – BabySoC Fundamentals & Functional Modelling

This repository contains all the **concepts, practical results, and documentation** for **Week 2** of the **VSD SoC Design Journey**, focused on understanding and implementing **BabySoC fundamentals** through **functional modelling**.

---

## 📘 Table of Contents
1. [Overview](#1-overview)  
2. [Part 1: Conceptual Understanding](#2-part-1-conceptual-understanding)  
3. [Part 2: Hands-on Functional Modelling](#3-part-2-hands-on-functional-modelling)  
4. [References](#4-references)

---

## 1. Overview

Week 2 emphasizes building a strong foundation in **System-on-Chip (SoC)** architecture while gaining **practical exposure** to functional verification using open-source tools.

### **Learning Outcomes**
- Grasp the **architecture and core components** of an SoC.  
- Understand **data exchange** between CPU, Memory, and Peripherals.  
- Perform **functional simulation** using *Icarus Verilog* and visualize results with *GTKWave*.  
- Document findings through waveform-based observations and analysis.

This week is structured into two key segments — a **conceptual theory module** and a **hands-on simulation exercise**.

---

## 2. Part 1: Conceptual Understanding

**Objective:**  
Develop a theoretical understanding of SoC design flow using the simplified **BabySoC model**.

### **Included Topics**
- Definition and role of a **System-on-Chip (SoC)**  
- Breakdown of SoC elements: **CPU, Memory, Peripherals, Bus, Clock & Reset**  
- Purpose and advantages of the **BabySoC learning model**  
- Role of **functional modelling** before RTL design and physical implementation  
- Summary and interpretation of theoretical learnings

**Deliverable:**  
A Markdown report summarizing theoretical insights, supported by relevant diagrams and references.  

📂 **Link to File:** [Part 1 – Conceptual Understanding](./PART-1/deliverables.md)

---

## 3. Part 2: Hands-on Functional Modelling

**Objective:**  
Simulate and analyze BabySoC behavior using open-source tools to understand functional verification in SoC design.

### **Practical Steps**
- Compile BabySoC Verilog modules using **Icarus Verilog (iverilog)**.  
- Run simulations to generate `.vcd` waveform files.  
- Analyze **clock**, **reset**, and **dataflow** between CPU, Memory, and Peripherals using **GTKWave**.  
- Record observations and screenshots demonstrating each step.  

**Deliverables:**
- `sim.log` – simulation log output  
- `.vcd` file – waveform data  
- `screenshots/` – waveform captures with captions  
- README – short description of each observation and result  

📂 **Link to Folder:** [Part 2 – Hands-on Functional Modelling](./Part2_Functional_Modelling/)

---

## 4. References

1. **Hemanth Kumar D M**, *SFAL-VSD SoC Journey – Fundamentals of SoC Design (BabySoC)*  
   🔗 [https://github.com/hemanthkumardm/SFAL-VSD-SoC-Journey](https://github.com/hemanthkumardm/SFAL-VSD-SoC-Journey)

2. **Icarus Verilog Documentation**  
   🔗 [https://steveicarus.github.io/iverilog/](https://steveicarus.github.io/iverilog/)

3. **GTKWave User Manual**  
   🔗 [https://gtkwave.sourceforge.net/](https://gtkwave.sourceforge.net/)

---

> 🧠 *This repository showcases both theoretical and practical aspects of SoC functional modelling using BabySoC — bridging the gap between system architecture concepts and real-world hardware simulation.*
