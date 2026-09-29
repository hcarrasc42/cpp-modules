These modules were built as part of the 42 cursus by hcarrasc42.

# CPP Modules

> _Learning C++ the way it was meant to be learned: one concept at a time._

The C++ track of the 42 cursus: nine progressive modules (CPP00–CPP09) that build
up object-oriented and modern C++ fundamentals from the ground up, deliberately
constrained to the **C++98** standard so the language's mechanics are learned
without leaning on newer conveniences.

![Language](https://img.shields.io/badge/language-C%2B%2B98-00599C?style=flat-square)
![Topics](https://img.shields.io/badge/topics-OOP%20%C2%B7%20templates%20%C2%B7%20STL-green?style=flat-square)
![Norm](https://img.shields.io/badge/norm-42-black?style=flat-square)

## 📖 About

Each module is a self-contained set of exercises focused on one theme, compiled
with `-Wall -Wextra -Werror -std=c++98`. The sequence moves from the very basics
of classes up to the STL, with the "orthodox canonical form" (default/copy
constructors, assignment operator, destructor) reinforced throughout.

| Module | Theme | Highlights |
|--------|-------|-----------|
| **CPP00** | Basics | namespaces, classes, member functions, I/O streams, a small phonebook |
| **CPP01** | Memory & references | `new`/`delete`, references vs. pointers, pointers to members |
| **CPP02** | Ad-hoc polymorphism | operator overloading, orthodox canonical form, a fixed-point number class |
| **CPP03** | Inheritance | base/derived classes, the ClapTrap hierarchy |
| **CPP04** | Subtype polymorphism | virtual functions, abstract classes, interfaces, deep vs. shallow copy |
| **CPP05** | Exceptions | `try`/`catch`, custom exception classes, a bureaucrat simulation |
| **CPP06** | Casting | `static_cast`, `dynamic_cast`, `reinterpret_cast`, `const_cast` |
| **CPP07** | Templates | function and class templates |
| **CPP08** | Templated containers | STL containers, iterators, and algorithms |
| **CPP09** | STL | Bitcoin exchange, RPN calculator, Ford–Johnson (merge-insertion) sort |

## 🛠 Technologies

| Component | Detail |
|-----------|--------|
| Language | C++98 (`-Wall -Wextra -Werror -std=c++98`) |
| Paradigm | object-oriented programming, generic programming, RAII |
| Standard library | the C++98 STL (from CPP08 onward) |
| Build system | GNU Make, one `Makefile` per exercise |

## 💡 Concepts covered

- **Classes and the orthodox canonical form** — the four member functions every
  well-behaved C++98 class provides.
- **Inheritance and polymorphism**, including abstract classes and interfaces.
- **Operator overloading** and value semantics (e.g. a fixed-point type).
- **Exceptions** and custom exception hierarchies.
- **The four C++ casts** and when each is appropriate.
- **Templates** — writing generic functions and containers.
- **The STL** — containers, iterators, and algorithms, plus a non-trivial
  sorting algorithm (Ford–Johnson) in CPP09.

## 🚀 How to Run

Each exercise builds on its own:

```sh
cd cpp02/ex00 && make
./<binary>
```

## 📂 Project Structure

```
cpp-modules/
├── cpp00/  ex00 … exNN     # each exercise: sources + its own Makefile
├── cpp01/
├── …
└── cpp09/  ex00 (Bitcoin) · ex01 (RPN) · ex02 (PmergeMe)
```

## 🎯 What This Project Demonstrates

- A **ground-up command of C++** fundamentals under a strict standard.
- **Object-oriented design**: encapsulation, inheritance, polymorphism.
- **Generic programming** with templates and the STL.
- **Disciplined resource management** (RAII, canonical form) and clean,
  Norm-compliant code.
