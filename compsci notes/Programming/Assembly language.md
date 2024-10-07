The first languages for the first computers were machine code (binary) that required input as 1s and 0s

Programming in binary was difficult so ==assembly language== was created, substituting binary code with **mnemonics** (abbreviations)

All assembly languages are classified as **low-level languages**

Assembly language is directly translated into machine code by an ==assembler==

# LMC instruction set

- ADD
- SUB
- STA - store
- LDA - load
- BRA - branch always
- BRZ - branch if accumulator is 0
- BRP - branch if accumulator is positive
- INP - input
- OUT
- HLT - end program
- DAT - data location

Actual instruction sets are much more expansive

# LMC layout
![[LMC layout.png]]

Important things to note on LMC

- LMC cannot discern instructions from data in RAM
- Labels before data locations act like a variable
- \\\\ is used to add comments 