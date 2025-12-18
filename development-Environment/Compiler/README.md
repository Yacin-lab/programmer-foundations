### GCC Compiler
- What is GCC?
  
  GCC (GNU Compiler Collection) is a tool that turns C code into a program you can run.
- `Preprocessing`
  * Expands macros          // exp:  #define SIZE 10
  * Includes header files   // exp:  #include <stdio.h>
- `Compilation`
  * The C code is checked for syntax errors
  * C code is translated into assembly code,  main.c → main.s
- `Assembly`
  * Assembly code is converted into machine code
  * Creates an object file,  main.s → main.o
- `Linking`
  * Combines all .o files together
  * Links libraries,  main.o + printf.o + other libraries → a.out

> [!NOTE]
> When you run `gcc main.c` GCC automatically does
>
>     Preprocessing → Compilation → Assembly → Linking

### Makefile
- What is a Makefile?
  A Makefile automates compilation so you can build your program with make.
  
  Avoids typing the same command

  ### Exampl:
---

      NAME = program
      SRC = main.c utils.c
      CC = gcc
      CFLAGS = -Wall -Wextra -Werror
      
      all:
      	$(CC) $(CFLAGS) $(SRC) -o $(NAME)
      
      clean:
      	rm -f $(NAME)
---

      `all` → builds the program
      `clean` → removes generated files
  
  ### How to Use It:

      make        // compile
      ./program   // run
      make clean  // delete executable
