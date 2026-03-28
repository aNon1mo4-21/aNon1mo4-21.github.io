# C/C++ Development: Mastery of the Machine

*——where the abstraction ends and the hardware begins* 🔌

C and C++ are the languages of **High-Performance Computing** and **Computer Vision**. My approach is centered on understanding memory layout, pointer arithmetic, and the zero-overhead principle.

## 📝 To-Do List

- [x] **C Fundamentals**: Manual memory management (`malloc`/`free`) and pointer logic.
- [ ] **Modern C++ (17/20)**: RAII, Smart Pointers, and Templates for type-safe generic programming.
- [ ] **Data Structures**: Implementing Linked Lists, Trees, and Hash Maps from scratch in C.
- [ ] **Performance Profiling**: Using `gdb` and `valgrind` to hunt memory leaks and bottlenecks.

------

## 💡 Philosophy: Pure & Efficient

## 1. Manual over Automatic

I prefer direct control over memory. No `<ctype.h>` or high-level abstractions if a simple character comparison or a bitwise operation can do the job faster.

## 2. The Power of Pointers

Understanding `void*`, pointer decay, and function pointers is essential for building flexible system-level software without the bloat of OOP.

## 3. Zero-Cost Abstractions

C++ is used when templates or classes provide a cleaner architecture without sacrificing a single CPU cycle of performance.

------

## 🏗️ Ongoing Projects

## 🌟 3D Vision Kernels

Writing efficient math routines for point cloud processing and transformation matrices.

- **Status**: *Prototyping*

## 📁 Custom Data Structures

A collection of "No-Standard-Library" implementations for embedded-style constraints.

- **Status**: *Continuous*

------

## 🌐 External Resources

## 📖 The Classics

- **The C Programming Language (K&R)**: The bible of C. Concise and perfect.
- **Effective C++ (Scott Meyers)**: Essential for writing robust, modern C++ code.

## 🛠️ Toolchain

- **Compiler**: `gcc` / `g++` (Strictly using `-Wall -Wextra -Werror`).
- **Debugger**: `GDB` (The terminal is my best friend).
- **Build**: `Makefiles` for small projects, `CMake` for everything else.

------

## 🧩 Code Snippets

C

```
/* Manual memory allocation & Pointer arithmetic */
int *arr = (int*)malloc(10 * sizeof(int));
for (int i = 0; i < 10; i++) {
    *(arr + i) = i * i;
}
free(arr);
```

------

<p align="center"> <small>"C makes it easy to shoot yourself in the foot; C++ makes it harder, but when you do, it blows your whole leg off." — Bjarne Stroustrup</small> </p>