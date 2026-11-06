---
aliases: [Python Roadmap, Master Plan, Course Roadmap]
tags: [meta, roadmap, index]
status: active
created: 2026-10-28
updated: 2026-10-28
---

# 🗺️ Python Mastery Roadmap

> From **absolute zero** to **advanced Python engineer**. A structured, hands-on journey with 13 modules, 50+ lessons, and hundreds of exercises.

## Who this is for

- Complete beginners who have **never written Python**
- Self-taught developers who want to **fill the gaps** and understand *why* Python behaves as it does
- Anyone preparing for **AI/ML/Data** work who needs a solid Python foundation

## How to use this roadmap

1. Read the **Module Overview** below to understand the arc of the course
2. Open each **`_MOC <Module>.md`** file to see the lessons inside
3. Follow modules **in order** — each builds on the previous
4. Complete the **Self-Check** before moving to the next lesson
5. Track progress in [[Progress Tracker]]

## Module Overview

| # | Module | Focus | Status |
|---|--------|-------|--------|
| 0 | **Foundations** | Setup, tooling, execution model | ✅ Complete |
| 1 | **Core Syntax** | Variables, types, strings, truthiness | ⬜ Not started |
| 2 | **Data Structures** | list, dict, set, tuple, comprehensions | ⬜ Not started |
| 3 | **Control Flow & Functions** | Conditionals, loops, functions, generators | ⬜ Not started |
| 4 | **OOP** | Classes, dunder methods, dataclasses, protocols | ⬜ Not started |
| 5 | **Errors & Context** | Exceptions, `with`, logging | ⬜ Not started |
| 6 | **Advanced Python** | Decorators, iterators, itertools, functools | ⬜ Not started |
| 7 | **Modules & Packaging** | Imports, project layout, uv deep dive | ⬜ Not started |
| 8 | **Types & Quality** | Type hints, mypy, ruff, pytest | ⬜ Not started |
| 9 | **Concurrency** | GIL, threading, multiprocessing, asyncio | ⬜ Not started |
| 10 | **Files & Data** | I/O, pathlib, json, datetime | ⬜ Not started |
| 11 | **Applied AI/Data** | numpy, pandas, torch intro | ⬜ Not started |
| 12 | **Shipping** | Testing, packaging, CI/CD, debugging | ⬜ Not started |

## Module Details

### Module 0 — Foundations ✅
- Setup Python + uv + VS Code
- Understand CPython, bytecode, PVM
- Virtual environments
- The `__main__` idiom

### Module 1 — Core Syntax
- Variables and references (`id()`, `is` vs `==`)
- Numbers: `int`, `float`, `Decimal`, `complex`
- Strings, f-strings, encoding
- Booleans and truthiness
- `None`

### Module 2 — Data Structures
- `list` — dynamic array internals
- `tuple` — immutability, unpacking
- `dict` — hash tables, insertion order
- `set` / `frozenset` — hashing
- Comprehensions and unpacking tricks

### Module 3 — Control Flow & Functions
- `if`/`elif`/`else`, `match` statement
- `for`/`while`, `enumerate`, `zip`
- Functions: all parameter types
- Closures, lambdas, functional tools
- Iterators vs generators

### Module 4 — OOP
- Classes, `__init__`, `__dict__`
- Dunder methods
- Inheritance, MRO, `super()`
- `@property`, `@staticmethod`, `@classmethod`
- `@dataclass`
- ABCs and Protocols

### Module 5 — Errors & Context
- `try`/`except`/`else`/`finally`
- Custom exceptions
- Context managers
- Logging vs print

### Module 6 — Advanced Python
- Decorators (from scratch)
- Generators deep dive
- `itertools`
- Closures and `nonlocal`/`global`
- `functools`

### Module 7 — Modules & Packaging
- Import mechanics
- Packages and namespaces
- Project layout
- `uv` deep dive

### Module 8 — Types & Quality
- Type hints basics
- Advanced typing (`TypeVar`, `Protocol`, `Literal`, `TypedDict`)
- `mypy`, `ruff`, `pre-commit`
- `pytest` basics

### Module 9 — Concurrency
- The GIL
- `threading` vs `multiprocessing`
- `asyncio`
- `concurrent.futures`

### Module 10 — Files & Data
- File I/O, `pathlib`
- `json`, `csv`, `pickle`
- `datetime`, `zoneinfo`
- `os`, `sys`, `subprocess`

### Module 11 — Applied AI/Data
- `numpy` fundamentals
- `pandas` essentials
- `torch` intro
- ML project dependencies

### Module 12 — Shipping
- `pytest` advanced
- Building and publishing
- GitHub Actions
- Debugging and profiling

## Legend

| Symbol | Meaning |
|--------|---------|
| ✅ | Complete |
| 🔄 | In progress |
| ⬜ | Not started |
| ⭐ | High-priority / core concept |
| ⚠️ | Common trap / gotcha |

## Related

- [[How to Use These Notes]] — reader guide
- [[Glossary]] — living dictionary
- [[Progress Tracker]] — your progress
- [[_MOC Foundations]] — Module 0 index