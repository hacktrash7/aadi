# Weekly Plan — What a Normal Week Looks Like

The curriculum has 7 phases, but the kid lives in **weeks**, not phases.
This doc shows what a typical week looks like in practice — so the parent
never has to wonder *"what do we do today?"*

---

## The baseline schedule

> **3 sessions per week × 45–60 minutes each.**
> Plus an *optional* 30–60 min weekend "tinker time".

That's it. Resist the urge to add more. Consistency beats intensity at
this age by a wide margin.

```
   MON      TUE      WED      THU      FRI      SAT      SUN
 ┌────┐   ┌────┐   ┌────┐   ┌────┐   ┌────┐   ┌────────────┐
 │ ✦  │   │    │   │ ✦  │   │    │   │ ✦  │   │ tinker /   │
 │NEW │   │rest│   │PRAC│   │rest│   │SHOW│   │ rest /     │
 │idea│   │    │   │tice│   │    │   │ &  │   │ catch up   │
 │    │   │    │   │    │   │    │   │tell│   │            │
 └────┘   └────┘   └────┘   └────┘   └────┘   └────────────┘
```

Pick three weekdays — any three — and stick to them. The day-names above
are illustrative.

---

## The three session types

We deliberately give each session a *personality*. Same kid, same week,
but different energy.

### Type A — "NEW IDEA" session (Monday-ish)

The session that introduces a concept.

| Beat            | Time    | Activity                                  |
|-----------------|---------|-------------------------------------------|
| Hook            | 2 min   | A question, meme, magic trick.            |
| Watch           | 5–10 min| One short video (see phase doc).          |
| Play            | 15–20 min | Interactive platform exploring the idea. |
| Build           | 15–20 min | Tiny project applying the idea.          |
| Explain back    | 5 min   | Kid teaches it to parent.                 |

This session is **low-stakes and curious**. We're not grading. We're
playing with a new toy.

### Type B — "PRACTICE" session (Wednesday-ish)

The session that builds fluency.

| Beat            | Time    | Activity                                  |
|-----------------|---------|-------------------------------------------|
| Warm-up         | 5 min   | 1 small CodingBat/Edabit problem.         |
| Project work    | 30–40 min | Continue the week's main project.        |
| Stuck-list      | 5 min   | Write down 1–3 things that got tricky.    |
| Explain back    | 5 min   | Kid narrates *progress*, not "what".      |

This session is **about reps**. No new ideas. We get *good* at what we
already half-know.

### Type C — "SHOW & TELL" session (Friday-ish)

The session that consolidates and celebrates.

| Beat            | Time    | Activity                                  |
|-----------------|---------|-------------------------------------------|
| Polish          | 15 min  | Finish / clean up the week's project.     |
| Mini-demo       | 5 min   | Kid demos the project to a parent / sibling. |
| Reflect         | 5 min   | Update `progress-tracker.md`: 1 line.     |
| Plan ahead      | 5 min   | Kid picks something to look up / try next week. |
| Free tinker     | 15+ min | *Anything* code-adjacent the kid wants.   |

This session is **about ownership and pride**. The kid leaves the week
feeling like they *finished* something.

---

## Optional — weekend "tinker time"

If (and only if) the kid asks. Things that fit naturally:

- **Scratch / CodeCombat** open-ended play.
- A Kaggle dataset they're curious about.
- A YouTube DS / ML "wow" video from the resources list.
- One Brilliant.org or Bebras puzzle.
- **Teach a younger sibling/cousin** something they learned (this works
  *miracles* for retention).

**Forbidden** on the weekend: forced curriculum. If they don't feel like
it, they don't do it. Curiosity is a renewable resource — don't burn it.

---

## A sample week from each phase

### Phase 1 (Foundation) — example week 2

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Watch Code.org "What is a loop?" → do 10 Code.org Course D maze puzzles |
| Wed | PRAC | Build "Catch the Apples" in Scratch (variables + loops + ifs) |
| Fri | SHOW | Finish & demo "Catch the Apples" to parent; record a 30-sec phone video |

### Phase 2 (Python Basics) — example week 4

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Watch Corey Schafer on lists → 3 small list exercises in Replit |
| Wed | PRAC | 1 CodingBat warm-up → build "To-Do List CLI" in Replit |
| Fri | SHOW | Finish To-Do List, walk parent through the code line by line |

### Phase 3 (Problem Solving) — example week 5

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Introduce the **Sort & Extremes** pattern; 1 worked example |
| Wed | PRAC | STO loop on 3 CodingBat List-2 problems + 2 Edabit Easy |
| Fri | SHOW | Pick the favorite solved problem; kid teaches the pattern back |

### Phase 4 (Data & Stats) — example week 2

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Watch StatQuest "Mean, Variance, SD" → drag points in Desmos stats |
| Wed | PRAC | In Sheets: load class-marks CSV, compute mean/median/SD, chart it |
| Fri | SHOW | "Average vs median fight" — kid presents one dataset where they disagree |

### Phase 5 (Data Science) — example week 6

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Watch Corey on `.groupby` → try one groupby on the Spotify dataset |
| Wed | PRAC | Build the Spotify trends notebook: clean → group → 3 charts |
| Fri | SHOW | 3-min screen-recorded walkthrough of the finished notebook |

### Phase 6 (Machine Learning) — example week 4

| Day | Type | What we do |
|-----|------|------------|
| Mon | NEW  | Watch StatQuest "KNN" → walk through the Penguins KNN notebook setup |
| Wed | PRAC | Train KNN, vary `k`, plot decision boundary, write down what changes |
| Fri | SHOW | Kid explains "what is a hyperparameter" to parent using their plot |

### Phase 7 (Capstone) — week-by-week is already in `phase-7-capstone.md`.

---

## Rhythm rules (to protect motivation)

1. **One concept per session, max.** If a video introduces three things,
   we explicitly *postpone* two.
2. **Always end on a working artifact.** Never close the laptop on a
   broken program. Either fix it or comment-out and `print("WIP")`.
3. **No surprise "extra" sessions.** Three a week. If the kid begs for
   more, say *"let's save it for the weekend tinker."* Scarcity makes
   it feel like a privilege.
4. **Skip a week without guilt** if life is busy. Then resume *exactly*
   where you left off — don't try to "catch up".
5. **Re-do, don't rush.** It is 100% normal to do an entire phase twice
   with different projects. The second pass is where *real* fluency
   lives.

---

## When to slow down

Slow down (revisit prior material) if any of these show up:

- Kid is **guessing** at syntax instead of reasoning.
- Kid is **silent** during "Explain back".
- Kid is **frustrated** three sessions in a row.
- Parent is **doing more than 20%** of the typing.
- Kid says **"I don't know where to start"** repeatedly on new problems.

The right move is *almost never* "push through". The right move is to go
back one phase and do **2 small projects** at that level. Confidence
restored, motivation restored.

---

## When to speed up

Speed up (skip ahead, take on more) only if **all** of these are true:

- The phase's **Exit Ticket** is being met effortlessly.
- The kid is **asking for more** unprompted.
- They're **finishing builds in half the time** allotted.
- They're **exploring outside the curriculum** on their own.

Even then, speeding up means: do the *next* phase, not skip phases.
**Never skip Phase 3** (problem solving) or **Phase 4** (stats), no
matter how shiny ML looks — those phases are the foundation that
prevents bad habits.

---

## Parental energy budget (real talk)

You're going to be present for ~3 hours of focused time a week. Budget it:

- **80%**: just *be there*, ask questions, play dumb during Explain Back.
- **15%**: unblock the kid when they're stuck for more than ~5 minutes.
- **5%**: read the next session's phase doc in advance.

You do **not** need to know Python or data science to do this. The
"Explain back" beat means *the kid* teaches *you*. That's the whole
trick.

---

Next: [`progress-tracker.md`](./progress-tracker.md) — checklists and
reflection prompts to keep momentum.
