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
