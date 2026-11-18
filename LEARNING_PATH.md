# Concept Dependencies & Learning Progress

This file is the readable companion to [CONCEPT_TRACKER.csv](CONCEPT_TRACKER.csv). The CSV is the **editable source of truth** for lesson status, scores, review dates, and notes. Detailed addition prerequisites live separately in [ADDITION_MASTERY.csv](ADDITION_MASTERY.csv).

## What the castaway remembers

The castaway can **count, add, subtract, multiply, and divide**, including ordinary calculations with fractions. These are remembered procedures, **not yet justified mathematical ideas**. He does not know why the rules work, when they fail, or how to reconstruct them from first principles.

He has scattered memories of school: **sine, cosine, angles, geometry, and linear equations**. He remembers only the words—not a single definition, identity, value, formula, or method. These are narrative clues, not usable mathematical knowledge.

**The challenge is no longer to invent arithmetic without knowing it. It is to justify familiar arithmetic, discover what it can do, and rebuild the forgotten mathematics of change.**

## The addition foundations branch

**The original 40 lessons are chapter milestones, not a complete prerequisite inventory.** Chapter 01 now has a rigorous optional-depth companion, [Interlude 01A](chapters/01a-laws-beneath-the-stones.md), with **20 separately trackable competencies** in [ADDITION_MASTERY.csv](ADDITION_MASTERY.csv). This avoids renumbering every later chapter.

```mermaid
flowchart TD
  A01["A01 Units and bijections"] --> A02["A02 Disjoint union"]
  A01 --> A03["A03 Peano axioms and induction"]
  A03 --> A04["A04 Recursive addition"]
  A04 --> A05["A05 Identity and closure"]
  A05 --> A06["A06 Associativity"]
  A06 --> A07["A07 Commutativity"]
  A04 --> A08["A08 Cancellation"]
  A06 --> A09["A09 Order translation"]
  A02 --> A10["A10 Set-theoretic interpretation"]
  A07 --> A11["A11 Monoids and groups"]
  A08 --> A12["A12 Integer group completion"]
  A11 --> A12
  A12 --> A13["A13 Rationals and reals"]
  A07 --> A14["A14 Multiplication and distributivity"]
  A13 --> A15["A15 Finite and infinite sums"]
  A11 --> A16["A16 Universal property"]
  A10 --> A17["A17 Ordinal/cardinal exceptions"]
  A13 --> A18["A18 Floating point"]
  A16 --> A19["A19 Philosophy of proof"]
  A19 --> A20["A20 Comprehensive defense"]
  A17 --> A20
  A18 --> A20
  A15 --> A20
  A14 --> A20
```

**The diagram shows the main route, not every edge.** The complete, exact per-competency prerequisites are in the addition CSV. Core readiness for Chapter 02: main Lesson 01 plus A01–A02 (units, bijections, disjoint union). The main tracker explicitly lists these cross-tracker prerequisites. A03–A20 are the optional rigorous-depth branch; they become required only for the comprehensive addition-defense milestone. Deep mastery of addition: A01–A20 at score 4. Later chapters can rely on the core route while the foundations branch remains available.

**Important sequence distinction:** The formal interlude deliberately looks ahead to zero, negatives, multiplication, fractions, and limits. It is a **foundations appendix** that proves and classifies familiar ideas; it is not the chronological order in which the castaway discovers them in the main story.

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

**Recommended unlock rule:** Begin a lesson when all its prerequisite lessons and cross-tracker concept IDs have a score of at least **3**. This is a study recommendation, not a mathematical theorem; we may deliberately explore ahead.

## Lesson routine

1. **The scene:** A short castaway episode poses one concrete need, sometimes prompted by a fragment of remembered mathematics.
2. **The notebook:** Use remembered arithmetic, then ask which rules justify the calculation.
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

**Story:** Brief, concrete, literary, and sometimes playful. The castaway remembers arithmetic procedures but cannot explain them; he recalls only the names of trigonometry, geometry, and linear equations, with no associated formulas or facts. A recurring castaway encounters a genuine problem on the island. No lecture disguised as dialogue, and no contrived survival problem merely to introduce a formula.

**Notebook:** Direct and precise. It shows the arithmetic, asks the reader to predict the next result, explains why an operation is needed, and records what is actually established. Numerical evidence is labeled as such.

Each lesson should be short enough to feel like one discovery. The story should never replace the calculation, and the calculation should never arrive before its motivation.

## Future editing

- Edit [ROADMAP.md](ROADMAP.md) to change the book's story and chapter plan.
- Edit [CONCEPT_TRACKER.csv](CONCEPT_TRACKER.csv) to track lesson mastery.
- Update the concept prerequisites whenever chapters are added, removed, or reordered.
- Keep all initial statuses at **Not started** until a mastery check is actually attempted.
