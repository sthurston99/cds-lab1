# Problem Statement

The goal of this lab is to use VHDL to build a FSM that detects whether or not a value "w" is high or low for a period of 4 clock cycles or more. From the problem statement and simple derivation there are only 9 states needed, an initial state, and then 4 states for each sequence of flipflops that store the number of clock cycles.

Sidenote: Theoretically, this problem could be optimized using a simple counting circuit with the reset tied to any positive or negative edge of the "w" input, with simple combinatoric logic detecting whether the counter has reached 4 (in this case, 100, for an optimized minimum 3-bit counter, storing the 3rd bit high state in a flipflop until the circuit reset is triggered by a change in the "w" input).

This project should contain vhdl files developed for the DE-10 standard FPGA, and project management files for Quartus Prime that will allow for simulation and writing via the software. With successful deployment, this vhdl should be portable across multiple altera compatible FPGAs, and with some minor modification, xilinx FPGAs.
