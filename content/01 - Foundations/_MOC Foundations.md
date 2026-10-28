---
aliases:
  - Foundations MOC
  - Module 0 Index
  - Foundations Index
tags:
  - moc
  - module-0
  - foundations
  - index
module: 0
status: active
created: 2026-10-28
---

# 🏗️ Module 0 — Foundations (MOC)

> **This is the index page for Module 0.** Everything about setting up Python and understanding the language's architecture lives here.

## 🎯 Module Goal

Before writing any real code, you must **understand the machine you're driving** and have a **clean, reproducible environment**. This module does both.

By the end of Module 0 you will:

- Know what Python is (and what CPython is)
- Have a working Python 3.12+ installation on Windows
- Have `uv`, VS Code, and all tooling configured
- Understand virtual environments and the modern project workflow
- Know the `if __name__ == "__main__":` idiom

## 📚 Lessons

| # | Lesson | Status | Difficulty |
|---|--------|--------|------------|
| 0.1 | [[0.1 What is Python]] | ✅ done | beginner |
| 0.2 | [[0.2 Setup on Windows]] | ✅ done | beginner |
| 0.3 | [[0.3 venv and uv]] | ✅ done | beginner |
| 0.4 | [[0.4 REPL and __main__]] | ⬜ not started | beginner |

## 🧠 Core Concepts Introduced in This Module

These are the ideas you must **master before moving to Module 1**. If any is fuzzy, revisit the lesson.

- [[CPython]] vs other [[Python Implementations]]
- [[Bytecode]] and the [[PVM]]
- [[GIL]] (first look — deep dive in [[9.1 GIL]])
- [[The Zen of Python]] (PEP 20)
- [[PATH]] environment variable
- [[REPL]] (Read-Eval-Print Loop)
- [[Virtual Environment]] (`venv`)
- [[uv]] — modern Python toolchain
- [[pyproject.toml]] (PEP 621)
- [[uv.lock]] and lock files
- [[__main__]] — the module entry point idiom
- [[__name__]] special variable

## 🔧 Tools Installed in This Module

| Tool | Version target | Purpose |
|------|---------------|---------|
| **Python** | 3.12+ | The language runtime |
| **uv** | 0.5+ | Package/project/version manager |
| **VS Code** | latest | Editor |
| **Pylance** | latest | Type checker / IntelliSense |
| **Jupyter** | latest | Notebooks (inside VS Code) |
| **Ruff** | latest | Linter + formatter (used from Module 8) |
| **PowerShell** | built-in | Shell (Windows) |

## ✅ Module 0 Self-Check (all should be ticked before Module 1)

- [ ] I can explain what Python is vs CPython
- [ ] I know what happens when I type `python script.py` (source → bytecode → PVM)
- [ ] `python --version`, `uv --version`, `code --version` all work in PowerShell
- [ ] I can create a `uv` project with `uv init`
- [ ] I can add a dependency with `uv add`
- [ ] I can run a script with `uv run python script.py`
- [ ] I can delete `.venv/` and rebuild it with `uv sync`
- [ ] I understand `if __name__ == "__main__":`
- [ ] I know the difference between REPL, script, and notebook workflows
- [ ] I know what a virtual environment is and why it exists

## 🧪 Module 0 Practice Projects

Small projects to solidify the setup skills:

- **Hello, uv** — a `uv init` project that prints environment info
- **Reproducibility drill** — delete `.venv/`, `uv sync`, verify it works
- **Notebook tour** — a Jupyter notebook with a markdown cell, code cell, and output cell
- **Manual venv comparison** — create one with `python -m venv` and compare speed to `uv`

## ⚠️ Module 0 Gotchas Recap

The pitfalls you should **never** fall into again:

1. Microsoft Store Python ❌
2. Forgetting "Add to PATH" during install ❌
3. Typing `python3` on Windows ❌
4. Committing `.venv/` to git ❌
5. Forgetting to commit `uv.lock` ❌
6. Using `pip install` instead of `uv add` in a `uv` project ❌
7. Manually activating `.venv/` when `uv run` exists ❌
8. Running `python` instead of `uv run python` in a project ❌
9. Editing `uv.lock` by hand ❌
10. Running a script from the wrong directory ❌

## 🔗 What Comes Next

- **Module 1 — Core Syntax** → [[_MOC Core Syntax]] (once written)
  - Variables, references, `id()`, `is` vs `==`
  - Numbers (`int`, `float`, `Decimal`, `complex`)
  - Strings, f-strings, encoding
  - Booleans and truthiness
  - `None`

## 📝 Notes on the Module

- **Pace:** 4 lessons, one per session. Deep pace — no rushing.
- **Estimated time to complete:** 3–5 hours including all practice.
- **Prerequisites:** none — this is the starting point.
- **Language:** English only (GitHub public repo).
- **Platform:** Windows-specific commands throughout, but concepts are cross-platform.

