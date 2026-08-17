<p align="center">
  <img src="https://hrcdn.net/fcore/assets/brand/logo-new-white-green-a5cb16e0ae.svg" alt="HackerRank" height="40" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/language-Python-blue" alt="Language" />
  <img src="https://img.shields.io/badge/focus-Embedded%20Systems%20Validation%20%26%20QA-orange" alt="Focus" />
  <img src="https://img.shields.io/badge/status-active-brightgreen" alt="Status" />
  <img src="https://img.shields.io/badge/learning-DataCamp-03EF62" alt="DataCamp" />
</p>

# Embedded-QA-Python-Practice

**Python problem-solving practice, curated for embedded systems validation and QA automation.** Every problem here is chosen — not just completed — because it builds a skill that shows up when writing PC-side test scripts that talk to embedded hardware over serial: parsing UART/log output, handling communication failures, timing test runs, structuring results.

## Purpose

This is the Python half of a broader problem-solving practice. It's a practice repo, not a tooling repo — the deliverable here is solved problems with notes, not runnable scripts against real hardware. The firmware/embedded-C half of the same overall practice lives in a separate repo: [Embedded-C-Practice](https://github.com/mohamedSamehMS/Embedded-C-Practice).

**What this repo is not:** a general algorithms archive in Python, and not a collection of hardware validation scripts either. Every problem is picked for a specific embedded-QA reason (see below), and problems chosen for general algorithmic fluency belong in the C-focused repo instead.

## Goal

Build enough Python fluency in string/error/collection/set/time handling that writing a `pyserial`-based validation script — reading a serial log from a microcontroller, parsing expected-vs-actual output, flagging a mismatch, retrying on timeout — is a five-minute task rather than a lookup-heavy one, once that script actually needs to be written.

## Learning approach

Two tracks run in parallel rather than sequentially:

- **DataCamp** — structured courses for learning the concept properly first.
- **HackerRank / LeetCode** — unstructured application, no guardrails.

## Subdomain selection — all 17 reviewed

HackerRank's Python domain has 17 subdomains. Each was evaluated specifically against "does this build a skill used in writing embedded driver validation scripts."

**Included (11)**

| Subdomain | Why it matters for embedded QA |
|---|---|
| **Errors and Exceptions** | Catching `SerialTimeoutException` / `SerialException`, retry logic when a board doesn't respond |
| **Date and Time** | Timestamping log entries, measuring test duration, detecting timeouts |
| **Collections** | `Counter` for pass/fail tallies, `deque` for a serial read buffer, `OrderedDict` for log sequencing |
| **Regex and Parsing** | Extracting sensor values and structured fields out of raw UART/log text — the single most relevant subdomain |
| **Closures and Decorators** | The mechanism behind `@retry` / `@timeout` wrappers around a flaky serial call |
| **XML** | Parsing JUnit-style test reports and nested config files |
| **Strings** | Splitting raw log lines into fields, validating field formats, formatting readable console reports |
| **Sets** | Comparing expected vs actual configuration — e.g. verifying every expected interrupt/pin is actually enabled |
| **Itertools** | Generating exhaustive test-parameter combinations; compressing repeated consecutive log lines |
| **Built-Ins** | `any`/`all` for aggregate pass/fail checks, `zip` for pairing expected-vs-actual lists, custom sort for ordering results |
| **Python Functionals** | `map`/`filter`/`reduce` for transforming and aggregating lists of test results |

**Excluded (6), with reasons**

| Subdomain | Why it's out |
|---|---|
| Introduction, Basic Data Types | Too general — no distinct embedded-QA angle beyond what's already covered |
| Math | Geometry/triangle-focused problems, no meaningful tie to driver validation |
| Classes | HackerRank's 2 problems are generic math OOP (complex numbers, torsional angle), not test-framework design |
| Numpy | Array/signal computation — only relevant for statistical ADC/waveform analysis, which isn't current scope |
| Debugging | Thin (2 problems), format is spot-the-bug in unrelated snippets — real debugging is already being practiced more meaningfully through live QA cycles and actual firmware bug-hunting (e.g. the NVIC priority bug already found and fixed) |

## Link verification note

Problem names below are all confirmed real HackerRank Python challenges, cross-checked across multiple sources. Exact URLs are only included where independently verified against HackerRank directly — everything else is marked TODO rather than guessed, consistent with this repo's no-fabricated-links policy. Paste the real link in the first time you open each problem; that's the fastest way to close these out as you actually reach them.

## Progress — HackerRank Python

**Errors and Exceptions**
| Problem | Status | Link |
|---|---|---|
| Exceptions | ⬜ Not started | TODO |
| Incorrect Regex | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/incorrect-regex/problem) |

**Date and Time**
| Problem | Status | Link |
|---|---|---|
| Calendar Module | ⬜ Not started | TODO |
| Time Delta | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/python-time-delta/problem) |

**Collections**
| Problem | Status | Link |
|---|---|---|
| collections.OrderedDict() | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/py-collections-ordereddict/problem) |
| collections.Counter() | ⬜ Not started | TODO |
| collections.deque() | ⬜ Not started | TODO |

**Regex and Parsing**
| Problem | Status | Link |
|---|---|---|
| Detect Floating Point Number | ⬜ Not started | TODO |
| Re.split() | ⬜ Not started | TODO |

**Closures and Decorators**
| Problem | Status | Link |
|---|---|---|
| Standardize Mobile Number Using Decorators | ⬜ Not started | TODO |
| Decorators 2 - Name Directory | ⬜ Not started | TODO |

**XML**
| Problem | Status | Link |
|---|---|---|
| XML 1 - Find the Score | ⬜ Not started | TODO |
| XML 2 - Find the Maximum Depth | ⬜ Not started | TODO |

**Strings**
| Problem | Status | Link |
|---|---|---|
| String Split and Join | ⬜ Not started | TODO |
| String Validators | ⬜ Not started | TODO |
| Text Alignment | ⬜ Not started | TODO |

**Sets**
| Problem | Status | Link |
|---|---|---|
| Symmetric Difference | ⬜ Not started | TODO |
| Check Subset | ⬜ Not started | TODO |
| Check Strict Superset | ⬜ Not started | TODO |

**Itertools**
| Problem | Status | Link |
|---|---|---|
| itertools.product() | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/itertools-product/problem) |
| itertools.combinations() | ⬜ Not started | TODO |
| Compress the String! | ⬜ Not started | TODO |

**Built-Ins**
| Problem | Status | Link |
|---|---|---|
| Any or All | ⬜ Not started | TODO |
| Zipped! | ⬜ Not started | TODO |
| Athlete Sort | ⬜ Not started | TODO |

**Python Functionals**
| Problem | Status | Link |
|---|---|---|
| Map and Lambda Function | ⬜ Not started | TODO |
| Reduce Function | ⬜ Not started | TODO |

### LeetCode

Not started — see [leetcode/README.md](leetcode/README.md) for planned structure.

## Repository layout

```
hackerrank/
  errors-and-exceptions/
  date-and-time/
  collections/
  regex-and-parsing/
  closures-and-decorators/
  xml/
  strings/
  sets/
  itertools/
  built-ins/
  python-functionals/
leetcode/
  (added once populated)
```

## File convention

Every Python solution file starts with a header block that includes *why* the problem was chosen:
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

Update a problem's status to 🟨 In progress or ✅ Solved as you work through it.
