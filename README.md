# CSCD95

This document will serve as the guide for the CSCD95 computer science project course

## Goals 
The main aim of to build an OS similar to pintOS in C69 but the goal is do it completely
from scratch in Rust. And boot the OS on bare metal hardware (Raspberry Pi) or an emulator (QEMU)

## Topics
- OS design 
- x86 assembly or ARM
- Rust 

## Resources 
- https://grasslab.github.io/NYCU_Operating_System_Capstone/labs/lab0.html
- https://raw.githubusercontent.com/tuhdo/os01/master/Operating_Systems_From_0_to_1.pdf
- https://pdos.csail.mit.edu/6.828/2018/xv6/book-rev10.pdf
- https://github.com/phil-opp/blog_os
- https://wiki.osdev.org
- https://github.com/thepowersgang/rust-barebones-kernel

## Outline

|Week| Topics | Description  |  Resourses |
|---|---|---|---|
| 1  | Bootloader   | The bootloader is a responsible for loading up basic system before transfering control to the OS. The first week will involve writing a bootloader in rust. Following example implementation already exists in rust. The goal is to study the example source code and be able to fully understand what the code is trying to accomplish | https://github.com/rust-osdev/bootimage  |
| 2   | Exceptions/Interupt Handling  | Setup exception and interrupt handling mechanism  | https://os.phil-opp.com/cpu-exceptions/ |
| 3-4   | Memory Allocator/Virtual Memory  | Setup paging and virtual memory. Plus memory allocation enabling rust to be able to use dynamic memory. Implement different memory allocation schemes to see the differences and advantage of each one. (Ex. Fixed-Blocked Allocation, Buddy System)  |
| 5-6   | Threads/User Process   |  Implement a scheduler, threads/processes, context switching   |
| 7-8   | File systems |  Implement virtual file systems + concrete file systems such as FAT32, NTFS |
| 8-9   | N/A  | to be determined  |
| 10-12 | N/A |  to be determined  |