<p align="center">
  <img src="https://hrcdn.net/fcore/assets/brand/logo-new-white-green-a5cb16e0ae.svg" alt="HackerRank" height="40" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/language-Python-blue" alt="Language" />
  <img src="https://img.shields.io/badge/focus-Embedded%20QA-orange" alt="Focus" />
  <img src="https://img.shields.io/badge/status-active-brightgreen" alt="Status" />
  <img src="https://img.shields.io/badge/learning-DataCamp-03EF62" alt="DataCamp" />
</p>

# Embedded-QA-Python-Practice

**Python problem-solving practice, selected for an Embedded QA and validation path.**

The goal is not to solve as many HackerRank problems as possible. The goal is to build enough Python problem-solving skill to make later work with test automation, serial communication, log parsing, and validation easier.

This is a **practice repo, not a tooling or project repo**.

The firmware/embedded-C side lives in [Embedded-C-Practice](https://github.com/mohamedSamehMS/Embedded-C-Practice).

## Goal

Build enough Python fluency that writing a `pyserial`-based validation script is practical and does not require constant syntax lookup.

The repository focuses first on HackerRank problem solving. Practical QA tools such as `pytest` and `pyserial` can be studied separately later.

## Learning approach

Two tracks run in parallel:

- **DataCamp** for structured Python learning
- **HackerRank / LeetCode** for problem-solving practice

Basic Python data types are not included because the fundamentals are already known.

---

# HackerRank Python

All 17 HackerRank Python subdomains were reviewed.

## Core problem set

These are the problems worth prioritizing for the current Embedded QA goal.

| Subdomain | Why it matters for Embedded QA | Core problems |
|---|---|---:|
| Errors and Exceptions | Serial failures, timeouts, retry logic, failure handling | 2 |
| Date and Time | Measuring durations, timestamps, timeout checks | 2 |
| Collections | Buffers, counters, result storage, ordered data | 6 |
| Regex and Parsing | Parsing UART messages, logs, and structured text | 7 |
| Closures and Decorators | Retry/timeout wrapper concepts | 2 |
| XML | Reading structured test-report data | 2 |
| Strings | Splitting, searching, validating, and formatting text | 8 |
| Sets | Comparing expected and actual values/configuration | 8 |
| Itertools | Test-matrix generation and combinations | 5 |
| Built-Ins | `zip`, `any`, `all`, sorting, and useful built-ins | 4 |
| Python Functionals | `map`, `lambda`, and `reduce` | 2 |

**Core total: 48 problems**

### Small additional areas

Two HackerRank subdomains are kept as small areas instead of full problem sets:

| Subdomain | Purpose |
|---|---|
| Classes | Useful for future test-framework and device abstraction design |
| Debugging | Useful for fixing Python test and automation code |

These are intentionally kept small because the available HackerRank problems do not strongly match the current Embedded QA goal.

## Lower priority problems

The other problems were **not deleted**. They were moved to [`hackerrank/optional/`](hackerrank/optional/).

This keeps the repository focused without losing the original practice material.

The optional area contains problems that are useful for general Python practice but are less important for the current goal.

---

# HackerRank domain decisions

## Keep as core

- Strings
- Sets
- Itertools
- Collections
- Date and Time
- Errors and Exceptions
- Built-Ins
- Python Functionals
- Regex and Parsing
- XML
- Closures and Decorators

## Keep as small areas

- Classes
- Debugging

## Not needed for the current plan

- Basic Data Types — already known
- Math — not a current Embedded QA priority
- Numpy — useful later for sensor/ADC/signal-data work, but not needed now

---

# Link verification note

Problem links are kept as verified links where available. A `TODO` means the link still needs to be added from the official HackerRank problem page.

Do not guess a URL just to remove a `TODO`.

---

# Progress — HackerRank Python

Update each problem as you work through it:

- ⬜ Not started
- 🟨 In progress
- ✅ Solved

Each problem file uses this format:

```python
"""
Problem   : <name>
Subdomain : HackerRank Python > <subdomain>
Link      : <url>

Why this one: <embedded QA relevance>

Notes:
- Approach:
- Concepts practiced:
- Anything that tripped me up:
"""
```

The most important field is **Why this one**. It keeps the problem connected to the Embedded QA goal.

---

# LeetCode

Not started yet.

See [leetcode/README.md](leetcode/README.md).

LeetCode remains secondary to the HackerRank Python practice in this repository.

---

# Repository layout

```text
hackerrank/
  errors-and-exceptions/   (2 core)
  date-and-time/           (2 core)
  collections/             (6 core)
  regex-and-parsing/       (7 core)
  closures-and-decorators/ (2 core)
  xml/                     (2 core)
  strings/                 (8 core)
  sets/                    (8 core)
  itertools/               (5 core)
  built-ins/               (4 core)
  python-functionals/      (2 core)
  classes/                 (small area)
  debugging/               (small area)
  optional/                (lower-priority original problems)

leetcode/
  README.md
```

## Scope

This repository intentionally does **not** contain a final embedded QA project yet.

The current goal is:

```text
Python problem solving
        ↓
Python fluency
        ↓
Embedded QA-focused practice
        ↓
Later: pytest / pyserial / real hardware testing
```

The practical automation stage can be added separately after the Python foundation is complete.
