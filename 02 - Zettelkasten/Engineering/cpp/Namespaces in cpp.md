---
title: Namespaces in cpp
created: 16-01-2026 11:57
domain: cpp
type: tool
tags:
  - cpp
  - engineering
source_note: "[[Standard Library]]"
Links to your resource note related:
---
# ⚙️ Namespaces in C++

> In C++, a **namespace** is a way to group related names (like variables, functions, and classes) under a **named scope**. This helps **avoid naming conflicts** when different parts of a program or different libraries use the same names. 

---
### Why Namespaces Are Useful?

Without **namespaces**, every name in a program must be unique. In small programs that’s easy, but in larger ones — or when using libraries — two functions or variables might accidentally have the same name. A namespace prevents these conflicts by keeping names separate. 

---
## Basic Namespace Syntax

You create a namespace using the `namespace` keyword and a name:

```cpp
namespace mySpace {
    int value;
    void greet() { /*…*/ }
}
```

To access members inside a namespace, use the **scope resolution operator `::`**:

```cpp
mySpace::greet();
```

This tells the compiler exactly which `greet` you mean. 

---
## The Global Namespace

Names that are **not** inside any namespace belong to the **global namespace**.
You can explicitly refer to the global namespace with `::` at the start:

```cpp
::someGlobalFunction();
```

This makes it clear you are referring to a name outside all namespaces. 

---
## Using Namespaces

Instead of always writing the namespace name, you can bring it into the current scope using a **using directive**:

```cpp
using namespace mySpace;
greet();  // no need to write mySpace::greet()
```

This makes names from the namespace available without the prefix.
However, be careful: if two namespaces contain the same name, this can lead to confusion. 

---
## Namespace Alias

If a namespace name is long, you can make a **short alias**:

```cpp
namespace ms = mySpace;
ms::greet();  // shorter than mySpace::greet()
```

This improves readability. 

---
## Nested and Extended Namespaces

* **Nested namespace**: a namespace inside another namespace.

  ```cpp
  namespace outer {
      namespace inner {
          void func();
      }
  }
  ```

  You access nested names with `outer::inner::func()`. 

* **Namespace extension**: you can define parts of the same namespace in multiple places.

  ```cpp
  namespace nm { void a(); }
  namespace nm { void b(); }
  // Both a() and b() are in nm
  ```

  This allows adding to a namespace over time. 

---
## Summary

* A **namespace** groups names to avoid conflicts. 
* Use `namespace name { … }` to define it. 
* Use `name::identifier` to access members. 
* A **using directive** can make names easier to use. 
* Namespaces help keep code organized and clear. 

---
## 🔗 Official & External Resources

*   **Documentation (cppreference):** [Namespaces](https://en.cppreference.com/w/cpp/language/namespace.html)
* **Documentation (geeks for geeks):** [Namespace in C++](https://www.geeksforgeeks.org/cpp/namespace-in-c/)

---
