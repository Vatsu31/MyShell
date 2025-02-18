# MyShell - Custom Unix Shell

## Overview

**MyShell** is a fully functional Unix-like shell implemented in C as part of a Systems Programming course. This project demonstrates expertise in process management, file I/O, system calls, and memory handling while simulating essential features of popular Unix shells such as Bash and Zsh.

The shell supports executing system commands, handling input/output redirection, implementing piping, and expanding wildcards. It operates in both **interactive** and **batch processing modes**, making it versatile for real-world applications.

## Key Features

- **Command Execution**: Runs standard Unix commands via `execvp()`.
- **Interactive Mode**: Provides a real-time user interface for command execution.
- **Batch Mode**: Reads commands from a file and executes them sequentially.
- **Built-in Commands**:
  - `cd` - Change directory.
  - `exit` - Exit the shell.
  - `pwd` - Print the current working directory.
  - `which` - Locate executables in the system's `PATH`.
- **Redirection (`>`, `<`)**: Supports input and output redirection for handling files.
- **Piping (`|`)**: Allows chaining multiple commands by passing output from one process to another.
- **Wildcard Expansion (`*`, `?`)**: Expands file-matching patterns using `glob()`.
- **Error Handling**: Detects and handles invalid commands, missing arguments, and permission errors.
- **Process Management**: Uses `fork()`, `waitpid()`, and `execvp()` for process execution.
- **Memory Management**: Efficiently allocates and frees memory to prevent leaks.
- **Script Execution**: Runs shell scripts in batch mode to automate tasks.

## Motivation & Learning Outcomes

This project was designed to:

- Gain a **deep understanding of Unix system calls** and process management.
- Implement **low-level memory handling** using `malloc()`, `realloc()`, and `free()`.
- Work with **string parsing** and tokenization to process user commands.
- Apply **concurrency and inter-process communication** techniques.
- Develop robust **error handling** strategies for command execution failures.

By building MyShell, I strengthened my ability to **write efficient C programs**, **debug system-level code**, and **design scalable software architectures**.

## Installation

To compile MyShell, ensure you have `gcc` installed and run:

```bash
make
```
