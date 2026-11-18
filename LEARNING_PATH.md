# Concept Dependencies & Learning Progress

This file is the readable companion to [CONCEPT_TRACKER.csv](CONCEPT_TRACKER.csv). The CSV is the **editable source of truth** for lesson status, scores, review dates, and notes.

## The learning path

```mermaid
flowchart TD
  A["01 Counting and units"] --> B["02–03 Zero, subtraction, negatives"]
  B --> C["04 Multiplication"]
  C --> D["05–06 Division, fractions, ratios"]
  D --> E["07–09 Sequences, powers, finite sums"]
  E --> F["10–12 Factorials, approximation, proof"]
  D --> G["13–16 Coordinates, distance, circles, turns"]
  G --> H["17–18 Complex numbers, rational rotations"]
  F --> I["19–22 Compounding, e, exponential approximations"]
  H --> J["23–25 Complex growth, trigonometry, Euler experiment"]
  I --> J
  E --> K["26–28 Numerical rates"]
  G --> L["29–30 Numerical area"]
  K --> M["31–32 Accumulation, dynamics"]
  L --> M
  F --> N["33–36 Bounds, convergence, limits, continuity"]
  M --> N
  N --> O["37–38 Exact derivatives and integrals"]
  I --> P["39 Exponential proof"]
  O --> P
  J --> Q["40 Euler identity proof"]
  P --> Q
```

The diagram groups chapters for readability. **Exact prerequisites for each individual lesson are in the CSV.** A chapter can have several prerequisites from different acts, and those are listed by lesson ID.

## How we track progress

| Status | Meaning |
|---|---|
| Not started | We have not studied the lesson |
| Learning | We are actively working through it |
| Practicing | We understand the idea but need independent examples |
| Mastered | We can pass the lesson's mastery check without help |
| Review | Previously mastered, but needs refreshing |

**Mastery scale:** 0 = unseen; 1 = recognize the idea; 2 = follow a worked example; 3 = solve independently; 4 = explain, derive, and apply in a new setting.

**Recommended unlock rule:** Begin a lesson when all its prerequisite lessons have a score of at least **3**. This is a study recommendation, not a mathematical theorem; we may deliberately explore ahead.

## Lesson routine

1. **The scene:** A short castaway episode poses one concrete need.
2. **The notebook:** Record what we already know; calculate a small example.
3. **The invention:** Name the new operation or concept only after constructing it.
4. **The experiment:** Test the idea numerically and track error where possible.
5. **The check:** Solve one fresh problem without prompts.
6. **The ledger:** Record earned tools, observed patterns, and unproved claims.
7. **The tracker:** Update status, score, date, and one sentence of notes in the CSV.

## Example of a dependency

**Lesson 25 — Half a Turn** requires:

- **20:** Numerical approximations to e
- **23:** Complex compounding
- **24:** Numerical trigonometric patterns

It does **not** require limits: at this stage, the goal is to *test* Euler's identity numerically. Its exact proof belongs to Lesson 40, which requires the rigorous material developed later.

## Editorial decision: Story + mathematical notebook

The book uses **two complementary registers**:

**Story:** Brief, concrete, literary, and sometimes playful. A recurring castaway encounters a genuine problem on the island. No lecture disguised as dialogue, and no contrived survival problem merely to introduce a formula.

**Notebook:** Direct and precise. It shows the arithmetic, asks the reader to predict the next result, explains why an operation is needed, and records what is actually established. Numerical evidence is labeled as such.

Each lesson should be short enough to feel like one discovery. The story should never replace the calculation, and the calculation should never arrive before its motivation.

## Future editing

- Edit [ROADMAP.md](ROADMAP.md) to change the book's story and chapter plan.
- Edit [CONCEPT_TRACKER.csv](CONCEPT_TRACKER.csv) to track lesson mastery.
- Update the concept prerequisites whenever chapters are added, removed, or reordered.
- Keep all initial statuses at **Not started** until a mastery check is actually attempted.
