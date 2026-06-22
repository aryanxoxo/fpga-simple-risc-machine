# Simple RISC Machine using Verilog and the DE1-SoC

Clean public archive for a Verilog RISC-style processor project targeting the DE1-SoC FPGA workflow. The design includes a top-level hardware wrapper, CPU control logic, datapath, register file, ALU, and shifter modules.

## What is included

- `rtl/` - Verilog source for the CPU, datapath, ALU, register file, shifter, and top-level DE1-SoC wrapper.
- `quartus/` - Quartus project and pin-assignment files preserved for hardware rebuild.
- `sim/` - ModelSim project/session files from the original verification workflow.
- `docs/` - sanitized collaboration note.

## Hardware and tools

- Terasic DE1-SoC / Cyclone V style FPGA board
- Intel Quartus Prime
- ModelSim / Questa
- Verilog RTL design flow

## Suggested build path

1. Open `quartus/lab7.qpf` in Quartus.
2. Confirm the top-level module and pin assignments from `quartus/lab7_top.qsf`.
3. Compile the design and inspect timing/resource reports locally.
4. Use the ModelSim project files in `sim/` to recreate the simulation workspace.
5. Program the DE1-SoC board after simulation and timing review.

This repository is intentionally source-focused. Generated Quartus databases, reports, bitstreams, and simulator caches are excluded so the project evidence stays compact and reviewable.

