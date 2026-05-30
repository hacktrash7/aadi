# Phase 7 — Capstone: One Real Project, Told Beautifully

> **Duration:** ~4 weeks (≈ 12 sessions)
> **Goal:** The kid picks **one** problem they actually care about,
> takes it through the full data-science pipeline, builds a working
> artifact, and presents it like a TED talk. This is the project they
> will *show people* for years.

---

## Why this phase exists

Phases 1–6 are training. Phase 7 is **performance**. It exists for three
reasons:

1. **Consolidation.** Doing one big thing forces every prior skill to
   re-surface. Gaps become visible — and fixable.
2. **Ownership.** The kid chose this. It's theirs. That's a different
   kind of motivation than any tutorial.
3. **Communication.** Data science *unshared* is data science wasted.
   This phase trains the storytelling muscle that matters more than
   syntax.

---

## What the capstone is

**One project, with three deliverables:**

1. A **[Colab](https://colab.research.google.com) notebook** — the
   technical artifact, well-commented, with markdown narrative throughout.
2. A **5-slide presentation** ([Google Slides](https://slides.google.com)
   or [Canva](https://www.canva.com)) — the human-friendly version.
3. A **5-minute screen-recorded video** ([Loom](https://www.loom.com) or
   [OBS Studio](https://obsproject.com)) — the kid presenting their work
   like [Hans Rosling](https://www.youtube.com/watch?v=jbkSRLYSojo): with energy and clarity.

That's it. We don't add anything else (like a website or a paper) —
adding more dilutes the focus.

---

## Inspiration to rewatch before starting

| Watch this | Why |
|-----------|-----|
| Hans Rosling — [*"200 Countries, 200 Years, 4 Minutes"*](https://www.youtube.com/watch?v=jbkSRLYSojo) | The gold standard of data storytelling. Energy + clarity. |
| Hans Rosling — [*"The best stats you've ever seen"* (TED)](https://www.ted.com/talks/hans_rosling_the_best_stats_you_ve_ever_seen) | The full 20-min version. Watch *how* he tells the story. |
| Keith Galli — [*"Solving real-world data science tasks with Pandas"*](https://www.youtube.com/watch?v=eMOA1pPVUc4) | A great worked Kaggle walkthrough. Watch for *structure*, not to copy. |

---

## How to pick the topic

The kid picks. The parent's job is only to **veto unrealistic scope**
(politely).

### Good topic shapes

- *"Which features make a Pokémon win battles?"*
- *"How has IPL batting changed over 15 years?"*
- *"What's the best time to release a song on Spotify?"*
- *"Can I predict tomorrow's temperature in my city from this week?"*
- *"What makes a Disney movie score highly on IMDB?"*
- *"Are there really distinct 'kinds' of cricketers, or is it a spectrum?"*

### Topic vibes that work

- Something the kid **already enjoys** outside of code (sports, music,
  games, movies, animals, weather).
- A dataset that **exists** on [Kaggle](https://www.kaggle.com/datasets)
  or a free source — we are not scraping the web yet.
- A question **you can answer with charts** — not a yes/no debate.

### Red flags (the parent should gently redirect)

- "I'll build a chatbot" — too vague, scope explodes.
- "I'll predict the stock market" — even adults can't.
- "I'll build a self-driving car." — yeah, no.
- "I'll use 5 different datasets" — pick one. *Always* one.

---

## The capstone timeline (4 weeks)

### Week 1 — Question & Data

| Session | Activity                                                                 |
|---------|--------------------------------------------------------------------------|
| 1       | Brainstorm: 10 possible questions. Pick top 3. Sleep on it.              |
| 2       | Pick the final question. Write it on top of the notebook in big letters.|
| 3       | Find the dataset(s). Inspect (`head/info/describe`). Sketch the plan.   |

### Week 2 — Clean & Explore

| Session | Activity                                                                 |
|---------|--------------------------------------------------------------------------|
| 4       | Clean: missing values, weird types, rename columns. Document it.         |
| 5       | First charts. Three of them. Write down what you notice.                |
| 6       | Refine question if needed (this is *good* science, not "cheating").     |

### Week 3 — Model (optional) & Polish

| Session | Activity                                                                 |
|---------|--------------------------------------------------------------------------|
| 7       | If the question needs prediction, train **one** simple ML model.        |
| 8       | Compare result against a "dumb baseline" (average / most-common-class). |
| 9       | Final round of charts. Title, axis labels, color. Make them beautiful.  |

### Week 4 — Present

| Session | Activity                                                                 |
|---------|--------------------------------------------------------------------------|
| 10      | Write the *story*: 5 markdown cells in the notebook, one per slide.     |
| 11      | Build 5 slides ([Google Slides](https://slides.google.com), [Canva](https://www.canva.com), or Keynote). Practice once. |
| 12      | Record the 5-min video. Watch it. Re-record once if needed. **Ship it.**|

---

## The 5-slide structure (Hans Rosling style)

1. **The Question.**
   *"I wanted to know: \_\_\_\_\_\_\_\_\_."* — one sentence. Big font.
2. **The Data.**
   *"I used this dataset, with this many rows and these columns."*
   One screenshot of `df.head()`.
3. **What I Found (1).**
   Best chart in the notebook. One sentence of insight beneath it.
4. **What I Found (2).**
   Second-best chart + insight.
5. **So What?**
   *"What this means is…"* + one *honest* limitation + one *open*
   question the kid still has.

That last slide — the "limitations + open questions" — is what
separates a kid who's been *taught* data science from a kid who *gets*
it. We make a big deal of it.

---

## Recording the video

Tools (pick any):

- [**Loom**](https://www.loom.com) — easiest, free, browser-based.
- [**OBS Studio**](https://obsproject.com) — free, slightly more setup, professional output.
- **Phone propped on books** — pointed at the screen. Charmingly low-fi.

Guidelines:

- 5 minutes, hard cap.
- Kid on camera (small webcam circle) **plus** screen.
- One take, mistakes and all. We're not editing.
- Energy > polish. *Excitement is the point.*

Show it to grandparents. Post it (privately) to a family group. Save it
forever. In two years the kid will rewatch and laugh — and notice how
much they've grown.

---

## Three example capstone shapes (pick one feel)

### Shape A — "Insight" project (analysis only)
> *"What makes a Disney movie a hit?"*
- No ML, just pandas + charts.
- Outcome: 3–5 strong insights.
- Easiest to scope.

### Shape B — "Prediction" project (light ML)
> *"Can I guess a Pokémon's win-rate from its stats?"*
- pandas + one ML model.
- Outcome: a model that beats a dumb baseline by *some* margin.

### Shape C — "Tool" project (light ML + deployment)
> *"A [Streamlit](https://streamlit.io) app that predicts which IPL team will win a match."*
- pandas + one ML model + Streamlit.
- Outcome: a working web app. Maximum "wow" factor.

Most kids will (and should) pick Shape A or B. Shape C is for the kid
who is *flying*.

---

## Grading rubric (only for the parent's eye)

Not for the kid — but the parent should privately check these. If 4 of
the 5 are 👍, ship it.

1. **Question is clear and answerable.** 👍/👎
2. **Notebook tells a story top-to-bottom, with markdown.** 👍/👎
3. **At least 3 well-labeled, honest charts.** 👍/👎
4. **Kid can defend every line of code if asked.** 👍/👎
5. **Slide 5 contains a real limitation + open question.** 👍/👎

If anything misses, **don't lower the score** — just have a session to
fix that specific thing. Standards are met by iteration, not by mercy.

---

## After the capstone — "what's next?"

Have a casual conversation. Possible paths:

- **More depth in DS:** harder [Kaggle](https://www.kaggle.com/competitions) datasets, intermediate ML
  ([XGBoost](https://xgboost.readthedocs.io)), pandas advanced features.
- **Math depth:** [Brilliant.org "Statistics II"](https://brilliant.org/courses/statistics/),
  [Khan Academy Algebra II](https://www.khanacademy.org/math/algebra2) → eventually calculus when school catches up.
- **Computer-science depth:** intro to algorithms via [USACO Guide
  Bronze](https://usaco.guide/), [CS50x lectures](https://cs50.harvard.edu/x/)
  (these are advanced but kid-friendly enough).
- **Web side-quest:** if the kid wants to *deploy* their work properly,
  a short HTML/CSS/JS + Streamlit deeper dive.
- **Just rest:** play more video games. Read more books. Touch grass.
  Burnout at 12 is real. The next phase can wait six months. The
  curriculum is not the goal — *the curious thinker* is.

---

## Exit ticket — for the entire curriculum

By the end of the capstone, the kid should be able to:

1. ✅ Open a brand-new CSV they've never seen, load it in [Colab](https://colab.research.google.com), ask
   three interesting questions, and answer them with charts.
2. ✅ Train a simple ML model on it and explain what it learned, what
   it got wrong, and why.
3. ✅ Sit a relative down and present any of their projects for 10
   minutes — confidently, in their own words, without jargon.
4. ✅ Recognize when a chart or claim on the internet is *misleading*.
5. ✅ Look at a new problem and know whether DS / ML is the right tool
   for it.

If those five are true — *we did it*. The 6th-grader has crossed the
bridge from "no coding" to "thinking like a data scientist".

Everything from here is depth, not direction.

---

Next: [`resources.md`](./resources.md) — the master list of videos,
channels, platforms, and books referenced across all phases.
