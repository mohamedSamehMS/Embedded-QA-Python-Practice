<p align="center">
  <img src="https://hrcdn.net/fcore/assets/brand/logo-new-white-green-a5cb16e0ae.svg" alt="HackerRank" height="40" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/language-Python-blue" alt="Language" />
<<<<<<< HEAD
  <img src="https://img.shields.io/badge/focus-Embedded%20QA-orange" alt="Focus" />
=======
  <img src="https://img.shields.io/badge/focus-Embedded%20Systems%20Validation%20%26%20QA-orange" alt="Focus" />
>>>>>>> origin/main
  <img src="https://img.shields.io/badge/status-active-brightgreen" alt="Status" />
  <img src="https://img.shields.io/badge/learning-DataCamp-03EF62" alt="DataCamp" />
</p>

# Embedded-QA-Python-Practice

<<<<<<< HEAD
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
=======
**Python problem-solving practice, curated for embedded systems validation and QA automation.** Every problem here supports one goal: writing PC-side test scripts that talk to embedded hardware over serial — parsing UART/log output, handling communication failures, timing test runs, structuring results.

## Purpose

This is the Python half of a broader problem-solving practice. It's a practice repo, not a tooling repo. The firmware/embedded-C half lives in [Embedded-C-Practice](https://github.com/mohamedSamehMS/Embedded-C-Practice).

## Goal

Build enough Python fluency that writing a `pyserial`-based validation script is a five-minute task, not a lookup-heavy one, once that script actually needs to be written.

## Learning approach

Two tracks run in parallel: **DataCamp** for structured concept-learning, **HackerRank / LeetCode** for unstructured application.

## Subdomain selection — all 17 reviewed

**Included (11) — full problem set for each, 76 problems total**

| Subdomain | Why it matters for embedded QA | Count |
|---|---|---|
| Errors and Exceptions | Catching `SerialTimeoutException`/`SerialException`, retry logic | 2 |
| Date and Time | Timestamping logs, measuring duration, detecting timeouts | 2 |
| Collections | `Counter`/`deque`/`OrderedDict` for tallying, buffering, ordering | 8 |
| Regex and Parsing | Extracting values from raw UART/log text | 17 |
| Closures and Decorators | `@retry`/`@timeout` wrapper mechanism | 2 |
| XML | JUnit-style test report parsing | 2 |
| Strings | Splitting/validating/formatting raw log fields | 14 |
| Sets | Comparing expected vs actual configuration | 13 |
| Itertools | Test-matrix generation, log compression | 7 |
| Built-Ins | Aggregate pass/fail checks, pairing expected/actual, sorting | 6 |
| Python Functionals | Transforming and aggregating result lists | 3 |

**Excluded (6)**

| Subdomain | Why it's out |
|---|---|
| Introduction, Basic Data Types | Too general, no distinct embedded-QA angle |
| Math | Geometry-focused, no meaningful tie |
| Classes | The 2 problems are generic math OOP, not test-framework design |
| Numpy | Only relevant for statistical ADC/signal analysis — not current scope |
| Debugging | Thin (2 problems), spot-the-bug format — real debugging already practiced through live QA/firmware work |

## Link verification note

Every problem name below is a confirmed real HackerRank challenge. Exact URLs are included only where independently verified — the rest are marked TODO rather than guessed, so nothing here is a dead or wrong link. Paste the real link in as you open each problem.

## Progress — HackerRank Python

### Errors and Exceptions
| Problem | Status | Link |
|---|---|---|
| Exceptions | ⬜ | TODO |
| Incorrect Regex | ⬜ | [problem](https://www.hackerrank.com/challenges/incorrect-regex/problem) |

### Date and Time
| Problem | Status | Link |
|---|---|---|
| Calendar Module | ⬜ | TODO |
| Time Delta | ⬜ | [problem](https://www.hackerrank.com/challenges/python-time-delta/problem) |

### Collections
| Problem | Status | Link |
|---|---|---|
| collections.Counter() | ⬜ | TODO |
| DefaultDict Tutorial | ⬜ | TODO |
| Collections.namedtuple() | ⬜ | TODO |
| Collections.OrderedDict() | ⬜ | [problem](https://www.hackerrank.com/challenges/py-collections-ordereddict/problem) |
| Word Order | ⬜ | TODO |
| Collections.deque() | ⬜ | TODO |
| Company Logo | ⬜ | TODO |
| Piling Up! | ⬜ | TODO |

### Regex and Parsing
| Problem | Status | Link |
|---|---|---|
| Detect Floating Point Number | ⬜ | TODO |
| Re.split() | ⬜ | TODO |
| Group(), Groups() & Groupdict() | ⬜ | TODO |
| Re.findall() & Re.finditer() | ⬜ | TODO |
| Re.start() & Re.end() | ⬜ | TODO |
| Regex Substitution | ⬜ | TODO |
| Validating Roman Numerals | ⬜ | TODO |
| Validating phone numbers | ⬜ | TODO |
| Validating and Parsing Email Addresses | ⬜ | TODO |
| Hex Color Code | ⬜ | TODO |
| HTML Parser - Part 1 | ⬜ | TODO |
| HTML Parser - Part 2 | ⬜ | TODO |
| Detect HTML Tags, Attributes and Attribute Values | ⬜ | TODO |
| Validating UID | ⬜ | TODO |
| Validating Credit Card Numbers | ⬜ | TODO |
| Validating Postal Codes | ⬜ | TODO |
| Matrix Script | ⬜ | TODO |

### Closures and Decorators
| Problem | Status | Link |
|---|---|---|
| Standardize Mobile Number Using Decorators | ⬜ | TODO |
| Decorators 2 - Name Directory | ⬜ | TODO |

### XML
| Problem | Status | Link |
|---|---|---|
| XML 1 - Find the Score | ⬜ | TODO |
| XML 2 - Find the Maximum Depth | ⬜ | TODO |

### Strings
| Problem | Status | Link |
|---|---|---|
| sWAP cASE | ⬜ | TODO |
| String Split and Join | ⬜ | TODO |
| What's Your Name? | ⬜ | TODO |
| Mutations | ⬜ | TODO |
| Find a string | ⬜ | TODO |
| String Validators | ⬜ | TODO |
| Text Alignment | ⬜ | TODO |
| Text Wrap | ⬜ | TODO |
| Designer Door Mat | ⬜ | TODO |
| Merge the Tools! | ⬜ | TODO |
| String Formatting | ⬜ | TODO |
| Alphabet Rangoli | ⬜ | TODO |
| Capitalize! | ⬜ | TODO |
| The Minion Game | ⬜ | TODO |

### Sets
| Problem | Status | Link |
|---|---|---|
| Introduction to Sets | ⬜ | TODO |
| Symmetric Difference | ⬜ | TODO |
| Set .add() | ⬜ | TODO |
| Set .union() Operation | ⬜ | TODO |
| Set .intersection() Operation | ⬜ | TODO |
| Set .difference() Operation | ⬜ | TODO |
| Set .symmetric_difference() Operation | ⬜ | TODO |
| Set Mutations | ⬜ | TODO |
| The Captain's Room | ⬜ | TODO |
| Check Subset | ⬜ | TODO |
| Check Strict Superset | ⬜ | TODO |
| Set .discard(), .remove() & .pop() | ⬜ | TODO |
| No Idea! | ⬜ | TODO |

### Itertools
| Problem | Status | Link |
|---|---|---|
| itertools.product() | ⬜ | [problem](https://www.hackerrank.com/challenges/itertools-product/problem) |
| itertools.permutations() | ⬜ | TODO |
| itertools.combinations() | ⬜ | TODO |
| itertools.combinations_with_replacement() | ⬜ | TODO |
| Compress the String! | ⬜ | TODO |
| Iterables and Iterators | ⬜ | TODO |
| Maximize It! | ⬜ | TODO |

### Built-Ins
| Problem | Status | Link |
|---|---|---|
| Zipped! | ⬜ | TODO |
| Input() | ⬜ | TODO |
| Python Evaluation | ⬜ | TODO |
| Any or All | ⬜ | TODO |
| Athlete Sort | ⬜ | TODO |
| ginortS | ⬜ | TODO |

### Python Functionals
| Problem | Status | Link |
|---|---|---|
| Map and Lambda Function | ⬜ | TODO |
| Validating Email Addresses With a Filter | ⬜ | TODO |
| Reduce Function | ⬜ | TODO |

**5 of 76 links independently verified so far** — the rest read TODO by design, not by omission.

### LeetCode

Not started — see [leetcode/README.md](leetcode/README.md).

## Repository layout

```
hackerrank/
  errors-and-exceptions/   (2)
  date-and-time/           (2)
  collections/             (8)
  regex-and-parsing/       (17)
  closures-and-decorators/ (2)
  xml/                     (2)
  strings/                 (14)
  sets/                    (13)
  itertools/               (7)
  built-ins/               (6)
  python-functionals/      (3)
leetcode/
  (added once populated)
```

## File convention
>>>>>>> origin/main

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

<<<<<<< HEAD
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
=======
Update a problem's status to 🟨 In progress or ✅ Solved as you work through it.
>>>>>>> origin/main
