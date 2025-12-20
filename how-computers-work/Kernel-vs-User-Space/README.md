# OS Basics – Kernel vs User Space

## Operating System
The Operating System controls hardware and manages system resources.
Programs cannot run without it.

---

## Execution Spaces
An OS separates execution into two spaces:
- User Space
- Kernel Space

---

## User Space
User space is where applications run.

Characteristics:
- limited permissions
- cannot access hardware directly
- crashes do not crash the OS

Examples:
- C programs
- shell commands
- editors

---

## Kernel Space
Kernel space is where the OS kernel runs.

Responsibilities:
- CPU scheduling
- memory management
- process management
- filesystem access
- hardware drivers

Kernel has full system access.

---

## System Calls
System calls are the interface between user space and kernel space.

Examples:
- read
- write
- open
- close
- fork
- execve

User programs use system calls to request services from the kernel.

---

## Segmentation Fault
A segmentation fault occurs when a program accesses invalid memory.
The kernel detects this and terminates the process.

---

## Key Takeaway
Programs run in user space.
The kernel controls hardware.
System calls connect the two.
