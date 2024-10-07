
combinational logic circuits are useful for processing data, but it provides no way to maintain a switch state, which is **important for memory**

memory can be built out of logic gates and circuits, which is done using a ==flip-flop==

a flip-flop is a fundamental logic circuit that can store one bit and ==toggle== it between 0 and 1

a flip-flop has two inputs:
- a  single-bit data input (labelled D)
- a clock signal (labelled C)

and two outputs:
- a single-bit data output (labelled Q)
- the inverse of the data output (labelled ¬Q)

[[flipflop]]

a d-type flip-flop is a positive-edge-triggered flip-flop circuit

this means the output can only be changed when the clock pulse is at a positive edge (signal of 1)

when the clock signal is not at a positive edge, the output value ==cannot be changed==

every time the clock signal is at a positive edge, the output **copies** the input D


flip-flop summary:
- a 1-bit memory device that is enabled and disabled by a clock signal
- used in memory circuits and registers
- can be edge-triggered, meaning it is enabled at the moment the clock signal rises from low to high