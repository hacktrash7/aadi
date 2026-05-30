# Phase 5 — Data Science with Python

> **Duration:** ~8–10 weeks (≈ 25 sessions)
> **Goal:** Load real datasets in Python, ask interesting questions of
> them, and answer those questions with charts and short written
> conclusions. This is the *core* of the curriculum.

---

## Why this phase exists

Everything we've done so far was preparation. Phase 5 is where it pays
off: Python from Phase 2, problem-solving from Phase 3, statistical
common sense from Phase 4 — they all *fuse* the first time the kid runs
`df.head()` on a dataset they actually care about.

The skills here are also the most **transferable** to school: the kid
will be able to do their *own* science-fair / social-studies projects
with actual data, not made-up examples.

---

## The big mental model

```
   ┌────────┐    ┌──────────┐    ┌──────────┐    ┌───────────┐    ┌────────┐
   │  ASK   │ →  │  GET     │ →  │  CLEAN   │ →  │  EXPLORE  │ →  │  TELL  │
   │  a     │    │  the     │    │  the     │    │  the      │    │  the   │
   │question│    │  data    │    │  data    │    │  story    │    │  story │
   └────────┘    └──────────┘    └──────────┘    └───────────┘    └────────┘
```

This is the same pipeline every data scientist on Earth follows. We teach
each stage explicitly. The kid should be able to point to "where they
are" in this pipeline at any moment.

---

## Tools — and *only* these tools

We keep the surface area small. By the end of this phase, the kid will
be fluent in:

| Tool             | What it does                                               |
|------------------|------------------------------------------------------------|
| **Google Colab** | Jupyter notebooks in the browser, no install               |
| **pandas**       | Loading, cleaning, slicing, grouping data                  |
| **matplotlib**   | Quick charts — the basics                                  |
| **seaborn**      | Pretty charts with one line of code                        |
| **numpy** (light) | Vectors of numbers — used implicitly inside pandas        |
| **Kaggle Datasets** | The data buffet — kid-safe, free, huge variety          |

We deliberately **do not** introduce: virtualenvs, pip on the local
machine, plotly dash, requests/APIs, SQL. All of those can come later.

---

## Watch (videos & visual demos)

### The spine: **"Pandas in 60 minutes" (freeCodeCamp / Corey Schafer)**

We watch Corey Schafer's **"Python Pandas Tutorial"** series, but
*one episode every few sessions*, paused liberally. The kid types every
example alongside the video. No passive watching.

### Supporting clips (one per relevant session)

| Topic                              | Channel / Video                                                | Length |
|------------------------------------|----------------------------------------------------------------|--------|
| What is a DataFrame?               | Keith Galli — *"Solving real-world data science tasks with Pandas!"* first 8 min | 8 min |
| Matplotlib intro                   | Corey Schafer — *"Matplotlib Tutorial 1"*                      | 35 min (split into 3 sessions) |
| Seaborn vs Matplotlib              | Data School short                                              | 5 min  |
| EDA mindset                        | StatQuest — *"Exploratory Data Analysis"* (a friendly walk-through) | 12 min |
| Cleaning messy data                | Real Python YouTube — *"Pandas: Clean Your Data"*              | 10 min |
| What is a Jupyter notebook?        | Keith Galli — short                                            | 6 min  |
| Telling a story with data          | TED — Hans Rosling clips (rewatch from Phase 4)                | 5 min  |
| How to read documentation          | mCoding — *"Read the docs!"*                                   | 5 min  |

### Bonus, optional, weekend

- **3Blue1Brown** — *"What's a Tensor?"* (only the first 2 minutes; the
  rest is for high school) — just so the word stops being scary.
- **Computerphile** — *"Big Data"* episode.
- **NetworkChuck / sentdex** — pick *one* short *enthusiastic* video each
  month to keep motivation high. Both are great for kid vibes.

---

## Play (the new playground: Colab)

### Setup, once

- Open [colab.research.google.com](https://colab.research.google.com).
- Sign in with the kid's Google account.
- Create a folder in Drive: `Aadi Data Science/`.
- Every notebook lives there. Name them `01-titanic.ipynb`,
  `02-pokemon.ipynb`, etc. Build a *portfolio*.

### Why Colab over local

- Zero install, runs on any laptop / Chromebook.
- Free GPU later (we won't need it until very late).
- Easy to share — kid can send a link to grandparents.
- Same UI as professional Jupyter, so nothing is "fake".

### Kaggle Datasets — our buffet

The single best repository of kid-friendly, real-world datasets:

- **Pokémon stats** (every kid's gateway dataset)
- **FIFA / NBA / IPL player stats**
- **Disney+ / Netflix titles**
- **Spotify "Top hits"**
- **Penguins / Iris / Palmer Penguins** (smaller, classic)
- **Titanic** (the legendary first ML dataset)
- **Global Happiness Report**
- **World Bank country indicators**
- **Movie reviews / IMDB Top 1000**
- **Weather in Delhi / Mumbai / your city**

We pick datasets the kid *already cares about*. Curiosity is the engine.

---

## Build (one notebook per week, growing in ambition)

Every project follows the **ASK → GET → CLEAN → EXPLORE → TELL** pipeline.
Each notebook ends with:

- A clear question at the top in markdown.
- The cleaned data table.
- At least 3 charts.
- A **"What I learned"** section in markdown — full sentences, not bullets.

| Week | Notebook                              | New ideas introduced                              |
|------|---------------------------------------|---------------------------------------------------|
| 1    | **"Hello, Colab"** — basic cells, markdown, importing pandas, loading a tiny CSV | Notebook UI, markdown, `pd.read_csv` |
| 2    | **Pokémon stats**                     | `df.head/info/describe`, selecting columns, sorting |
| 3    | **Pokémon stats, deeper**             | Filtering rows, `value_counts`, basic `groupby`   |
| 4    | **NBA / IPL players**                 | Multiple groupbys, charts with `df.plot` and seaborn |
| 5    | **Movies dataset**                    | Joining / merging two DataFrames                  |
| 6    | **Spotify top songs**                 | Time / date columns, line charts of trends        |
| 7    | **Penguins**                          | Scatterplots, color-by-category, foreshadowing ML |
| 8    | **Titanic (EDA only)**                | Missing values, cleaning, hypotheses              |
| 9    | **Local weather**                     | Bringing in *your own* CSV (kid chooses city)     |
| 10   | **MINI-CAPSTONE: Kid's own dataset**  | Full pipeline, presented to family                |

The week-10 mini-capstone matters. The kid:

- Picks **a question they care about** ("Which Pokémon type wins most
  battles?", "Did my favorite cricketer get better over the years?",
  "What's the rainiest month in our city?").
- Finds or builds a dataset.
- Goes through the full pipeline.
- Presents to the family with the notebook on screen.

This is *practice* for the actual Capstone in Phase 7.

---

## The pandas mini-syllabus

Taught organically *through projects*, but here's the checklist of skills
the kid should own by end of phase:

### Loading & inspecting
- `pd.read_csv`, `df.head`, `df.tail`, `df.shape`, `df.info`, `df.describe`
- `df.columns`, `df.dtypes`

### Selecting
- `df["col"]`, `df[["col1", "col2"]]`
- Boolean filtering: `df[df["age"] > 10]`
- `.loc` vs `.iloc` (light touch — kid learns one, parent enforces the other)

### Cleaning
- `df.isna().sum()`, `df.dropna()`, `df.fillna(0)`
- `df["col"].astype(int)`
- Renaming columns

### Aggregating
- `df.groupby("type").mean()`
- `df["col"].value_counts()`
- `df.sort_values("col", ascending=False)`

### Charting
- `df.plot(kind="bar"|"line"|"hist"|"scatter")`
- `sns.histplot`, `sns.scatterplot`, `sns.boxplot`, `sns.heatmap`
- Always set: title, x-label, y-label. Always.

### Combining
- `pd.merge` for joins (single example is enough this phase)
- `df.apply` (one example with a small lambda)

> Notice what's *not* in the list: pivot tables, multi-index, complex
> reshape, performance tuning. All of that waits.

---

## AI tools — introduced here, carefully

From Phase 5 onwards, the kid is allowed to use ChatGPT / Cursor / Claude
**as a tutor**, supervised. The rule, posted on the wall:

> **"Ask the AI to *explain*, never to *do*."**

Specifically, the kid may:
- Ask: *"Explain this pandas error in simple words."*
- Ask: *"What does `groupby` actually do?"*
- Ask: *"Give me 3 practice problems on filtering DataFrames."*

The kid may **not** (yet):
- Paste a project prompt and copy the output.
- Ask the AI to "write me a notebook that…"
- Use AI without the parent in the room (for now).

Once the kid demonstrates self-restraint for ~4 weeks, the supervision
relaxes.

---

## Critical-thinking spice

Keep solving **1 problem from CodingBat/Edabit at the start of each
session**. By Phase 5 they should be doing **"Medium"** problems on
Edabit comfortably. We are not letting this muscle atrophy.

---

## Explain back (checkpoints)

- After every notebook, the kid records a **3-minute screen-recorded
  walkthrough** (Loom / OBS / phone) — explaining their question, their
  cleaning steps, their findings. Stored in a folder. By end of phase
  there should be ~8 of these. This is **mandatory** — public-speaking
  practice with data is rare and valuable.
- Friday session = kid demos that week's notebook to the family for 5
  minutes.

---

## Exit ticket

Before moving to Phase 6, the kid must:

1. ✅ Given a **brand-new CSV they've never seen** and a written
   question, produce a clean, well-charted notebook that answers it —
   start to finish — in one 60-minute session.
2. ✅ Fluently use the pandas checklist above without referring to notes
   (looking things up online is fine; that's real-world DS).
3. ✅ Explain, in their own words, the **ASK → GET → CLEAN → EXPLORE →
   TELL** pipeline and which step they find hardest.
4. ✅ Have **8+ notebooks** in their portfolio folder, each with a clear
   question and a "what I learned" section.
5. ✅ Spot at least one **misleading chart** in their *own* old notebooks
   and improve it.

---

Next: [`phase-6-machine-learning.md`](./phase-6-machine-learning.md) — *Now,
the magical part — teaching the computer to learn.*
