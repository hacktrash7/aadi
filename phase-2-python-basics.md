# Phase 2 — Python Basics: First Real Code

> **Duration:** ~6–8 weeks (≈ 20 sessions)
> **Goal:** Read, write, and *debug* small Python programs comfortably.
> Translate every Phase-1 idea (loop, condition, variable) into Python
> syntax — and start to feel "fluent enough to play".

---

## Why this phase exists

Python is the lingua franca of data science. We pick it for three reasons:

1. **Reads like English.** `if score > 10: print("you win")` — that
   basically *is* a sentence.
2. **Forgiving for beginners.** No semicolons, no types to declare, errors
   are mostly readable.
3. **Same Python all the way up.** The code we write in week 6 of this
   phase looks structurally identical to the code we'll write in Phase 5
   for data science. No re-learning.

---

## What we're learning

| Block                  | Specific topics                                                        |
|------------------------|------------------------------------------------------------------------|
| **Hello, Python**      | `print`, comments, running code, reading errors                        |
| **Variables & types**  | int, float, string, bool, naming, reassignment                         |
| **Input & output**     | `input()`, type-casting (`int(...)`, `float(...)`), f-strings          |
| **Math**               | `+ - * / // % **`, order of operations, `math` module basics           |
| **Conditions**         | `if / elif / else`, comparison & logical operators                     |
| **Loops**              | `for` (with `range` and lists), `while`, `break`, `continue`           |
| **Lists**              | indexing, slicing, append/remove, length, iteration                    |
| **Strings**            | slicing, `.upper()`, `.lower()`, `.split()`, `in`                      |
| **Dictionaries**       | key–value pairs, lookup, iteration                                     |
| **Functions**          | `def`, parameters, return, scope (light touch), docstrings             |
| **Modules**            | `import random`, `import math`, `import datetime`                      |
| **Files (gentle)**     | reading a `.txt` file line by line — *foreshadows pandas in Phase 5*   |

We do **not** cover classes, OOP, decorators, comprehensions (we'll meet
list comprehensions naturally in Phase 5), exceptions beyond a basic
`try/except`. Keep the surface area small.

---

## Watch (videos & visual demos)

The "spine" video series is the **freeCodeCamp "Python for Beginners with
Mike Dane"** ([▶ full course, ~1 hr](https://www.youtube.com/watch?v=rfscVS0vtbw)), broken into 3-to-5-min chapters. Watch
**one chapter per session**, never more.

Supplement with:

| Topic                  | Channel / Video                                                                                                                                       | Length |
|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------|--------|
| What is a variable?    | CS Dojo — [*"Python Tutorial for Beginners 1"*](https://www.youtube.com/watch?v=Z1Yd7upQsXY)                                                          | 11 min |
| f-strings              | Corey Schafer — [*"Python Quick Tip: f-strings"*](https://www.youtube.com/watch?v=nghuHvKLhJA)                                                        | 5 min  |
| Lists vs dicts         | Tech With Tim — [*"Python Lists vs Dictionaries"*](https://www.youtube.com/results?search_query=tech+with+tim+lists+vs+dictionaries+python)           | 6 min  |
| How loops work         | Computerphile — [*"Iteration"*](https://www.youtube.com/results?search_query=computerphile+iteration)                                                 | 5 min  |
| Reading errors         | mCoding — [*"How to read a Python traceback"*](https://www.youtube.com/results?search_query=mcoding+python+traceback)                                 | 4 min  |

Add **3Blue1Brown's** [intro on functions / "a machine that takes input → output"](https://www.youtube.com/@3blue1brown/search?query=function) during the function week — beautiful visualization.

---

## Play (interactive platforms)

### Primary — [Replit](https://replit.com)

- Free, browser-based, **no install ever**.
- Make one Replit account for the kid. Every project lives there.
- We use the **classic Python** template.

### Visual side-quests — pick *one* and use across the phase

These are gamified Python platforms. Pick whichever the kid clicks with —
don't force one.

- [**CodeCombat**](https://codecombat.com) (Python mode) — top-down RPG; the kid writes Python to move
  a hero. Excellent for syntax muscle memory. Free tier is enough.
- [**Tynker Python**](https://www.tynker.com/programming/python) — heavier on visuals, slightly younger feel.
- [**Mimo**](https://mimo.org) (mobile app) — bite-sized lessons, good for car rides / waiting
  rooms. Great supplement, *not* a main course.

### Drill yard — [`pythontutor.com`](https://pythontutor.com/python-debugger.html)

This is **non-negotiable**. PythonTutor visualizes Python code execution
**step by step** with arrows showing variables changing in memory.

Whenever the kid says "but *why* did that happen?" — paste the code into
PythonTutor and step through it together. This single habit is worth more
than 10 videos.

---

## Build (mini-projects)

We build **one project per week**, building roughly from "uses a variable"
to "uses everything we know".

| Week | Project                          | What it teaches                              |
|------|----------------------------------|----------------------------------------------|
| 1    | **Mad Libs**                     | input, strings, f-strings                    |
| 1    | **Tip / Bill Splitter**          | math, floats, formatting                     |
| 2    | **Guess the Number**             | `while`, conditions, `random`                |
| 2    | **Rock–Paper–Scissors**          | conditions, `random`, functions (introduced) |
| 3    | **Times-Table Quiz**             | `for`, `range`, scoring                      |
| 3    | **Hangman** (text version)       | lists, strings, loops, functions             |
| 4    | **To-Do List (CLI)**             | lists, menus, `while True`, functions        |
| 4    | **Dice-Roll Statistics**         | loops + counters → *foreshadows stats!*      |
| 5    | **Address Book** (dictionaries)  | dicts, search, update                        |
| 5    | **Simple Calculator** (menu)     | functions, recursion-free, error handling    |
| 6    | **Pokemon Battle (text)**        | dicts of stats, conditions, RNG, decomposition |
| 6    | **Story Generator** (Mad-Libs++) | random + lists + functions                   |
| 7    | **Personal Finance Tracker**     | files (read/write a `.txt`), dicts, totals   |
| 8    | **MINI-CAPSTONE: Quiz Game with Score File** — full project: load questions from a file, ask them in random order, save high scores to a file. | All of the above |

**Rule:** the mini-capstone in week 8 must be built **without copying any
tutorial**. The kid plans it on paper first (decomposition!), then codes.

---

## How to teach syntax (the "translation" trick)

For the first 3 weeks, every new Python concept is taught as a *translation*
from Phase-1 Scratch blocks:

| Scratch block                         | Python equivalent                             |
|---------------------------------------|-----------------------------------------------|
| `when green flag clicked`             | the top of the file                           |
| `set score to 0`                      | `score = 0`                                   |
| `change score by 1`                   | `score = score + 1`  *(or `score += 1`)*      |
| `repeat 10`                           | `for i in range(10):`                         |
| `forever`                             | `while True:`                                 |
| `if <touching wall>`                  | `if touching_wall:`                           |
| `ask "..." and wait`                  | `answer = input("...")`                       |
| `say "Hello"`                         | `print("Hello")`                              |

Print this table and stick it on the wall next to the laptop for 3 weeks.
Take it down once the kid stops glancing at it.

---

## Critical-thinking spice (small dose)

Even though Phase 3 is the dedicated problem-solving phase, in this phase
we sprinkle **one CodingBat warm-up at the start of each session** from
week 4 onwards. Pick from the **Warmup-1** and **String-1** sections of
[codingbat.com/python](https://codingbat.com/python). It takes 5 minutes
and quietly builds the muscle.

---

## Explain back (checkpoints)

Each Friday session, the kid does a **2-minute "show & tell"** of the
week's project to a parent or sibling. Required structure:

1. *"This is what it does."* (demo)
2. *"This is how it works."* (open the code, point at the loop)
3. *"This was the trickiest bug I fixed."* (show what they learned)

---

## Exit ticket

Before moving to Phase 3, the kid must:

1. ✅ Write, from a blank file, a Python program that uses **a function,
   a loop, an `if/else`, a list, and a dictionary** — and runs without
   errors. (The quiz-game mini-capstone counts.)
2. ✅ Read a 20-line Python program they've **never seen** and explain
   what it does, line by line.
3. ✅ When shown a Python *error message*, identify what kind of error
   it is (`SyntaxError`, `NameError`, `TypeError`, `IndexError`,
   `KeyError`) and where to look.
4. ✅ Use [**PythonTutor**](https://pythontutor.com/python-debugger.html) independently to debug their own code at least once.

---

Next: [`phase-3-problem-solving.md`](./phase-3-problem-solving.md) — *Now
that we can write Python, let's think harder.*
