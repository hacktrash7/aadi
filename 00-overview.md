# 00 — Overview, Philosophy, and Ground Rules

This document is for the **parent / mentor** more than the kid. Read it once,
then use it as a reference when things feel off-track.

---

## 1. Who this is designed for

- A 6th-grader (~11–12 years old).
- **Smart and curious**, but with **no coding background**.
- Prefers **visuals and video-based learning**.
- Has limited weekday time because of school — assume **3 sessions × 45–60
  min/week**, plus optional weekend tinkering.

If any of those change (e.g., the kid suddenly wants to do 2 hours a day on
holidays), don't slow them down — let them sprint. But never speed *up* just
because you're impatient. Pace is set by the kid.

---

## 2. The learning loop we use every single session

Every session — from "what is a variable" to "train a neural network" —
follows the same 5-beat rhythm:

```
[ HOOK ] → [ WATCH ] → [ PLAY ] → [ BUILD ] → [ EXPLAIN BACK ]
  2 min    5–10 min    15–20 min  15–20 min      5 min
```

| Beat            | What happens                                                                                       |
|-----------------|----------------------------------------------------------------------------------------------------|
| **Hook**        | A question, a meme, a magic trick. "How does Netflix know what you'll like?" Curiosity first.      |
| **Watch**       | One short, *high-quality* video or animation. Never longer than 10 min.                            |
| **Play**        | Interactive platform — [Scratch](https://scratch.mit.edu), [Trinket](https://trinket.io), [Replit](https://replit.com), [Brilliant](https://brilliant.org). Hands on keyboard, low stakes. |
| **Build**       | Tiny project applying the day's idea. Must produce a visible artifact (a chart, a game, a number). |
| **Explain back**| Kid explains the day's idea to the parent in *under 5 minutes*. Parent plays dumb on purpose.      |

The **Explain Back** beat is the secret weapon. It catches misconceptions
early and trains the kid to *own* the knowledge — which is exactly what
data science work looks like in real life (explaining to non-technical
people).

---

## 3. Why visuals first, syntax later

A 6th-grader's brain is *spectacular* at pattern recognition and analogy,
but is still developing tolerance for abstract symbol manipulation
(brackets, colons, semicolons). So we always:

- Show a **picture or animation** of the concept before writing any code.
- Use **drag-and-drop blocks** ([Scratch](https://scratch.mit.edu) /
  [Blockly](https://blockly.games)) before raw Python where it makes sense.
- Translate Python errors into **English sentences** with the kid the first
  20 times.
- Reach for **physical metaphors**: variables = labeled boxes, functions =
  recipes, lists = a row of lockers, dictionaries = a class register.

This is also why the curriculum leans heavily on:

- [**StatQuest with Josh Starmer**](https://www.youtube.com/@statquest) —
  for stats and ML, with the friendliest visualizations on the internet.
- [**3Blue1Brown**](https://www.youtube.com/@3blue1brown) — for math
  intuition (some episodes are too advanced; we cherry-pick).
- [**Code.org**](https://studio.code.org/courses),
  [**Scratch**](https://scratch.mit.edu),
  [**Brilliant.org**](https://brilliant.org) — for interactive visual thinking.
- [**Teachable Machine**](https://teachablemachine.withgoogle.com) — for ML
  without code.

Full list with direct links in [`resources.md`](./resources.md).

---

## 4. The three platforms we *live* on

We deliberately keep the tool count small so the kid develops fluency, not
tab-confusion.

| Platform                                                         | What we use it for                                | When introduced |
|------------------------------------------------------------------|---------------------------------------------------|-----------------|
| [**Replit**](https://replit.com) (in browser)                    | Writing & running Python from day one             | Phase 2         |
| [**Google Colab**](https://colab.research.google.com)            | Notebooks, pandas, plots, ML (no install pain)    | Phase 5         |
| **A notebook + pen**                                             | Sketching ideas, drawing data flow, taking notes  | Phase 1         |

That's it. Everything else (Scratch, Brilliant, Khan, YouTube) is a
*visit*, not a home.

---

## 5. Critical thinking is the spine

The user (parent) specifically asked for **critical problem solving on
coding platforms**. We treat that as a separate muscle from "learning
Python syntax". So we train it explicitly:

- In **Phase 3**, every session ends with **2 problems on
  [CodingBat](https://codingbat.com/python) or
  [Edabit](https://edabit.com)**, chosen by difficulty, not topic.
- We follow a fixed **"Solve, then Explain, then Optimize"** pattern (the
  STO loop) for every problem:
  1. **Solve** — get *any* working answer, even ugly.
  2. **Explain** — narrate your code line by line to the parent.
  3. **Optimize** — can it be shorter, faster, or clearer? Rewrite it.
- Problems are kept in a personal **`solved/`** folder with one-line notes:
  *"What did I learn from this one?"*

This is also great preparation for school olympiads
([Bebras](https://www.bebraschallenge.org), IOI Junior, etc.) if the kid
is interested later.

---

## 6. Safety, screen-time, and AI use

- All platforms used are kid-safe and widely vetted.
- Sessions are capped at **60 min** plus a 5-min explain-back; longer
  doesn't help retention at this age.
- **AI tools ([ChatGPT](https://chat.openai.com),
  [Cursor](https://cursor.com), etc.) are introduced only in Phase 5**, and
  used as a *tutor*, never as a code generator the kid pastes from.
  The rule: *"You may ask the AI to explain, never to do."* The parent
  supervises AI sessions until the habit is solid.

---

## 7. How we know it's working

After every phase, the kid should be able to do the phase's **Exit Ticket**
without help. If they can't, we don't move on — we revisit the weakest beat
(usually it's "Build" because we skipped "Play").

There's also a **Progress Tracker** in [`progress-tracker.md`](./progress-tracker.md)
with checkboxes per phase and a reflection prompt per week. Fill it in
together — the kid checks the boxes; the parent jots two lines about what
they noticed.

---

## 8. What we are *not* doing (on purpose)

- ❌ No HTML / CSS / web dev. Different skill tree, can come later.
- ❌ No competitive programming grind. We touch problem-solving, we don't
  drown in it.
- ❌ No deep math derivations. Calculus / linear algebra come later if the
  kid pursues DS seriously in high school.
- ❌ No "let's build a full app". The point is *thinking with data*, not
  shipping software.

Keeping the scope tight is what makes this finishable.

---

Next: [`phase-1-foundation.md`](./phase-1-foundation.md) — *Think like a
computer (no syntax yet).*
