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
- read()
- write()
- open()
- close()
- fork()
- execve()

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

---

# Linux Filesystem Structure

## Overview
The filesystem defines how files and directories are stored and organized.

Linux uses a single hierarchical tree starting at `/`.

---

## Root Directory `/`
The root directory is the top of the filesystem.

All files and directories exist under `/`.

[linux-filesystem](https://github.com/Yacin-lab/Uses/blob/main/img/linux-filesystem-hierarchy.png)

---

## Important Directories

- /bin      : essential system commands
- /usr/bin  : user programs
- /lib      : shared libraries
- /etc      : configuration files
- /home     : user home directories
- /tmp      : temporary files
- /var      : variable data (logs, cache)
- /dev      : device files
- /proc     : virtual process information

---

## Files and Inodes
A file consists of:
- data blocks
- metadata stored in an inode

Directories map filenames to inode numbers.

---

## Permissions
Each file has permissions:

- read (r)
- write (w)
- execute (x)

Permissions apply to:
- owner
- group
- others

---

## Paths
- Absolute paths start with `/`
- Relative paths depend on the current directory

---

## Key Takeaway
The filesystem is a tree managed by the kernel.

Everything in Linux is treated as a file.

