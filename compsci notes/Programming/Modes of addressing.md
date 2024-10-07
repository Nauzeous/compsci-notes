There are 4 main modes of addressing,

- Immediate
- Indexed
- Direct
- Indirect

Once an instruction has been fetched, it has to be decoded, meaning it turns the machine instruction into two parts

- Opcode - first 4 bits - tells the computer what to do
- Operand - last 4 bits - tells the computer what to do it to

so the instruction 01101110 becomes
0110      1110
   6           14

in the various modes of addressing, the operand can take on different meanings.


## Immediate addressing
In immediate addressing, the value in the operand is accepted as a binary value, meaning it does not have to search memory
this means if the opcode is telling the computer to load a value into the accumulator, the value 14 will be loaded.

## Direct addressing

In direct addressing, the value in the operand is a reference to a memory location
so 0110 1110 means that you load the value in memory location 14

## Indirect addressing





