# Phase 3 — Critical Problem Solving on Coding Platforms

> **Duration:** ~6–8 weeks (≈ 20 sessions)
> **Goal:** Train the *thinking* muscle. The kid stops copying patterns and
> starts attacking new problems with a method.

---

## Why this phase exists

Knowing Python ≠ being able to solve problems with Python. This phase is
where the parent's specific ask — *"critical problem solving over coding
platforms"* — gets its own dedicated, structured runway.

Even more importantly, data science is mostly **problem framing** in
disguise: *"What question am I actually trying to answer? What does the
data tell me? What's the simplest experiment to find out?"* The habits we
build here transfer directly.

---

## What we're learning

This is less about new syntax and more about **habits of mind**:

1. **The STO loop** — Solve → Talk-through → Optimize (introduced below).
2. **Reading a problem statement carefully** (and re-reading it).
3. **Working a small example by hand first**.
4. **Spotting the *pattern* of a problem** (counter, accumulator, lookup,
   two-pointer-lite, simulation, etc.).
5. **Edge cases** — empty input, one element, negatives, very large input.
6. **Time / space "feel"** — not Big-O proofs, just "does this scale?"
7. **Reading other people's solutions** *after* solving yours.

We also pick up, *through problems*, a few new tools:

- List comprehensions (gentle).
- `sorted`, `min`, `max`, `sum`, `len`, `any`, `all`, `zip`, `enumerate`.
- `set` (for "have I seen this before?") and `Counter` from `collections`.
- Recursion — *one* week, *very* gently, with the staircase / Russian-doll
  analogy.

---

## The STO loop (do this for *every* problem)

```
        ┌─────────┐
        │  READ   │ ← read it twice; rewrite the question in your own words
        └────┬────┘
             ▼
        ┌─────────┐
        │  PLAN   │ ← work one tiny example on paper before any code
        └────┬────┘
             ▼
        ┌─────────┐
   ┌──▶ │  SOLVE  │ ← get *anything* working — ugly is fine
   │    └────┬────┘
   │         ▼
   │    ┌─────────┐
   │    │ EXPLAIN │ ← narrate the code to the parent, line by line
   │    └────┬────┘
   │         ▼
   │    ┌─────────┐
   └────│OPTIMIZE │ ← simpler? shorter? clearer? more general?
        └─────────┘
```

The *Explain* step is where most learning happens. If the kid can't
explain a line, that line is borrowed, not earned — rewrite it from
understanding.

---

## Watch (videos — short and curated)

Problem solving is mostly *doing*, not watching, so the video diet is
small here.

| Topic                                | Channel / Video                                                                                                                          | Length |
|--------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------|--------|
| How to think about a problem         | freeCodeCamp — [*"How to think like a programmer"*](https://www.youtube.com/watch?v=azcrPFhaY9k)                                          | 8 min  |
| Polya's 4 steps (kid-friendly)       | TED-Ed — [*"Can you solve…?"* riddle playlist](https://www.youtube.com/playlist?list=PLJicmE8fK0EgVwBRDvSJyTfufx7ynjpJW)                  | 5 min  |
| Reading errors confidently           | re-watch the mCoding traceback short from Phase 2                                                                                        | 4 min  |
| What's an algorithm? (revisit)       | Crash Course CS — [Ep. 13 *"Algorithms"*](https://www.youtube.com/watch?v=rL8X2mlNHPM)                                                    | 12 min |
| Sorting visualized                   | Timo Bingmann — [*"15 Sorting Algorithms in 6 Minutes"*](https://www.youtube.com/watch?v=kPRA0W1kECg)                                     | 6 min  |
| Searching visualized                 | Computerphile — [*"Binary Search"*](https://www.youtube.com/results?search_query=computerphile+binary+search)                             | 9 min  |

That's it for the phase. Resist the urge to add more — *they need reps,
not lectures*.

---

## Play (the platforms, in order of difficulty)

We climb a ladder. Don't skip rungs.

### Rung 1 — [CodingBat](https://codingbat.com/python)

- **Best beginner site in the world.** Microscopic problems, one function
  each, instant feedback in the browser.
- Order to do them in:
  [Warmup-1](https://codingbat.com/python/Warmup-1) → [Warmup-2](https://codingbat.com/python/Warmup-2) →
  [String-1](https://codingbat.com/python/String-1) → [List-1](https://codingbat.com/python/List-1) →
  [Logic-1](https://codingbat.com/python/Logic-1) → [String-2](https://codingbat.com/python/String-2) →
  [List-2](https://codingbat.com/python/List-2) → [Logic-2](https://codingbat.com/python/Logic-2)
- Goal for this phase: **at least 80 problems solved**.

### Rung 2 — [Edabit](https://edabit.com)

- Beautiful UI, gamified XP, problems tagged by difficulty.
- Stay in **"Very Easy" and "Easy"** for this phase.
- Goal: **at least 40 problems** across "Very Easy" → "Easy".

### Rung 3 — [HackerRank "Python" track](https://www.hackerrank.com/domains/python), *Easy* only

- Specifically the **"Introduction"** and **"Basic Data Types"** sections.
- Slightly more "test-input-from-stdin" style — good prep for any contest.

### Rung 4 (stretch) — [CodeChef "Beginner" / "School" practice](https://www.codechef.com/practice)

- Filter *Difficulty: 1★*.
- Only attempt these in the **last 2 weeks** of the phase, and only if
  Rungs 1–3 feel easy.
- Skip the contests for now — the time pressure is unhelpful at this age.

> **Avoid LeetCode for now.** Its problem culture is built for adult job
> interviews; the difficulty curve and the discussion-section vibes are
> not age-appropriate yet. We'll meet it in high school if needed.

---

## A typical Phase 3 session

```
00:00–00:05   Warm-up: 1 easy CodingBat problem solo (timed, fun).
00:05–00:20   New concept of the day (e.g., "the Counter pattern").
              Parent or video walks through ONE worked example.
00:20–00:45   Kid solves 2–3 problems in that pattern.
              STO loop on each. Parent only nudges with questions:
              "What happens if the list is empty?" "Can you draw it?"
00:45–00:55   Reflect: kid writes one line in solved/NOTES.md
              about what they learned today.
00:55–01:00   Explain back: kid teaches the day's pattern to parent.
```

---

## Curriculum of "patterns" (one per week)

| Week | Pattern              | Example problem                                                |
|------|----------------------|----------------------------------------------------------------|
| 1    | **Counter / Tally**  | Count vowels in a word; count even numbers in a list           |
| 2    | **Accumulator**      | Sum of digits; product of a list; running max                  |
| 3    | **Filter & map**     | Keep only positive numbers; double every odd number            |
| 4    | **Search**           | First index of X; does this string contain Y?                  |
| 5    | **Sort & extremes**  | Top-3 scores; second largest number; sort by length            |
| 6    | **Lookup with dict / set** | Most frequent letter; find duplicates; "have I seen this?" |
| 7    | **Simulation**       | Bouncing ball; simulate a dice game; "rotate this list N times" |
| 8    | **Gentle recursion** | Factorial, Fibonacci, "draw a triangle of stars"               |

Each pattern is taught once, then reinforced in problems for the rest of
the phase. By the end, the kid should recognize the *shape* of a problem
on sight.

---

## Build (small, problem-solving flavored)

Two project bursts in this phase, each one session:

1. **Personal Solver Book** — a tiny static site (just one `index.html` or
   a [Notion](https://www.notion.so) page) where the kid lists every problem they've solved with:
   - link
   - their solution
   - one line: *"What was the trick?"*

   This becomes their portfolio. By the end of Phase 3, it should have
   ~100 problems in it. Watching the list grow is *enormously*
   motivating.

2. **Mini Olympiad** — pick 5 problems they haven't seen, of mixed
   difficulty. Time it (60 minutes). No help. Then review together.
   Do this once around week 6 and once at the end. Celebrate, don't grade.

---

## Critical thinking, beyond code

Problem solving isn't only on a screen. Once a week, do **one non-code
puzzle** together. Rotate:

- [**Bebras Challenges**](https://www.bebraschallenge.org) — free past papers; every problem is a CS-thinking puzzle in disguise.
- [**Brilliant.org "Logic"**](https://brilliant.org/courses/logic-deduction/) course.
- **Smullyan-style** knights-and-knaves riddles (search YouTube for [Ted-Ed Smullyan-style riddles](https://www.youtube.com/results?search_query=ted-ed+knights+knaves+riddle)).
- A real-life decomposition: *"How would you organize a 30-person birthday
  party? Break it into the smallest possible steps."*

This keeps "problem solving" from collapsing into "screen problem solving".

---

## Explain back (checkpoints)

- Every Friday, the kid presents **one problem they're proud of**. They:
  1. Read the problem out loud.
  2. Show their solution.
  3. Explain *why* their solution works.
  4. Mention one **alternative** approach they considered.

- Once a month, the kid teaches **one pattern** (e.g., "the Counter
  pattern") to a sibling or parent — by inventing their *own* example
  problem.

---

## Exit ticket

Before moving to Phase 4, the kid must:

1. ✅ Have solved **at least 100 problems** total across CodingBat / Edabit /
   HackerRank (volume *is* the point here — it builds fluency).
2. ✅ Walk through a **brand-new "Easy" problem** start-to-finish with the
   STO loop, narrating each step out loud.
3. ✅ Identify the **pattern** of a problem they've never seen (counter?
   filter? lookup?) before writing any code.
4. ✅ Spot at least one **edge case** for any problem unprompted (empty
   input, single element, negatives, duplicates, very long input).

---

Next: [`phase-4-data-and-stats.md`](./phase-4-data-and-stats.md) — *Now
the data showing up. Time to think in numbers.*
