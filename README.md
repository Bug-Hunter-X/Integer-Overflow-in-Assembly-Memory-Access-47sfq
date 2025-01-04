# Integer Overflow in Assembly Memory Access

This repository demonstrates a common but subtle bug in assembly code: integer overflow during memory address calculation. The code snippet `mov eax, [ebx + ecx*4]` is vulnerable because the addition and multiplication can exceed the maximum addressable memory, leading to undefined behavior.

The `bug.asm` file contains the vulnerable code, while `bugSolution.asm` provides a solution that mitigates the risk of overflow by adding checks before the memory access.  This example highlights the importance of careful memory management and input validation in low-level programming.