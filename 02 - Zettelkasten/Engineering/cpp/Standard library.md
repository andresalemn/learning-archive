---
title: Standard library
created: 22-12-2025 10:09
domain: cpp
type: tool
tags:
  - cpp
  - engineering
source_note: "[[cpp]]"
Links to your resource note related:
---

# ⚙️ Standard library

> The **C++ Standard Library** is a core part of the C++ language specification that provides reusable facilities across a wide range of programming needs in C++. 

---
### **1. Purpose and Overview**

The C++ Standard Library offers a set of **standardized components** that support common programming tasks such as memory management, data structures, algorithms, input/output, concurrency, and more. All features (except `operator new` and `operator delete`) reside in the `std namespace` (or nested `namespaces`).

---
### **2. Major Library Categories**

The library is organized into conceptual groups:

- **Language Support Library**  
	Provides components required by the language itself (e.g., memory allocation, exception handling). 
- **Concepts Library** _(since C++20)_  
	Tools for compile-time type checking and constraints on templates. 
- **Diagnostics Library**  
	Error reporting frameworks, including standard exception classes.     
- **Memory Management Library** _(since C++11)_  
    Smart pointers and allocator support. 
- **Metaprogramming Library**  
    Compile-time utilities (e.g., type traits, integer sequences). 
- **General Utilities Library**  
    Fundamental infrastructure such as tuples and function wrappers. 
- **Containers, Iterators, Algorithms, and Ranges**  
	Standard data structures (vectors, maps, etc.) and algorithms operating on them. Ranges were added in C++20. 
- **Strings Library**  
    Text handling e.g.,  `std::string`, `std::u16string`.
- **Text Processing** _(since C++11)_  
    Regular expressions and formatting utilities (format added in C++20), with encoding support introduced in later standards. 
- **Numerics Library**  
    Numeric algorithms, complex number support, valarrays, and random number generation. 
- **Time Library**  
    Time utilities (`<chrono>`). 
- **Input/Output Library**  
    Streams (`iostream`) and related functionality. 
- **Thread Support Library** _(since C++11)_  
    Thread creation and management, atomics, mutexes. 
- **Execution Support Library** _(since C++26)_  
    High-level support for asynchronous execution. 
---
### **3. Library Contents and Headers**

- The library is **split into headers** that declare and define components. 
- C++ provides both standard C++ headers and C compatibility headers (e.g., `<cstring>`, `<cstdlib>`). 
- Some legacy headers have been **removed in recent standards** (e.g., `<codecvt>`).
---
### **4. Using the Library**

- Components are made available to a program by **including the appropriate headers**.
- Starting with C++20, parts of the library can also be **imported as modules**. 
---
### **5. C Standard Library Integration**

- The C++ Standard Library **incorporates the C Standard Library** (with static type safety), usually by including C headers (like `<cstdio>`).
- These C facilities often appear inside the `std` namespace in C++. 
---
### **6. Requirements on Implementations**

Implementations of the library must conform to rules that ensure correct behaviour and prevent data races (e.g., iterators and threads must not cause undefined behaviour when used as specified). 

---
### **7. Library Hardening**

Some library functions may include **strengthened preconditions** for safety in hardened implementations; if these preconditions are violated, behavior is undefined. 

---
### **8. C++ Standard Library – Cheat Sheet**

| Category               | Purpose                  | Key Headers                                                | Common Types / Utilities                   |
| ---------------------- | ------------------------ | ---------------------------------------------------------- | ------------------------------------------ |
| **Language Support**   | Core language facilities | `<cstddef>`, `<limits>`, `<new>`, `<typeinfo>`             | `size_t`, `nullptr_t`, `bad_alloc`, RTTI   |
| **Concepts (C++20)**   | Template constraints     | `<concepts>`                                               | `same_as`, `integral`, `ranges::range`     |
| **Diagnostics**        | Error handling           | `<exception>`, `<stdexcept>`, `<cassert>`                  | `exception`, `logic_error`, `assert`       |
| **Memory Management**  | Resource safety          | `<memory>`                                                 | `unique_ptr`, `shared_ptr`, `allocator`    |
| **Metaprogramming**    | Compile-time logic       | `<type_traits>`, `<utility>`                               | `is_same`, `enable_if`, `integer_sequence` |
| **General Utilities**  | Core helpers             | `<utility>`, `<tuple>`, `<optional>`, `<variant>`, `<any>` | `pair`, `tuple`, `optional`, `variant`     |
| **Containers**         | Data structures          | `<vector>`, `<map>`, `<unordered_map>`, `<set>`            | `vector`, `map`, `unordered_map`, `set`    |
| **Iterators**          | Container traversal      | `<iterator>`                                               | `iterator_traits`, iterator tags           |
| **Algorithms**         | Data processing          | `<algorithm>`, `<numeric>`                                 | `sort`, `find`, `accumulate`, `transform`  |
| **Ranges (C++20)**     | Lazy algorithms          | `<ranges>`                                                 | `views::filter`, `views::transform`        |
| **Strings**            | Text storage             | `<string>`, `<string_view>`                                | `string`, `wstring`, `string_view`         |
| **Text Processing**    | Regex & formatting       | `<regex>`, `<format>`                                      | `regex`, `smatch`, `format`                |
| **Numerics**           | Math utilities           | `<cmath>`, `<random>`, `<complex>`                         | `complex`, `mt19937`, distributions        |
| **Time**               | Clocks & durations       | `<chrono>`                                                 | `time_point`, `duration`, `steady_clock`   |
| **Input / Output**     | Streams                  | `<iostream>`, `<fstream>`, `<sstream>`                     | `cin`, `cout`, `ifstream`, `ostringstream` |
| **Filesystem (C++17)** | File operations          | `<filesystem>`                                             | `path`, `directory_iterator`               |
| **Threading (C++11)**  | Concurrency              | `<thread>`, `<mutex>`, `<atomic>`                          | `thread`, `mutex`, `atomic`                |
| **Async & Futures**    | Task execution           | `<future>`                                                 | `async`, `future`, `promise`               |
| **Execution (C++26)**  | Execution policies       | `<execution>`                                              | `execution::par`, `execution::seq`         |
| **C Compatibility**    | C standard library       | `<cstdio>`, `<cstdlib>`, `<cstring>`                       | `printf`, `malloc`, `memcpy`               |