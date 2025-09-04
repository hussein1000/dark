# PyOS - C Kernel with Python Applications

## Overview

PyOS is an experimental operating system with a C-based kernel and a Python runtime for applications. The OS demonstrates how low-level system functionality (process management, memory, file system, and I/O) can be implemented in C, while allowing developers to write applications in Python.

PyOS provides a secure sandbox for Python apps, offering access to OS services via a Python API while keeping the core system efficient and lightweight.

## Features

- C-based kernel: Handles process scheduling, memory management, and device drivers.

- Python runtime: Executes Python applications directly on the OS.

- Virtual file system: Accessible to both C kernel modules and Python applications.

- Networking support: TCP/IP stack implemented in C, exposed to Python apps via API.

- Graphical shell: Optional GUI written in Python using a lightweight toolkit.

- Modular architecture: Easily extendable kernel modules and Python app ecosystem.


## System Requirements

- Minimum 2 GB RAM

- 1 GB free disk space

- GCC toolchain and Python 3.11+ for building apps

- Virtualization software recommended (QEMU, VirtualBox)


## Installation Instructions

- Clone the Repository

- Build the Kernel. This compiles the kernel and produces a bootable image (PyOS.iso).

- Launch in Virtual Machine:

-- Create a new VM in VirtualBox or QEMU.

2- Attach PyOS.iso as the boot medium.

3- Boot into the OS to access the Python shell.


## Running Python Applications

- Place Python scripts in any desired directory.

- From the PyOS shell:
run_app example_app.py

- Python apps have access to OS services via the **pycore** module.

## Limitations

- Experimental OS: not suitable for production.

- Limited hardware support: works best in virtualized environments.

- Python runtime is sandboxed and cannot access low-level kernel memory directly.

## Notes

PyOS is an educational and experimental OS. It demonstrates how a C kernel and a high-level language runtime can coexist, allowing rapid application development while keeping the core OS efficient.

