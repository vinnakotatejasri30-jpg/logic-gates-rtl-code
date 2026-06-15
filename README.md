# logic-gates-rtl-code
# Logic Gates in Verilog HDL

## Overview

This project demonstrates the implementation of basic digital logic gates using Verilog HDL. The design includes the following gates:

* AND
* OR
* NOT
* NAND
* NOR
* XOR
* XNOR

A testbench is provided to verify the functionality of each logic gate by applying all possible input combinations.

---

## Project Structure

```text
├── logic_gates.v       # Verilog design file
├── logic_gates_tb.v    # Testbench file
└── README.md
```

---

## Design Module

### Inputs

| Signal | Description |
| ------ | ----------- |
| a      | Input A     |
| b      | Input B     |

### Outputs

| Signal | Gate              |
| ------ | ----------------- |
| y_and  | AND Output        |
| y_or   | OR Output         |
| y_not  | NOT Output (of a) |
| y_nand | NAND Output       |
| y_nor  | NOR Output        |
| y_xor  | XOR Output        |
| y_xnor | XNOR Output       |

---

## Truth Table

| a | b | AND | OR | NOT(a) | NAND | NOR | XOR | XNOR |
| - | - | --- | -- | ------ | ---- | --- | --- | ---- |
| 0 | 0 | 0   | 0  | 1      | 1    | 1   | 0   | 1    |
| 0 | 1 | 0   | 1  | 1      | 1    | 0   | 1   | 0    |
| 1 | 0 | 0   | 1  | 0      | 1    | 0   | 1   | 0    |
| 1 | 1 | 1   | 1  | 0      | 0    | 0   | 0   | 1    |

---

## Simulation

The testbench applies all possible combinations of inputs `a` and `b`.

```verilog
a=0; b=0;
a=0; b=1;
a=1; b=0;
a=1; b=1;
```

Simulation output is displayed using:

```verilog
$monitor(...)
```

Waveforms are generated using:

```verilog
$dumpfile("dump.vcd");
$dumpvars;
```

---

## Tools Used

* Verilog HDL
* EDA Playground
* Icarus Verilog
* GTKWave

---

## How to Run

1. Open EDA Playground.
2. Paste the design code into the Design section.
3. Paste the testbench code into the Testbench section.
4. Select **Icarus Verilog** as the simulator.
5. Click **Run**.
6. View the output in the console or open the waveform in GTKWave.

---

## Learning Outcomes

* Understanding basic logic gates.
* Verilog gate-level modeling.
* Writing and running testbenches.
* Generating and analyzing simulation waveforms.

---

## Author

**Teja Sri**
B.Tech – Electronics and Communication Engineering (ECE)
