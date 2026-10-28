---
aliases: [Glossary, Terms, Dictionary]
tags: [meta, glossary, reference]
status: active
created: 2026-10-28
updated: 2026-10-28
---

# 📖 Glossary

> A **living dictionary** of every term used across the course. New terms get added as modules progress. If you encounter a term and can't find it here, that's a signal to add it — don't just move on.

## How to use this glossary

- **Skim** it before starting Module 1 — you don't need to memorize it
- **Search** with `Ctrl+F` when you hit an unfamiliar term
- **Contribute** new terms as you learn them (each term should be 1–2 sentences max, with a link to the lesson where it's introduced)

## A–C

### Bytecode
The intermediate representation that CPython compiles your `.py` source into before executing it. Stored in `__pycache__/` as `.pyc` files. Not machine code — the PVM interprets it. → [[0.1 What is Python]]

### CPython
The **reference implementation** of Python, written in C. When people say "Python" they almost always mean CPython. Alternative implementations: PyPy, Jython, IronPython, MicroPython. → [[0.1 What is Python]]

### Closure
A function that captures variables from its enclosing scope, remembering them even after the outer function returns. → [[3.4 Closures and Lambdas]]

### Comprehension
A concise syntax for building lists, dicts, or sets from iterables: `[x*2 for x in range(5)]`. Faster and more Pythonic than a loop. → [[2.5 Comprehensions and Unpacking]]

### Context manager
An object usable with `with`, defining `__enter__` and `__exit__` methods. Ensures cleanup (closing files, releasing locks) runs even if an exception occurs. → [[5.3 Context Managers]]

### Coroutine
A function defined with `async def` that can be paused and resumed. The building block of `asyncio`. → [[9.3 asyncio]]

## D–F

### Decorator
A function that takes another function and returns a modified version. Used with `@decorator` syntax. → [[6.1 Decorators]]

### Dict (`dict`)
Python's **hash map** — O(1) average lookup, insertion-order-preserving (since Python 3.7). → [[2.3 Dicts]]

### Duck typing
"If it walks like a duck and quacks like a duck, it's a duck." Python doesn't check *types*, it checks *behavior* — anything with the right methods works. → [[4.6 ABCs and Protocols]]

### Dunder
**D**ouble **under**score methods like `__init__`, `__repr__`, `__eq__`. Also called "magic methods." They power operators and built-in functions. → [[4.2 Dunder Methods]]

### f-string
Formatted string literal: `f"Hello, {name}!"`. The modern, fastest way to format strings (since Python 3.6). → [[1.3 Strings]]

## G–I

### Generator
A function using `yield` that produces values lazily. Memory-efficient for large/infinite sequences. → [[3.6 Iterators vs Generators]]

### GIL (Global Interpreter Lock)
CPython's mechanism that allows only **one thread to execute Python bytecode at a time**. Makes threading useful only for I/O-bound tasks in CPython. → [[9.1 GIL]]

### Immutable
An object whose value can't change after creation. Examples: `int`, `str`, `tuple`, `frozenset`. → [[1.1 Variables and References]]

### Import
Loading a module into the current namespace with `import x` or `from x import y`. Has side effects (the module's top-level code runs). → [[7.1 Import Mechanics]]

### Interpreter
A program that executes source code directly, without a separate compile step. **Python is *not* purely interpreted** — CPython compiles to bytecode first. → [[0.1 What is Python]]

### Iterable
An object that can be iterated with `for` (has `__iter__`). Lists, dicts, strings, files, generators are all iterable. → [[3.6 Iterators vs Generators]]

### Iterator
An object with `__next__` that yields items one at a time. Returned by `iter(x)`. → [[3.6 Iterators vs Generators]]

## J–L

### JIT (Just-In-Time) compiler
A compiler that translates bytecode to native machine code at runtime, for hot code paths. PyPy uses a JIT; CPython does not (as of 3.13). → [[0.1 What is Python]]

### Lambda
An anonymous one-line function: `lambda x: x * 2`. Useful for `sorted(key=...)` and similar callbacks. → [[3.4 Closures and Lambdas]]

### Lock file
A file (e.g., `uv.lock`) recording exact versions and hashes of every dependency, ensuring reproducible builds. **Commit it to git.** → [[0.3 venv and uv]]

## M–O

### MOC (Map of Content)
An Obsidian convention — an index page that links to related notes. Every module has a `_MOC <Module>.md` file. → [[How to Use These Notes]]

### Module
A single `.py` file (or package directory) that can be imported. Its `__name__` is the filename without `.py` (unless run directly, then `"__main__"`). → [[0.4 REPL and __main__]]

### MRO (Method Resolution Order)
The order Python searches base classes when looking up a method. Uses the **C3 linearization** algorithm. → [[4.3 Inheritance and MRO]]

### Mutable
An object whose value can change after creation. Examples: `list`, `dict`, `set`, `bytearray`. → [[1.1 Variables and References]]

### `__main__`
The `__name__` value given to the **entry script**. Guarded by `if __name__ == "__main__":`. → [[0.4 REPL and __main__]]

### `__name__`
A global variable holding the module's name. `"__main__"` if the module is the entry point, otherwise the module's filename. → [[0.4 REPL and __main__]]

### Namespace
A mapping from names to objects. Modules, classes, and function calls each have their own namespace. → [[7.1 Import Mechanics]]

### None
The **only** null value in Python. It's a singleton of type `NoneType`. Not the same as `0`, `""`, or `False`. → [[1.5 None]]

## P–R

### Package
A directory of Python modules with an `__init__.py` (or a namespace package without it). → [[7.2 Packages and Namespaces]]

### PATH
The environment variable listing directories the shell searches for executables. If Python isn't on PATH, `python` won't work. → [[0.2 Setup on Windows]]

### PEP
**Python Enhancement Proposal** — a document proposing a change to Python. PEP 8 = style guide. PEP 20 = The Zen of Python. PEP 621 = `pyproject.toml`. → [[Glossary]]

### pip
Python's traditional package installer. **For new projects, use `uv` instead** — it's much faster and manages lock files. → [[0.3 venv and uv]]

### `pip install`
The traditional install command. In `uv` projects, use `uv add` instead — it updates `pyproject.toml` and `uv.lock`. → [[0.3 venv and uv]]

### PVM (Python Virtual Machine)
The part of CPython that executes bytecode instruction by instruction. → [[0.1 What is Python]]

### `pyproject.toml`
The modern project configuration file (PEP 621). Contains project metadata, dependencies, and tool configs (ruff, pytest, mypy). → [[0.3 venv and uv]]

### PyPI
The **Python Package Index** — the public registry where most Python packages live (`pypi.org`). → [[12.2 Build and Publish]]

### PyPy
An alternative Python implementation with a **JIT compiler**. Often 4–10x faster than CPython for pure-Python code. → [[0.1 What is Python]]

### Reference counting
CPython's primary memory management strategy — each object tracks how many references point to it; when the count hits zero, the object is freed. → [[1.1 Variables and References]]

### REPL
**R**ead–**E**val–**P**rint **L**oop — the interactive Python shell. → [[0.4 REPL and __main__]]

## S–U

### `site-packages`
The directory inside a virtual environment where installed packages live. → [[0.3 venv and uv]]

### Slot
A class-level optimization via `__slots__` that replaces `__dict__` with a fixed set of attributes. Saves memory. → [[4.5 Dataclasses]]

### `str` vs `bytes`
`str` is Unicode text; `bytes` is raw binary. They're **not** interchangeable. Convert with `.encode()` and `.decode()`. → [[1.3 Strings]]

### `sys.path`
The list of directories Python searches when you `import` something. → [[7.1 Import Mechanics]]

### `typing`
The standard library module for type hints (`list[int]`, `Optional[str]`, `Protocol`, etc.). → [[8.1 Type Hints Basics]]

### `uv`
A Rust-based Python toolchain by Astral. Replaces `pip`, `venv`, `pip-tools`, `pyenv`, and `pipx`. 10–100x faster than `pip`. → [[0.3 venv and uv]]

### `uv run`
Execute a command inside the project's virtual environment, without manual activation. → [[0.3 venv and uv]]

### `uv sync`
Install exactly what's locked in `uv.lock`, recreating `.venv/` from scratch if needed. → [[0.3 venv and uv]]

### `uv.lock`
The lock file — exact versions and hashes of all dependencies. **Commit it to git.** → [[0.3 venv and uv]]

## V–Z

### venv
Python's built-in virtual environment module. **Use `uv venv` for modern projects** — same concept, much faster. → [[0.3 venv and uv]]

### Virtual environment
An isolated Python environment with its own `site-packages`. Prevents dependency conflicts between projects. → [[0.3 venv and uv]]

### The Zen of Python (PEP 20)
19 aphorisms that capture Python's design philosophy. Run `import this` in a REPL to see them. → [[0.1 What is Python]]

## To Add

Terms we'll cover in future modules:

- `asyncio` → [[9.3 asyncio]]
- `@dataclass` → [[4.5 Dataclasses]]
- `functools` → [[6.5 functools]]
- `itertools` → [[6.3 itertools]]
- `pathlib` → [[10.1 File IO and pathlib]]
- `pytest` → [[8.4 pytest Basics]]
- `Protocol` → [[4.6 ABCs and Protocols]]
- `ruff` → [[8.3 mypy ruff pre-commit]]
- `typing.Protocol` → [[4.6 ABCs and Protocols]]
- `yield` → [[3.6 Iterators vs Generators]]

## Contributing new terms

When you add a term:

1. Group alphabetically (A–C, D–F, etc.)
2. One or two sentences max
3. Include a `→ [[link]]` to the lesson where it's taught
4. If it's not taught yet, put it under "To Add"

**The glossary is not a nice-to-have.** It's the memory of the course. Every term you add is a term you won't forget.