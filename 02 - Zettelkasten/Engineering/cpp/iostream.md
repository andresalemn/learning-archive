---
title: iostream
created: 15-01-2026 16:27
domain: cpp
type: header
tags:
  - cpp
  - engineering
source_note: "[[Standard Library]]"
Links to your resource note related:
---
# ⚙️  `iostream` in C++

The `<iostream>` header is used for **input and output** in C++. It works using **streams**.

---
## What Is a Stream?

A **stream** is an object that represents a **flow of bytes** between the program and an external source or destination.

- It can **receive data** (input)
- It can **send data** (output)    
- It hides the details of the actual device (keyboard, screen, file, etc.)

Because of this abstraction:
- Reading from the keyboard
- Writing to the screen
- Reading or writing files

all use **the same syntax**.

The behavior of a stream depends on:

- The **type of stream** (input or output)
- The **operators** used with it (`>>` and `<<`)

---
## Standard Stream Objects

C++ provides four main standard stream objects:

| Stream | Purpose                            |
| ------ | ---------------------------------- |
| `cin`  | Reads input from the keyboard      |
| `cout` | Writes normal output to the screen |
| `cerr` | Writes error messages immediately  |
| `clog` | Writes error or log messages       |
Wide-character versions also exist (`wcin`, `wcout`, `wcerr`, `wclog`).

---

## `cin` — Standard Input Stream

* Used to read input from the keyboard
* Uses the extraction operator `>>`
* Object of type `istream`

```cpp
int x;
std::cin >> x;
```

---

## `cout` — Standard Output Stream

* Used to display normal output
* Uses the insertion operator `<<`
* Output may be stored briefly before appearing on the screen

```cpp
std::cout << "Hello\n";
```

---

## `cerr` — Standard Error Stream (Unbuffered)

* Used for error messages
* Messages appear immediately
* Useful when something goes wrong and feedback must be instant

```cpp
std::cerr << "Error: file not found\n";
```

---

## `clog` — Standard Error Stream (Buffered)

* Used for logging and diagnostic messages
* Output may be delayed slightly
* Useful for messages that do not need to appear immediately

```cpp
std::clog << "Loading configuration...\n";
```

---

## Quick Note on Buffering

* Some streams (like `cout` and `clog`) may **delay output** for efficiency
* `cerr` does **not delay output**, so errors are shown right away
* Output can be forced to appear using `std::endl` or `std::flush`

---

## 🔗 Official & External Resources

*   **Documentation (cppreference) :** [Standard library header iostream](https://en.cppreference.com/w/cpp/header/iostream.html)

---
