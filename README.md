# Encryption-Decryption-Memory-System

#  LFSR-Based Data Memory System

##  Overview  
This project builds upon the LFSR-Based Memory System, implementing a **Linear Feedback Shift Register (LFSR) Based Data Memory System** in **SystemVerilog**. The system manages **memory read/write operations**, utilizes **LFSR for pseudo-random sequences**, and explores additional functionalities such as **encryption/decryption**.

 **Part 1** – Read/write memory with LFSR integration.  
 **Part 2** – Attempted implementation of enhanced encryption features.  

---

##  Features  
- **Linear Feedback Shift Register (LFSR)** – Generates pseudo-random sequences for testing.  
- **Memory System** – Implements **data memory storage and access** (`dat_mem.sv`).  
- **State-Based Control Logic** – Controls memory transactions.  
- **Encryption/Decryption Attempt** – Explored but encountered issues in **Part 2**.  

---

##  File Structure  

### **Part 1**  
| File | Description |  
|------|------------|  
| `dat_mem.sv` | Implements data memory storage and operations. |  
| `lfsr6b.sv` | Implements a modified 6-bit LFSR for sequence generation. |  
| `top_level_5b_start.sv` | Manages system integration and high-level control. |  

### **Additional Files**  
| File | Description |  
|------|------------|  
| `Lab5.pdf` | Lab report detailing implementation, issues, and challenges. |  

---

##  Simulation & Testing  
### **Requirements**  
- **SystemVerilog Compiler** (e.g., ModelSim, QuestaSim, Quartus)  
- **Testbench for Validation**  

### **Running the Simulation**  
1️⃣ **Compile the SystemVerilog files**  
```sh
vlog dat_mem.sv lfsr6b.sv top_level_5b_start.sv
```  
2️⃣ **Run the simulation**  
```sh
vsim -c -do "run -all" top_level_5b_start
```  
3️⃣ **Check the waveform output** or **debug memory operations**.  

---

##  Issues Encountered  
### **Part 1**  
- **Address Mapping Errors** – Initial issues with associating read/write addresses with cycle counts.  
- **LFSR Pattern Matching** – Required adjustments for correct pattern identification.  

### **Part 2**  
- **Data Output Corruption** – `data_out` became **unusable when integrated into case 72**.  
- **Decryption Errors** – The first letter of each decrypted string was **cut off**, with no workaround found.  
- **Unresolved Bugs** – Part 2 remains incomplete due to the above issues.  

---

##  Contributors  
- **Joachim Galil**  
- **Sean King** 
