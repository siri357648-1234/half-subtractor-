# Half Subtractor using Verilog

## 📌 Project Overview

A Half Subtractor is a combinational logic circuit used to subtract one binary digit (B) from another binary digit (A). It has:

### Inputs
- A (Minuend)
- B (Subtrahend)

### Outputs
- Difference (Diff)
- Borrow (Borrow)

---

## Truth Table

| A | B | Difference | Borrow |
|---|---|------------|--------|
| 0 | 0 |     0      |   0    |
| 0 | 1 |     1      |   1    |
| 1 | 0 |     1      |   0    |
| 1 | 1 |     0      |   0    |

---

## Logic Equations

Difference = A XOR B

Borrow = A' AND B

---

## Project Files

- `half_subtractor.v` → Verilog design
- `half_subtractor_tb.v` → Testbench
- `simulation_results.png` → Simulation waveform

---

## Software Used

- Xilinx Vivado
- ModelSim
- Icarus Verilog
- GTKWave

---

## Simulation

Compile and run using Icarus Verilog:

```bash
iverilog -o half_subtractor half_subtractor.v half_subtractor_tb.v
vvp half_subtractor
```

---

## Expected Output

```
A B | Difference Borrow
0 0 |     0         0
0 1 |     1         1
1 0 |     1         0
1 1 |     0         0
```

---

## Author
shirisha 
