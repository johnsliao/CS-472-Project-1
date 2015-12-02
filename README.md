# CS-472-Project-1

CS 472 - Computer Architecture (Taken SUMMER 2015)

MIPS Disassembler

Your project is to write a partial disassembler for MIPS instructions. That is, your input will be the 32-bit machine instructions that a compiler or assembler produces.  Your program then figures out what the original source instructions were that created those 32-bit machine instructions and outputs them.  The possible source instructions that you must be able to disassemble are: add, sub, and, or, slt, lw, sw, beq, bne.  Ignore all other MIPS instructions.  

The specific machine instructions that you will disassemble (one after another in this exact order) are:
0x022DA822, 0x8EF30018, 0x12A70004, 0x02689820, 0xAD930018, 0x02697824, 0xAD8FFFF4, 
0x018C6020, 0x02A4A825, 0x158FFFF6, 0x8E59FFF0

That is, the above 32-bit instructions will be the input to your program.  (Eight hex digits are 32 binary bits.)  Feel free to embed them in the program itself so you can avoid typing them in each time.  Your program will then analyze a 32-bit instruction and figure out what the opcode, register operands and other fields in the instruction are and then print out the assembly language instruction that produced it.  Assume that the first instruction begins at address hex 7A060 and the rest follow right after that one.  You must output the address along with the instruction.
