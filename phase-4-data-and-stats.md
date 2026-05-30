# Phase 4 — Data & Statistics Foundations

> **Duration:** ~3–4 weeks (≈ 10 sessions)
> **Goal:** Build intuition for what *data* is and what numbers like
> average, spread, and probability actually mean — through pictures, not
> formulas. This is the on-ramp to "real" data science.

---

## Why this phase exists

If we go straight from Python to pandas, the kid will know *how* to compute
a mean — but not *why* a mean is interesting, when it lies, or what to
draw next. This phase gives them the **statistical common sense** that
makes Phase 5 click.

We deliberately keep it short and visual. There is **no calculus**, **no
sigma notation**, **no formal proofs**. Everything is shown as a picture or
explored with a slider.

---

## What we're learning

| Block                  | Topics                                                                 |
|------------------------|------------------------------------------------------------------------|
| **What is data?**      | Records, fields, rows vs columns, categorical vs numerical             |
| **Summarizing**        | Mean, median, mode — and *when each one lies*                          |
| **Spread**             | Range, "middle 50%" (IQR), variance & std-dev (intuition only)         |
| **Charts**             | Bar, histogram, line, scatter — *which chart for which question*       |
| **Outliers**           | What they are, why they matter, when to keep/drop them                 |
| **Probability (gentle)** | Coin flips, dice, "law of large numbers" simulated in Python         |
| **Correlation ≠ causation** | The single most important sentence in data science             |
| **Lying with charts**  | Truncated axes, cherry-picking, misleading scales                      |

---

## Watch — this phase is *heavy* on videos (parent's stated preference)

This is the most video-friendly phase of the curriculum. We use it.

### The spine: [**StatQuest with Josh Starmer**](https://www.youtube.com/@statquest)

StatQuest is, by a wide margin, the friendliest, most visual stats channel
on the internet. The "Statistics Fundamentals" playlist is the spine — watch them in order, **one per session**:

| # | Video | Length |
|---|-------|--------|
| 1 | [*"Histograms, Clearly Explained"*](https://www.youtube.com/watch?v=qBigTkBLU6g)                                    | 3 min  |
| 2 | [*"The Mean, Variance and Standard Deviation, Clearly Explained!"*](https://www.youtube.com/watch?v=SzZ6GpcfoQY)    | 14 min |
| 3 | [*"The Median, In 1 Minute"*](https://www.youtube.com/results?search_query=statquest+median+in+1+minute)            | 1 min  |
| 4 | [*"Percentiles and Quantiles, Clearly Explained!!!"*](https://www.youtube.com/watch?v=IFKQLDmRK0Y)                  | 6 min  |
| 5 | [*"Boxplots, Clearly Explained"*](https://www.youtube.com/watch?v=fHLhBnmwUM0)                                      | 5 min  |
| 6 | [*"The Normal Distribution, Clearly Explained!!!"*](https://www.youtube.com/watch?v=rzFX5NWojp0)                    | 5 min  |
| 7 | [*"Probability is not Likelihood. Find out why!!!"*](https://www.youtube.com/watch?v=pYxNSUDSFH4) — intuition only  | 5 min  |
| 8 | [*"Pearson's Correlation, Clearly Explained!!!"*](https://www.youtube.com/watch?v=xZ_z8KWkhXE)                      | 8 min  |

### Supporting videos

| Topic                                | Channel / Video                                                                                                                              | Length |
|--------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------|--------|
| What is data?                        | TED-Ed — [*"What's all that data about you?"*](https://www.youtube.com/results?search_query=ted-ed+what%27s+all+that+data+about+you)         | 5 min  |
| Why averages can mislead             | Veritasium — [*"Simpson's Paradox"*](https://www.youtube.com/watch?v=ebEkn-BiW5k)                                                            | 8 min  |
| The Law of Large Numbers (visualized)| 3Blue1Brown — [*"Probabilities of probabilities"*](https://www.youtube.com/watch?v=8idr1WZ1A7Q) (first 5 min)                                | 5 min  |
| Lying with charts                    | Vox — [*"The most misleading charts of 2015, fixed"*](https://www.youtube.com/watch?v=E91bGT9BjYk)                                            | 6 min  |
| Correlation ≠ causation              | TED-Ed — [*"Why correlation doesn't imply causation"*](https://www.youtube.com/results?search_query=ted-ed+correlation+causation)             | 4 min  |
| What a histogram actually shows      | StatQuest — [*"Histograms"* (rewatch)](https://www.youtube.com/watch?v=qBigTkBLU6g)                                                          | 3 min  |

### Bonus, weekend watching

- [**Hans Rosling — "200 Countries, 200 Years, 4 Minutes"** (BBC)](https://www.youtube.com/watch?v=jbkSRLYSojo). Hands-down the most inspiring data-storytelling clip ever filmed.
- [**Gapminder Tools**](https://www.gapminder.org/tools) — let the kid press play on a few topics that interest them.

---

## Play (interactive platforms)

### Primary — [**Google Sheets**](https://sheets.google.com)

Yes, really. Sheets are the kid-friendliest data tool on Earth: every cell
is visible, every formula is editable, charts appear with two clicks.

Mini-lessons in Sheets:

1. **Load a CSV** of countries' populations. Sort. Filter. *Done.*
2. **Compute by formula**: `=AVERAGE`, `=MEDIAN`, `=COUNTIF`, `=SUMIF`.
3. **Insert chart** → choose between bar, line, scatter, histogram for
   the same data; *discuss* which one helps and which one misleads.
4. **Conditional formatting** — heatmaps without code.

We'll be *moving away* from Sheets into pandas in Phase 5 — but the kid
will forever benefit from having the spreadsheet mental model first.
("Pandas is just Sheets that you talk to in code.")

### Secondary — [**Brilliant.org**](https://brilliant.org)

The [**Probability Fundamentals**](https://brilliant.org/courses/probability-fundamentals/) and
[**Statistics Fundamentals**](https://brilliant.org/courses/statistics/) courses are visual, interactive, and perfectly age-appropriate. If you have access (free trial works), this is excellent.

### Tertiary — [**Desmos**](https://www.desmos.com/calculator) & [**GeoGebra**](https://www.geogebra.org)

Use the [**Desmos statistics calculator**](https://www.desmos.com/calculator) to drop in 20 numbers and see
the mean / median / IQR / boxplot update *as you drag points*. Magical.

### Code-side play — *first* Python data work

In the *last two sessions* of this phase, the kid writes small Python
programs (in Replit, still no Jupyter yet) that:

- Read a list of test scores → print mean, median, max, min.
- Simulate 10,000 coin flips with `random` → plot heads-percent over time
  using `matplotlib`'s simplest API (intro only — full pandas/plots come
  in Phase 5).
- Simulate 10,000 dice rolls → print frequency of each outcome (Counter!).

These programs deliberately reuse the **Counter / Accumulator** patterns
from Phase 3, so the kid feels the two phases connecting.

---

## Build (mini-projects)

| Session(s) | Project                                                          | Concepts             |
|------------|------------------------------------------------------------------|----------------------|
| 1          | **"All About Me" dataset** — kid lists 30 friends/family/pets with age, height, favorite food in Sheets | What is data           |
| 2          | **Average vs median fight** — find/construct one dataset where they differ wildly; explain why | Mean lies, median doesn't |
| 3          | **Class marks analysis** — fake or real test scores: chart + write 3 observations | Histograms, summarizing |
| 4          | **Weather chart** — load a month of local weather from a free CSV; chart it; spot the outliers | Charts, outliers       |
| 5          | **Coin-flip simulator** in Python                                | Probability + code     |
| 6          | **Lying-with-charts challenge** — kid creates *two* charts of the same data: one honest, one misleading | Chart literacy   |
| 7          | **Gapminder tour** — pick 3 countries, write a 1-paragraph story comparing them using [Gapminder](https://www.gapminder.org/tools) | Storytelling with data |
| 8          | **Mini-report** (1-page Google Doc) summarizing any dataset of choice: question → chart → finding | Putting it together   |

---

## Critical-thinking spice

Keep doing **1 CodingBat / Edabit problem at the start of each session** —
just to keep the Phase-3 muscle warm. This is the only way fluency
survives.

Also: at least once this phase, do a **"chart autopsy"** — find a real
chart in a newspaper or on social media, and analyze together:
*What's the question? What does the chart say? What does it leave out?
Could it mislead?* This habit pays off for life.

---

## Explain back (checkpoints)

- After the median session, kid explains: *"When does the average lie?
  Give a story."*
- After the correlation session, kid explains *with their own example*
  why "ice-cream sales and shark attacks rise together" doesn't mean ice
  cream attracts sharks.
- End of phase: kid gives a **3-minute presentation** of their mini-report
  to the family — chart on screen, three observations, one question they
  *still* have.

---

## Exit ticket

Before moving to Phase 5, the kid must:

1. ✅ Look at a small dataset and choose the **right chart** for a given
   question (and defend the choice).
2. ✅ Explain the **difference between mean and median**, and produce a
   small example where they disagree.
3. ✅ Spot at least **two ways a chart can mislead** without help.
4. ✅ State **"correlation is not causation"** *and* give their own
   example of why.
5. ✅ Have a Google Sheets file with one analyzed dataset, charted, and
   summarized in writing.

---

Next: [`phase-5-data-science.md`](./phase-5-data-science.md) — *Now we put
Python and data together. Welcome to the real thing.*
