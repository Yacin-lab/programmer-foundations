# Compilation and Linking in C

A C program becomes an executable through four stages:

1. Preprocessing
2. Compilation
3. Assembly
4. Linking

---

## 1. Preprocessing
Handles all lines starting with `#`.

Tasks:
- expands #include
- replaces macros (#define)
- removes comments
- handles conditional compilation

Command:
gcc -E main.c

Output: expanded C source code.

---

## 2. Compilation
Checks syntax and translates C code into assembly.

Transformation:
main.c → main.s

Command:
gcc -S main.c

Errors here:
- syntax errors
- type errors

---

## 3. Assembly
Translates assembly code into machine code.

Transformation:
main.s → main.o

Command:
gcc -c main.c

Output:
- object file (.o)
- not executable

---

## 4. Linking
Combines object files and libraries into an executable.

Transformation:
main.o + libraries → executable

Command:
gcc main.o -o program

Errors here:
- undefined reference
- multiple definition

---

## Key Takeaway
Each stage has a specific role.
Understanding the 4 stages is essential for debugging and system-level programming.

[https://github.com/Yacin-lab/Uses/blob/main/img/compilation%20process.png]
