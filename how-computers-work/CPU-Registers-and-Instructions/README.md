# CPU Basics – Registers and Instructions

## What is the CPU?
The CPU (Central Processing Unit) is the component that executes programs.
It reads instructions from memory and runs them one by one.

---

## Main CPU Components
- ALU: performs arithmetic and logic operations
- Registers: very fast, small memory inside the CPU
- Control Unit: manages instruction execution

---

## Registers
Registers are used to store temporary data while the CPU executes instructions.

Characteristics:
- Extremely fast
- Very small
- Used for values, addresses, counters, and return values

The CPU works mainly with registers, not directly with RAM.

    RAM → Register → CPU operation → Register → RAM

---

## Instructions
An instruction is a low-level command understood by the CPU.

Examples:
- move data
- add values
- compare values
- jump to another instruction

---

## Instruction Cycle
The CPU follows this cycle continuously:
1. Fetch instruction from memory
2. Decode instruction
3. Execute instruction
 > This repeats millions of times per second.

Exampl :

    x = a + b;

    load a into register
    load b into register
    add registers
    store result in x
    
> [!IMPORTANT]
> - CPU executes instructions
>
> - Registers hold temporary data
>
> - RAM stores program data
>
> - Stack manages function calls


---

## Relation to C Programming
- C is close to hardware
- Function calls use stack and registers
- Return values are passed via registers
- Memory errors affect instruction execution

---

## Key Takeaway
Understanding CPU basics helps with:
- debugging segmentation faults
- understanding stack behavior
- writing efficient C code

> [!NOTE]
> The CPU executes instructions using registers,
> following a strict execution cycle, and C code maps closely to this process.










