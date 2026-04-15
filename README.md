# 🔷 OAI221 Domino Logic Design (VLSI Project)

## 📌 Overview
This project focuses on the **design, simulation, and layout implementation** of an **OAI221 gate using Domino Logic**.  

Two implementations are analyzed:
- ✔ Complex Gate (Optimized implementation)
- ✔ Non-Complex Gate (Expanded logic implementation)

The project evaluates:
- Area
- Power consumption
- Delay
- Layout efficiency
- PVT variations

---

## 🎯 Objectives
- Design OAI221 gate using **Domino logic**
- Compare **complex vs non-complex implementations**
- Perform:
  - Pre-layout simulation
  - Post-layout simulation
  - Monte Carlo analysis
- Evaluate **power, delay, and area trade-offs**

---

---

## 🧠 Design Approach

### 1️⃣ Complex Gate Design
- Direct implementation of logic using fewer transistors
- Optimized pull-down network
- Uses:
  - Precharge transistor
  - Evaluation network
  - Keeper transistor

📌 Schematic shown in project report :contentReference[oaicite:0]{index=0}  

---

### 2️⃣ Non-Complex Gate Design
- Logic broken into smaller sub-blocks
- Uses more transistors and interconnections
- Higher routing complexity

📌 Schematic shown in project report :contentReference[oaicite:1]{index=1}  

---

## 🧱 Layout Implementation

### Complex Gate
- Area: **7.787 µm²**

### Non-Complex Gate
- Area: **15.704 µm²**

👉 Non-complex layout uses ~2× area :contentReference[oaicite:2]{index=2}  

---

## ✅ Physical Verification
- ✔ DRC Clean  
- ✔ LVS Matched  

Ensures correct layout-to-schematic mapping :contentReference[oaicite:3]{index=3}  

---

## 🧪 Functional Simulation

### Verified Cases:
- A=1, B=1, C=1, D=1, E=1 → Output = 0  
- A=0, B=0, C=0, D=1, E=0 → Output = 1  

✔ Correct functionality confirmed :contentReference[oaicite:4]{index=4}  

---

## ⚡ Power Analysis (Pre vs Post Layout)

| Parameter | Complex (Post) | Non-Complex (Post) |
|----------|---------------|--------------------|
| Leakage | 115.27 nA | 207.4 nA |
| Static Power | 139 nW | 271 nW |
| Dynamic Power | 69.7 µW | 77.7 µW |

👉 Complex gate consumes **~12% less power** :contentReference[oaicite:5]{index=5}  

---

## ⏱️ Delay Analysis

### Fall Time (ns)
- Increases under:
  - Lower voltage (SS corner)
  - Higher temperature  

### Rise Delay (ns)
- Higher in complex gate due to stacked transistors  
- Post-layout delay slightly higher due to parasitics  

📌 Detailed timing tables available in report :contentReference[oaicite:6]{index=6}  

---

## 📉 Monte Carlo Analysis

- Performed for **process variation**
- Example:
  - Delay ≈ **5.23 ns (average)**

✔ Confirms robustness under variation :contentReference[oaicite:7]{index=7}  

---

## ⚖️ Comparison: Complex vs Non-Complex

| Parameter | Complex | Non-Complex |
|----------|--------|------------|
| Transistors | 12 | 24 |
| Area | 7.787 µm² | 15.704 µm² |
| Power | Lower | Higher |
| Complexity | Moderate | High |
| Performance | Better | Slower |

👉 Complex gate is clearly more efficient :contentReference[oaicite:8]{index=8}  

---

## 🔁 Pre vs Post Layout Insights
- Power slightly increases due to parasitics  
- Delay increases due to routing capacitance  
- Functional behavior remains correct  

---

## 🛠️ Tools Used
- Cadence Virtuoso  
- Spectre Simulator  
- Calibre (DRC/LVS)  
- Monte Carlo Analysis  

---

## 📂 Project Structure
.
├── Schematic/
├── Layout/
├── Simulation/
├── Results/
├── Reports/


---

## 📌 Key Learnings
- Domino logic design methodology  
- Trade-offs between:
  - Area vs Power vs Delay  
- Impact of:
  - Parasitics (post-layout)  
  - Process variations (Monte Carlo)  
- Importance of:
  - Efficient transistor-level design  

---

## 🚀 Conclusion
- Successfully designed and verified **OAI221 Domino Logic gate**
- Complex implementation shows:
  - Lower area  
  - Lower power  
  - Better performance  
- Demonstrates real-world **VLSI design trade-offs**

---

## 👨‍💻 Authors
- Rajnesh Kumar  
- Rahul  
- Abhishek Bhooshan  
- Kabeer Kundra  

--

