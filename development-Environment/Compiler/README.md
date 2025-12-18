### GCC Compiler
- What is GCC?
  GCC (GNU Compiler Collection) is a tool that turns C code into a program you can run.
- `Preprocessing`
  * Expands macros          // exp:  #define SIZE 10
  * Includes header files   // exp:  #include <stdio.h>
- `Compilation`
  * The C code is checked for syntax errors
  * C code is translated into assembly code  main.c → main.s
- `Assembly`
  * Assembly code is converted into machine code
  * Creates an object file  main.s → main.o
- `Linking`
  * Combines all .o files together
  * Links libraries  main.o + printf.o + other libraries → a.out
> [!NOTE]
> When you run `gcc main.c` GCC automatically does
>
>     Preprocessing → Compilation → Assembly → Linking
