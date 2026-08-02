# 1-Bit Full Subtractor using Verilog

## Project Description
A Full Subtractor is a combinational logic circuit that subtracts three binary inputs:
- A (Minuend)
- B (Subtrahend)
- Bin (Borrow Input)

It produces two outputs:
- Difference (Diff)
- Borrow Out (Bout)

## Truth Table

| A | B | Bin | Diff | Bout |
|---|---|-----|------|------|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 1 |
| 0 | 1 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 0 |
| 1 | 1 | 0 | 0 | 0 |
| 1 | 1 | 1 | 1 | 1 |

## Boolean Equations

Difference = A ⊕ B ⊕ Bin

Borrow Out = (~A & B) | (~A & Bin) | (B & Bin)

## Files

- full_subtractor.v
- full_subtractor_tb.v
- README.md

## Software Required

- ModelSim
- Vivado Simulator
- Xilinx ISE
- EDA Playground
- Icarus Verilog

## Compilation

Compile:

iverilog full_subtractor.v full_subtractor_tb.v

Run:

vvp a.out
