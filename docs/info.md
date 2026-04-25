<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

# tt_um_full_adder

## Overview
This design implements a simple 1-bit full adder using the TinyTapeout interface.  
Inputs `a`, `b`, and `c` are taken from `ui_in[0]`, `ui_in[1]`, and `ui_in[2]`.  
The outputs are the sum and carry of the addition.

## Interface
- **Inputs**
  - `ui_in[0]` → operand `a`
  - `ui_in[1]` → operand `b`
  - `ui_in[2]` → carry-in `c`
  - `ena`, `clk`, `rst_n` → unused but tied off to avoid warnings
- **Outputs**
  - `uo_out[0]` → sum
  - `uo_out[1]` → carry
  - `uo_out[7:2]` → tied to 0
  - `uio_out` → tied to 0
  - `uio_oe` → tied to 0

## Functionality
The module computes:
