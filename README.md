# C-Stem
Batman's utility belt equivalent for system programming.

## Description
Working in Systems, I found myself having to write the same code too many times, often in multiple languages.
After a 5 years PhD, I finally realized it might be worth turning these bits of code into re-usable libraries.

This repository includes: 

### DLL
A generic implementation of double-linked-lists using macros.
The first time I wrote this was in 2012 for my OS class at CMU, and the last time was in 2023.


### Common
A simple logging library to print debugging information based on logging-level (feature pending).
The particularity of this code is that it is meant to work both in applications and kernel drivers.
It also defines very useful SUCCESS and FAILURE values.

### Elf64
An ELF64 parsing library. 

### Pts
A generic page table mapper/walker.
For the moment I only have a profile for x86 and Risc-V 4-level page tables, but theoretically it should be super easy to add profiles for, e.g., extended page-tables, I/O MMU page tables etc.
