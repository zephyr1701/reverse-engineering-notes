## Registers

Registers are the most fundamental concepts in reverse engineering.
Almost every assembly instruction reads data from registers,writes data to registers,or perform many imp instruction
Now we will understand what registers are and how they work.

## What is a Register?

 Think registers as tiny,superfast-storage locations inside the CPU.The CPU uses them to hold data that it is currently working with.
 Think of registers as the CPU's working desk.
 Instead of going to RAM everytime,the CPU first tries to use registers because they are much faster.
 ##
 In Protected mode:-
_ **Each register is 32 bits (4bytes) wide.**
_ **Programs can not directly access all the hardware.**
_ **Memory is protected so one program can not easily corrupt another.**

 ## The x86 architecture has eight 32bit general registers(GPRs)
 1-EAX
 2-EBX
 3-ECX
 4-EDX
 5-ESI
 6-EDI
 7-EBP
 8-ESP

## EAX (Extended Accumulator register)
**Most commonly used register.**
**It often stores:-
1.Return values from functions
2.Arithmetic results
3.Temporary values**
### Example
1. mov eax,5
**This means put the value inside EAX**

## EBX (Extended Base Register)

