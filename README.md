[addvars.txt](https://github.com/user-attachments/files/21824720/addvars.txt)

1. Thought Process:
  
![asm2](https://github.com/user-attachments/assets/9bec63a8-0493-403e-adf1-2e1a3d81b93a)

   
2. Challenges:

   Running a program does not print anything unless system calls are implemented.
   Understanding GDB commans was challenging & caused many errors initially. Had to learn how to properly use command step by step to inspect     memory.
   It was not clear whether the reaul was being correctly recognized by GDB.

   

4. Working Code:
  
  
  [Uplsection .text
        global _start

_start:
        ;======== write your code below ===========
        mov eax, [var1]
        add eax, [var2]
        mov [result], eax
        ;======== write your code above ===========

        mov eax,1
        int 0x80

segment .bss
        result resd 1

segment .data
        var1 dd 10
        var2 dd 15
oading addvars.txt…]()

  
 ![1](https://github.com/user-attachments/assets/fcae0806-2335-4d89-a040-db86b06fa623)

