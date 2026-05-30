# Phase 6 — Machine Learning (Kid-Friendly)

> **Duration:** ~6–8 weeks (≈ 20 sessions)
> **Goal:** Demystify "AI". The kid trains, evaluates, and *explains* simple
> ML models — first with no code (Teachable Machine), then with
> scikit-learn — and develops a healthy, critical view of what ML really is.

---

## Why this phase exists

Every kid hears "AI" and "ML" constantly today. Most of them think it's
magic. This phase replaces the magic with a clean, simple, *correct*
mental model:

> **"ML is just finding patterns in past data so we can guess about new
> data — and it's always, sometimes, wrong."**

We aim for the kid to:

- Train a model and see it succeed.
- Train a model and see it *fail* — and understand why.
- Develop healthy skepticism about AI hype.

We do **not** aim for the kid to learn the math behind ML algorithms.
That's high-school + work. We aim for the *intuition* + *the workflow*.

---

## The big mental model

```
       ┌────────────┐       ┌────────────┐       ┌──────────────┐
       │  training  │ ───▶  │   model    │ ◀───  │   new        │
       │   data     │       │   learns   │       │   data       │
       │ (examples) │       │ a pattern  │       │ (to predict) │
       └────────────┘       └─────┬──────┘       └──────────────┘
                                  ▼
                          ┌────────────────┐
                          │   prediction   │
                          └────────────────┘
```

Three kinds of ML we touch:

| Type             | Plain-English question                            | Example                       |
|------------------|----------------------------------------------------|-------------------------------|
| **Classification** | "Which *category* does this belong to?"         | Is this a cat or a dog?       |
| **Regression**     | "What *number* will it be?"                     | What price will this house sell for? |
| **Clustering**     | "Which things are *similar* to each other?"     | Group customers by behavior   |

That's it. Everything else (deep learning, GANs, transformers, RL) we
acknowledge by name and *defer*.

---

## Watch (videos & visual demos)

### The spine: **StatQuest with Josh Starmer — "Machine Learning Basics"**

Watch in order, one per session, with notebook open:

1. *"Machine Learning Fundamentals: Cross Validation"* — overview of the
   whole training/testing idea. (6 min)
2. *"The Confusion Matrix"* (7 min)
3. *"Sensitivity and Specificity"* (11 min — slow this one down)
4. *"Bias and Variance"* (7 min)
5. *"Decision Trees Clearly Explained!!!"* (17 min)
6. *"Random Forests Clearly Explained!!!"* (10 min)
7. *"K-Nearest Neighbors (KNN) Clearly Explained!"* (6 min)
8. *"K-means clustering"* (9 min)
9. *"Linear Regression, Clearly Explained!"* (27 min — split over 2 sessions)
10. *"Logistic Regression, Clearly Explained!"* (9 min)

If StatQuest feels like too much for one beat, *cut, don't extend*.

### Supporting clips

| Topic                              | Channel / Video                                                | Length |
|------------------------------------|----------------------------------------------------------------|--------|
| What is ML, intuitively?           | CGP Grey — *"How Machines Learn"*                              | 8 min  |
| What is a neural network? (intuition only) | 3Blue1Brown — *"But what is a neural network?"* — first 8 min | 8 min  |
| Bias in AI                         | TED — *"How I'm fighting bias in algorithms"* (Joy Buolamwini) | 9 min  |
| AI gone wrong                      | Two Minute Papers — pick a recent "AI fails" episode           | 5 min  |
| Why we split train / test          | Data School — *"What is overfitting?"*                         | 6 min  |
| Ethics of AI for kids              | Code.org / Common Sense Media — *"AI ethics for tweens"*       | 6 min  |

### Optional, weekend

- **Computerphile**: *"How AlphaGo Beat the World Champion"*.
- **Veritasium**: *"The most important algorithm ever"*.

---

## Play — *no-code first*

### Week 1–2: Google's **Teachable Machine** (teachablemachine.withgoogle.com)

This is *the* perfect first ML experience. The kid:

- Trains an **image classifier** on their *own* webcam:
  *"Thumbs up" vs "thumbs down" vs "peace sign"*.
- Trains an **audio classifier**:
  *"clap" vs "snap" vs "silence"*.
- Watches the **confidence meter** wiggle in real time.
- Deliberately tries to *break* the model (wear sunglasses, change
  lighting) and discovers **bias / robustness** by themselves.

Required experiments (do all):

1. Train a 3-class image model with 30 examples per class. Test it.
2. Retrain with **only 5 examples per class**. Watch it get worse.
3. Train it in a bright room; test in a dark room. Watch it fail.
4. Train it with *only the kid's own face*. Test with a sibling. Discuss
   bias.

These four little experiments teach more about ML than any textbook.

### Week 3–4: **scikit-learn intro in Colab**

Now we move from "magic box" to "Python code". Three core notebooks:

#### Notebook A — Iris classifier
- Load the classic Iris dataset (`sklearn.datasets.load_iris`).
- Plot petal length vs petal width with color = species.
- Train a `DecisionTreeClassifier`.
- Split train/test (the kid manually splits 80/20 first, then learns
  `train_test_split`).
- Look at accuracy. Look at confusion matrix.
- *Visualize* the decision tree (`sklearn.tree.plot_tree`) — beautiful,
  intuitive.

#### Notebook B — Penguins KNN
- Same workflow with K-Nearest Neighbors on the Palmer Penguins dataset.
- Vary `k`. Watch how the boundary changes (use a 2D feature plot).
- Introduce the idea of a **hyperparameter**.

#### Notebook C — Linear regression
- Use a small *housing* or *cars-price* dataset.
- Predict price from one feature first, then several.
- Plot the prediction line over the scatter.
- Look at *residuals* (errors) — discuss "the model is always a little
  wrong".

### Week 5–6: Apply to *their own data*

- Re-open the Phase-5 capstone dataset.
- Pick one prediction question.
- Try **two different models**, compare them.
- Discuss: *which is better, and how do we know?*

### Week 7–8: A tiny taste of clustering + a deployed app

- **Clustering**: `KMeans` on the penguins or Spotify dataset; see the
  groups the algorithm finds without being told the labels.
- **Deployment** (optional, exciting): take one model and put it behind
  a **Streamlit** mini-app, in Colab or on streamlit.io. The kid types
  values into a web form and gets a prediction. *Their* model, on the
  internet. Massive motivational payoff.

---

## Build (mini-projects)

| Week | Project                                              | Concepts                          |
|------|------------------------------------------------------|-----------------------------------|
| 1    | Teachable Machine: rock-paper-scissors classifier    | Train / test, confidence          |
| 2    | Teachable Machine: "is the cat in the room?" audio   | Real-world ML, bias               |
| 3    | scikit-learn Iris decision tree                      | First code-based model            |
| 4    | Penguins KNN                                         | Hyperparameters, intuition        |
| 5    | Linear regression on housing                          | Regression, residuals             |
| 6    | Compare 2 models on the kid's Phase-5 dataset        | Model selection, fair comparison  |
| 7    | KMeans clustering on Spotify or penguins             | Unsupervised, "let the data speak" |
| 8    | Streamlit demo app of one of the models               | Sharing your work                 |

---

## Vocabulary to own (and explain)

By end of phase, the kid can define, in their own words:

- **Features** vs **labels**
- **Training set** vs **test set** (and *why* we hold one out)
- **Overfitting** ("memorizing instead of learning")
- **Underfitting** ("too lazy")
- **Accuracy**, **confusion matrix**, **precision/recall** (intuition only)
- **Hyperparameter**
- **Bias** — both the statistical kind and the *societal* kind
- **Supervised** vs **unsupervised** learning

We make a "ML Glossary" markdown cell in their notebooks and grow it as
words appear.

---

## The ethics beat (mandatory, not optional)

Once in the phase — ideally after Teachable Machine — we have a 30-minute
"AI Ethics" conversation. Anchored by:

- The "lighting / sunglasses" failure they discovered.
- The Joy Buolamwini TED talk.
- One news story of an AI mistake (changes monthly; pick a current one).

Discussion prompts:

- Who decides what data goes into a model?
- What happens if the data is *unfair* (only one kind of face, only one
  language)?
- Is it *always* good to use AI? When might it not be?
- "If an AI gets something wrong, who is responsible?"

This is non-negotiable. Kids who grow up with ML need ethics literacy
from day one.

---

## Explain back (checkpoints)

- After every model the kid trains, they must say out loud:
  - *"This is what it learned."*
  - *"This is what it got wrong."*
  - *"This is **why** I think it got that wrong."*
- End of phase: kid does a **10-minute family presentation**:
  *"What machine learning actually is, in 10 minutes, no jargon."*

---

## Exit ticket

Before moving to Phase 7, the kid must:

1. ✅ Train a model **from scratch** on a dataset they've never used,
   using `train_test_split`, fit, predict, and evaluate.
2. ✅ Explain a **confusion matrix** in their own words.
3. ✅ Explain **overfitting** with their own analogy (no copying Josh).
4. ✅ Identify when ML is *the wrong tool* for a problem (yes, this is
   a real skill, and a kid who has it is rare).
5. ✅ Articulate one **ethical concern** about AI in society.

---

Next: [`phase-7-capstone.md`](./phase-7-capstone.md) — *Put it all
together and tell a story.*
