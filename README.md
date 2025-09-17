# Virtual Memory Simulation

## Overview
This project simulates the concept of virtual memory management in operating systems. Virtual memory allows an OS to use hardware and software to manage memory more efficiently, enabling processes to run as if they have access to a large, contiguous block of memory, even when physical memory is limited. This simulation provides a simplified model to help understand how memory management units (MMU), process scheduling, and page replacement algorithms work together to manage memory in a multi-process environment. It is designed for educational purposes, making it easier to visualize and experiment with core OS concepts.

## Features
- Simulates multiple processes and their individual memory requirements
- Implements a basic memory management unit (MMU) that handles address translation and page table management
- Demonstrates page replacement algorithms such as FIFO (First-In-First-Out) and LRU (Least Recently Used)
- Includes process scheduling to show how the OS manages CPU time among competing processes
- Provides detailed logging and output to help users understand the flow of memory operations
- Modular code structure for easy understanding and extension

## File Structure
- `master.c`: Main controller for the simulation, coordinates process and memory management
- `mmu.c`: Contains logic for the memory management unit, including page table operations
- `proc.c`: Handles process creation, management, and termination
- `sched.c`: Implements process scheduling algorithms
- `includes.h`: Header file with common includes and definitions
- `makefile`: Build instructions for compiling the project
- `rem.sh`: Shell script for cleaning up build artifacts
- `LA8.pdf`: Assignment description and requirements

## Build Instructions
1. Ensure you have a C compiler (e.g., GCC) installed on your system.
2. Open a terminal in the project directory.
3. Run the following command to build the project:
   ```sh
   make
   ```
4. To clean up build files, run:
   ```sh
   ./rem.sh
   ```

## Usage
After building, run the executable generated (usually `master.exe` or `master`):
```sh
./master
```
The program will prompt you to enter the number of processes, memory size, and other simulation parameters. It will then display the results of memory allocation, page faults, and scheduling decisions. Example output includes:

- Process creation and termination logs
- Page table status for each process
- Page fault occurrences and handling
- Scheduling order and context switches

This helps users visualize how virtual memory works and how different algorithms affect system performance.

## Requirements
- GCC or compatible C compiler
- Windows, Linux, or macOS

## References
- [Operating System Concepts, Silberschatz, Galvin, Gagne]
---
For questions or contributions, please contact the project maintainer.

