**We know array is the most fundamental basic while solving reverse engineering concepts.**
- **Lets see how we see arrays in reverse engineering.**

  [Base+Index*Scale]

- **Imagine this C array**

   int number[5]:

Suppose it looked like this-:

- 1000    -  number[0]
- 1004    -  number[1]
- 1008    -  number[2]
- 1012    -  number[3]
- 1016    -  number[4]

   Suppose ESI=2 that means Index=2

Now look at the instruction-:

**mov esi,[kdLogBuffer+esi*4]**
- Pretend kdLogBuffer=1000
    we have Bse=1000
- The CPU calculates-:
   1000+2*4
   =1008
- Then it reads memory[1008]

     which is number[2]

**Now the question arises why we multiply by 4?** -
Becouse every integer is 4 bytes

  
