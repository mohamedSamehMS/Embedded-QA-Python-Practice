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

**What this repo is not:** a general algorithms archive in Python, and not a collection of hardware validation scripts either. Every problem is picked for a specific embedded-QA reason (see the table below), and problems chosen for general algorithmic fluency (arrays, DP, graphs) belong in the C-focused repo instead.

## Goal

Build enough Python fluency in string/error/collection/time handling that writing a `pyserial`-based validation script — reading a serial log from a microcontroller, parsing expected-vs-actual output, flagging a mismatch, retrying on timeout — is a five-minute task rather than a lookup-heavy one, once that script actually needs to be written.

## Learning approach

Two tracks run in parallel rather than sequentially:

- **DataCamp** — structured courses for learning the concept properly first (syntax, standard library modules, correct usage patterns).
- **HackerRank / LeetCode** — unstructured application, no guardrails, forces recalling and applying what DataCamp taught rather than following along.

## Why these specific problems

| Subdomain | Why it matters for embedded QA |
|---|---|
| **Errors and Exceptions** | Maps directly to catching `SerialTimeoutException` / `SerialException` and building retry logic when a board doesn't respond |
| **Date and Time** | Timestamping log entries, measuring test duration, detecting timeouts |
| **Collections** | `Counter` for pass/fail tallies, `deque` for modeling a serial read buffer, `OrderedDict` for preserving log sequence while deduplicating |
| **Regex and Parsing** | The single most directly relevant subdomain — extracting sensor values and structured fields out of raw UART/log text |

## Overview

| | |
|---|---|
| **Repo type** | Problem-solving practice (not a tooling or validation-script repo) |
| **Companion repo** | [Embedded-C-Practice](https://github.com/mohamedSamehMS/Embedded-C-Practice) — the firmware/embedded-C half of the same overall practice |
| **Platforms** | HackerRank (active), LeetCode (planned) |
| **Learning support** | DataCamp courses, run in parallel |
| **Target use case** | Building the Python fluency `pyserial`-based validation scripts and test-log parsing would eventually need |

## Progress — HackerRank Python

**Errors and Exceptions**
| Problem | Status | Link |
|---|---|---|
| Exceptions | ⬜ Not started | TODO — paste once found on HackerRank |
| Incorrect Regex | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/incorrect-regex/problem) |

**Date and Time**
| Problem | Status | Link |
|---|---|---|
| Calendar Module | ⬜ Not started | TODO — paste once found on HackerRank |
| Time Delta | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/python-time-delta/problem) |

**Collections**
| Problem | Status | Link |
|---|---|---|
| collections.OrderedDict() | ⬜ Not started | [problem](https://www.hackerrank.com/challenges/py-collections-ordereddict/problem) |
| collections.Counter() | ⬜ Not started | TODO — paste once found on HackerRank |
| collections.deque() | ⬜ Not started | TODO — paste once found on HackerRank |

**Regex and Parsing**
| Problem | Status | Link |
|---|---|---|
| Detect Floating Point Number | ⬜ Not started | TODO — paste once found on HackerRank |
| Re.split() | ⬜ Not started | TODO — paste once found on HackerRank |

A few links are marked TODO rather than guessed — no fabricated URLs. Paste the real link the first time you open each problem.

### LeetCode

Not started — see [leetcode/README.md](leetcode/README.md) for planned structure.

## Repository layout

```
hackerrank/
  errors-and-exceptions/
  date-and-time/
  collections/
  regex-and-parsing/
leetcode/
  (added once populated)
```

## File convention

Every Python solution file starts with a header block that includes *why* the problem was chosen, not just what it is:
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
