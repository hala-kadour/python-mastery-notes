---
aliases: [Progress Tracker, Progress, Checklist]
tags: [meta, progress, tracker]
status: active
created: 2026-10-28
updated: 2026-10-28
---

# ✅ Progress Tracker

> Your personal **master checklist** for the whole course. Update this file as you progress. **Only tick a box when you can honestly pass the lesson's Self-Check.**

## How to use this file

- Every time you **finish a lesson**, tick its box here
- If a lesson takes multiple sessions, mark it **🔄 in progress**
- If you get stuck, leave it unchecked and add a note under "Open questions"
- Review the whole file **once a week** to see the big picture

## Legend

- ⬜ Not started
- 🔄 In progress
- ✅ Complete
- ⭐ Core / must-master
- ⚠️ Tricky — revisit

---

## Module 0 — Foundations ✅

- [x] [[0.1 What is Python]] ⭐
- [x] [[0.2 Setup on Windows]] ⭐
- [x] [[0.3 venv and uv]] ⭐
- [x] [[0.4 REPL and __main__]] ⭐

**Module 0 Self-Check:**

- [x] I can explain Python vs CPython
- [x] I know what happens when `python script.py` runs
- [x] `python`, `uv`, `code` all work in PowerShell
- [x] I can create a `uv` project, add a dependency, run a script
- [x] I can delete `.venv/` and rebuild with `uv sync`
- [x] I understand `if __name__ == "__main__":`
- [x] I know the difference between REPL, script, notebook

---

## Module 1 — Core Syntax ⬜

- [ ] [[1.1 Variables and References]] ⭐
- [ ] [[1.2 Numbers]] ⭐
- [ ] [[1.3 Strings]] ⭐
- [ ] [[1.4 Booleans and Truthiness]] ⭐
- [ ] [[1.5 None]]

**Module 1 Self-Check:**

- [ ] I can explain `x = 5` in terms of references, not boxes
- [ ] I understand `is` vs `==`
- [ ] I know that `int` is arbitrary precision, and `float` is not
- [ ] I can use f-strings confidently
- [ ] I can explain truthiness rules
- [ ] I know why `None is None` works but `x is 5` doesn't

---

## Module 2 — Data Structures ⬜

- [ ] [[2.1 Lists]]
- [ ] [[2.2 Tuples]]
- [ ] [[2.3 Dicts]]
- [ ] [[2.4 Sets]]
- [ ] [[2.5 Comprehensions and Unpacking]]

**Module 2 Self-Check:**

- [ ] I can choose between `list`/`tuple`/`set`/`dict` based on the problem
- [ ] I know `dict` is O(1) and insertion-ordered
- [ ] I can write comprehensions fluently
- [ ] I can unpack with `*` and `**`
- [ ] I know why mutable keys break `dict`/`set`

---

## Module 3 — Control Flow & Functions ⬜

- [ ] [[3.1 Conditionals and match]]
- [ ] [[3.2 Loops]]
- [ ] [[3.3 Function Parameters]] ⭐
- [ ] [[3.4 Closures and Lambdas]]
- [ ] [[3.5 Functional Tools]]
- [ ] [[3.6 Iterators vs Generators]] ⚠️

**Module 3 Self-Check:**

- [ ] I can use positional-only, keyword-only, `*args`, `**kwargs`
- [ ] I understand closures and `nonlocal`
- [ ] I know the difference between iterators and iterables
- [ ] I can write a generator from scratch
- [ ] I know when `map`/`filter` are better than comprehensions (rarely)

---

## Module 4 — OOP ⬜

- [ ] [[4.1 Classes Basics]]
- [ ] [[4.2 Dunder Methods]] ⭐
- [ ] [[4.3 Inheritance and MRO]]
- [ ] [[4.4 Properties and Class Methods]]
- [ ] [[4.5 Dataclasses]]
- [ ] [[4.6 ABCs and Protocols]] ⚠️

**Module 4 Self-Check:**

- [ ] I can implement `__repr__`, `__eq__`, `__hash__` correctly
- [ ] I can explain MRO with an example
- [ ] I know when to use `@property` vs a plain attribute
- [ ] I use `@dataclass` for data-holding classes
- [ ] I can define and implement a `Protocol`

---

## Module 5 — Errors & Context ⬜

- [ ] [[5.1 Exceptions]]
- [ ] [[5.2 Custom Exceptions]]
- [ ] [[5.3 Context Managers]] ⭐
- [ ] [[5.4 Logging]]

**Module 5 Self-Check:**

- [ ] I can write `try/except/else/finally` correctly
- [ ] I can define a custom exception hierarchy
- [ ] I can write a context manager from scratch
- [ ] I use `logging` instead of `print` for real programs

---

## Module 6 — Advanced Python ⬜

- [ ] [[6.1 Decorators]] ⭐
- [ ] [[6.2 Generators Deep Dive]]
- [ ] [[6.3 itertools]]
- [ ] [[6.4 Closures nonlocal global]]
- [ ] [[6.5 functools]]

**Module 6 Self-Check:**

- [ ] I can write a decorator from scratch, with `functools.wraps`
- [ ] I can write a generator using `yield from`
- [ ] I use `itertools` in at least 3 places
- [ ] I understand `lru_cache` and `partial`

---

## Module 7 — Modules & Packaging ⬜

- [ ] [[7.1 Import Mechanics]]
- [ ] [[7.2 Packages and Namespaces]]
- [ ] [[7.3 Project Layout]]
- [ ] [[7.4 uv Deep Dive]]

**Module 7 Self-Check:**

- [ ] I can explain how `import` finds modules (sys.path, __init__.py)
- [ ] I can create a namespace package
- [ ] I use the `src/` layout
- [ ] I can build and install my own package

---

## Module 8 — Types & Quality ⬜

- [ ] [[8.1 Type Hints Basics]]
- [ ] [[8.2 Advanced Typing]]
- [ ] [[8.3 mypy ruff pre-commit]]
- [ ] [[8.4 pytest Basics]]

**Module 8 Self-Check:**

- [ ] I annotate all public functions with types
- [ ] I can write generic functions with `TypeVar`
- [ ] I run `mypy --strict` and `ruff check` on my projects
- [ ] I write `pytest` tests with fixtures and parametrization

---

## Module 9 — Concurrency ⬜

- [ ] [[9.1 GIL]] ⭐
- [ ] [[9.2 Threading vs Multiprocessing]]
- [ ] [[9.3 asyncio]] ⚠️
- [ ] [[9.4 concurrent.futures]]

**Module 9 Self-Check:**

- [ ] I can explain the GIL in one sentence
- [ ] I know when to use threads vs processes vs async
- [ ] I can write an `async` function and await it
- [ ] I've used `concurrent.futures.ThreadPoolExecutor` in real code

---

## Module 10 — Files & Data ⬜

- [ ] [[10.1 File IO and pathlib]]
- [ ] [[10.2 json csv pickle]]
- [ ] [[10.3 datetime]]
- [ ] [[10.4 os sys subprocess]]

**Module 10 Self-Check:**

- [ ] I use `pathlib` instead of `os.path`
- [ ] I can read/write JSON, CSV, and binary files
- [ ] I handle timezones with `zoneinfo`
- [ ] I can run subprocesses safely

---

## Module 11 — Applied AI/Data ⬜

- [ ] [[11.1 numpy]]
- [ ] [[11.2 pandas]]
- [ ] [[11.3 torch intro]]
- [ ] [[11.4 ML project deps]]

**Module 11 Self-Check:**

- [ ] I can vectorize a numpy operation
- [ ] I can do basic pandas `groupby`/`merge`
- [ ] I've run a minimal PyTorch model
- [ ] I know how to pin ML dependencies

---

## Module 12 — Shipping ⬜

- [ ] [[12.1 pytest advanced]]
- [ ] [[12.2 Build and Publish]]
- [ ] [[12.3 GitHub Actions]]
- [ ] [[12.4 Debugging and Profiling]]

**Module 12 Self-Check:**

- [ ] I've published a package to PyPI (or TestPyPI)
- [ ] I have a CI pipeline for tests + lint + type check
- [ ] I can use `pdb` and `cProfile` to debug performance

---

## 🏁 Completion Checklist

When all modules are ✅, you've achieved **Python Mastery**. Additional final tasks:

- [ ] Build a **portfolio project** (CLI tool, library, or small service)
- [ ] Publish **one package** to PyPI
- [ ] Contribute a PR to an **open-source Python project**
- [ ] Write a blog post explaining a tricky concept to others
- [ ] Re-read your old notes and see how far you've come

---

## 📝 Open Questions / Notes

Use this section to jot down things you want to revisit:

- _(e.g., "Revisit Module 9 GIL section — I got confused about async + multiprocessing")_
- _(e.g., "Try PyPy on a CPU-bound task")_
- _(e.g., "Look up PEP 703 — free-threaded Python")_

---

## 🔄 Session Log

| Date | Duration | Lesson | Notes |
|------|----------|--------|-------|
| 2026-10-28 | ~4h | 0.1–0.4 | Completed Module 0. Setup works. Ready for Module 1. |
| — | — | — | — |

---

## 🎯 Current Focus

> **Right now:** Move to **Module 1 — Core Syntax**, starting at [[1.1 Variables and References]].

---

## 📊 Progress Stats

- **Modules complete:** 1 / 13
- **Lessons complete:** 4 / 50+
- **Estimated remaining time:** ~95–145 hours

**Update these numbers as you go.** Watching them grow is the best motivation.