# ENCS4370-Computer-Architecture-Project-2

# Objectives:
This project aims to design and verify a basic RISC processor using Verilog. The processor is defined by the following specifications:

# Processor Specifications:
1) Instruction size: 32 bits 
2) 32-bit general-purpose registers (R0 to R31)  
3) Special purpose register for the program counter (PC) 
4) Control stack to save return addresses   
5) Stack pointer (SP) to point to the top of the control stack (initialized to zero) 
6) Four instruction types: R-type, I-type, J-type, and S-type
7) ALU with a "zero" signal indicating if the last operation result is zero 
8) Separate data and instruction memories 

# Instruction Types and Formats:
Common Fields:
  1) 2-bit instruction type (00: R-Type, 01: J-Type, 10: I-Type, 11: S-Type)
  2) 5-bit function code
  3) Stop bit (marks the end of a function code block)  
Instruction Formats:
R-Type (Register Type) Format:
  1) 5-bit Rs1 (first source register)
  2) 5-bit Rd (destination register)
  3) 5-bit Rs2 (second source register)
  4) 9-bit unused
I-Type (Immediate Type) Format:
  1) 5-bit Rs1 (first source register)
  2) 5-bit Rd (destination register)
  3) 14-bit immediate (unsigned for logic instructions, signed otherwise)
J-Type (Jump Type) Format:
  1) 24-bit signed immediate (jump offset)
S-Type (Shift Type) Format:
  1) 5-bit Rs1 (first source register)
  2) 5-bit Rd (destination register)
  3) 5-bit Rs2 (second source register) for variable shift amounts
  4) 5-bit SA (constant shift amount)
  5) 4-bit unused

# Instructions' Encoding:
  * A subset of instructions is implemented, including AND, ADD, SUB, CMP, ANDI, ADDI, LW, SW, BEQ, J, JAL, SLL, SLR, SLLV, and SLRV. 

# summary
This project involves designing, implementing, and verifying a RISC processor in Verilog, emphasizing correct functionality, comprehensive testing, and clear documentation.

# Results
![image](https://github.com/lamaNase/ENCS4370-Computer-Architecture-Project-2/assets/138326030/5a958d69-3fda-4af7-b9c0-940ff2652fac)

![image](https://github.com/lamaNase/ENCS4370-Computer-Architecture-Project-2/assets/138326030/32172faf-423b-4c39-9424-2520fc19cdfa)

![image](https://github.com/lamaNase/ENCS4370-Computer-Architecture-Project-2/assets/138326030/3a802c76-e003-4e20-a4c0-e3bdf2678bd3)

![image](https://github.com/lamaNase/ENCS4370-Computer-Architecture-Project-2/assets/138326030/15745f9c-3ce3-4119-af8d-75628fa00005)

![image](https://github.com/lamaNase/ENCS4370-Computer-Architecture-Project-2/assets/138326030/1884745e-00ab-4089-929a-8da2d36894a8)

# Partner
Lama Nasser 1200190
Maha Mali 1200746
Basheer Arouri 1201141




