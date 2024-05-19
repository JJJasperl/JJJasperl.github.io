---
layout: page
title: Pintos Operating System
description: Comprehensive project extending the Pintos operating system
img: assets/img/pintos.jpg
importance: 1
category: School Projects
related_publications: false
---

The Pintos Operating System project is a comprehensive series of tasks designed to extend and enhance the functionality of the Pintos operating system. Written entirely in `C`, The project is divided into three main components: User Programs, Threads, and File Systems. Each component focuses on different aspects of operating system development, including process management, thread scheduling, and file system operations.

### Project Details

### 1. User Programs
This component involves implementing core functionalities for user programs, such as argument passing, system calls, and floating point operations.

- **Argument Passing**: Implemented argument passing in the process_execute function to correctly handle argc and argv for user programs.
- **Process Control Syscalls**: Added support for syscalls such as `practice`, `halt`, `exec`, and `wait` to manage processes and handle user inputs.
- **File Operation Syscalls**: Implemented file operation syscalls including `create`, `remove`, `open`, `filesize`, `read`, `write`, `seek`, `tell`, and `close`.
- **Floating Point Operations**: Enabled support for floating point operations in user programs and the kernel, including the `compute_e` syscall for computing the value of e using the Taylor series.

### 2. Threads
This component focuses on enhancing the threading system of Pintos by supporting multithreaded user programs, an efficient alarm clock, and a strict priority scheduler.

- **Efficient Alarm Clock**: Reimplemented `timer_sleep` to avoid busy waiting and improve efficiency.
- **Strict Priority Scheduler**: Modified the scheduler to respect thread priority values and implemented priority donation to handle priority inversion.
- **User Threads**: Implemented a simplified version of the pthread library to allow user programs to create, join, and manage threads. Added support for user-level synchronization with locks and semaphores.

### 3. File Systems
This component involves enhancing the file system by adding a buffer cache, support for extending files, and enabling hierarchical directory structures.

- **Buffer Cache**: Implemented a buffer cache to improve performance of reads and writes by caching disk blocks and using a clock replacement algorithm.
- **Extensible Files**: Modified the file system to support file growth beyond the initial size, using an indexed inode structure with direct, indirect, and doubly-indirect pointers.
- **Subdirectories**: Added support for hierarchical directory trees, including system calls for changing directories (`chdir`), creating directories (`mkdir`), reading directory entries (`readdir`), and identifying directories (`isdir`).

### Conclusion
The Pintos Operating System project provided a comprehensive experience in operating system development, covering essential topics such as process management, thread scheduling, and file system operations. The implementation of these features involved significant modifications to the existing Pintos codebase and required a deep understanding of operating system concepts and design principles.

### Address
For more details on this project, visit: CS162 Pintos Project [1](https://cs162.org/static/proj/proj-userprog/), [2](https://cs162.org/static/proj/proj-threads/), and [3](https://cs162.org/static/proj/proj-filesys/)
