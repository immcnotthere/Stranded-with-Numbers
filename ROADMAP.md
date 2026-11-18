# Roadmap — Stranded with Numbers

*An Islander's Guide to Reinventing Mathematics*

> **The challenge:** Reconstruct the computational ideas of calculus using remembered arithmetic whose rules we cannot yet justify. No advanced formula may be used merely because its name sounds familiar.

This is a **working editorial roadmap**, not a fixed syllabus. Each chapter should be revised together before it becomes finished prose.

**Chosen voice: story + mathematical notebook.** A short castaway scene motivates each problem; a direct notebook reconstructs the mathematics with finite calculations before introducing new notation. See [LEARNING_PATH.md](LEARNING_PATH.md) for the dependency graph and [CONCEPT_TRACKER.csv](CONCEPT_TRACKER.csv) for lesson-by-lesson progress.

## What the castaway remembers

The castaway can **count, add, subtract, multiply, and divide**, including ordinary calculations with fractions. These are remembered procedures, **not yet justified mathematical ideas**. He does not know why the rules work, when they fail, or how to reconstruct them from first principles.

He has scattered memories of school: **sine, cosine, angles, geometry, and linear equations**. These are clues and narrative foreshadowing, not tools he may invoke without rebuilding them.

**The challenge is no longer to invent arithmetic without knowing it. It is to justify familiar arithmetic, discover what it can do, and rebuild the forgotten mathematics of change.**

## Rules of the island

1. **Arithmetic is remembered, not earned.** Counting, addition, subtraction, multiplication, division, and basic fractions may be used computationally from day one; their properties and justifications must be reconstructed.
2. **A problem precedes its tool.** Every chapter begins with a concrete challenge a castaway could encounter.
3. **Calculate before naming.** Use small, reproducible examples before introducing notation.
4. **Finite arithmetic first.** No limits, derivatives, integrals, or infinite sums are assumed at the outset.
5. **Separate evidence from proof.** Numerical patterns motivate conjectures; they do not alone establish exact identities.
6. **Keep an invention ledger.** State exactly which tools have been earned and which claims remain conjectural.
7. **Avoid artificial survival problems.** The island is a narrative constraint, not an excuse for contrived word problems.
8. **Familiar names are clues, not shortcuts.** Sine, cosine, angles, geometry, and linear equations are vague memories; their meaning must be recovered through problems and calculations.

## The six acts

| Act | Narrative question | Mathematical inventions | Milestone |
|---|---|---|---|
| I. Counting the Island | How can one quantity be compared with another? | units, counting, addition, zero, subtraction, repeated addition, multiplication, equal sharing, fractions | rational arithmetic |
| II. Patterns in the Sand | How can we predict without counting every step? | sequences, powers, geometric growth, tables, finite sums, factorials, approximation, error | calculable patterns |
| III. The Shape of the Shore | How can arithmetic describe space and turning? | coordinates, distance, squares, rational approximations, angles, circles, signed directions, complex pairs | arithmetic of rotation |
| IV. The Compounding Tide | What number describes growth broken into many steps? | repeated compounding, exponential approximations, factorial expansions, complex multiplication, numerical sine/cosine, π | Euler's formula and identity |
| V. Measuring the Unmeasurable | How can we measure a speed or area when it keeps changing? | difference quotients, finite differences, rectangles and sums, numerical rates, numerical accumulation, error refinement | computational differentiation and integration |
| VI. The Rules Behind the Rules | When do our approximations justify exact claims? | bounds, convergence, limits, continuity, derivatives, integrals, fundamental theorem, rigorous Euler identity | calculus with proofs |

---

## Act I — Counting the Island

**Question:** We remember arithmetic. Why do its rules work, and what can we establish from them?

- **01. One Thing, Two Things** — Distinguish objects, choose a unit, count, compare, and add.
- **02. The Empty Basket** — Invent zero and learn why a neutral quantity is useful.
- **03. Giving Things Back** — Reverse addition; introduce subtraction and negative quantities when a debt or direction requires them.
- **04. Too Many Additions** — Invent multiplication as a shortcut for repeated equal additions.
- **05. Sharing the Harvest** — Divide quantities into equal groups; invent fractions and rational arithmetic.
- **06. Can We Always Share Exactly?** — Explore ratios, remainders, and the first limitations of fractions.

**Justified:** units, zero, inverse operations, repeated addition, equal sharing, fractions, and elementary equation-solving. The procedures were familiar; their explanations were not.  
**Open question:** What if we need more precision than our present fractions conveniently provide?

## Act II — Patterns in the Sand

**Question:** Can we calculate the hundredth step without performing the first ninety-nine?

- **07. The Hundredth Pile** — Arithmetic sequences, repeated increments, and finite arithmetic sums.
- **08. The Doubling Problem** — Repeated multiplication, powers, and geometric sequences.
- **09. Adding What Keeps Growing** — Derive a finite geometric-sum formula by rearranging and subtracting two sums.
- **10. The Counting of Arrangements** — Factorials and the number of ways to choose or order objects.
- **11. How Wrong Are We?** — Approximation, decimal representation, upper/lower estimates, and explicit numerical error.
- **12. A Pattern Is Not a Proof** — Counterexamples and the distinction between tested examples and universal claims.

**Earned:** powers, finite series, factorials, numerical algorithms, error accounting.  
**Open question:** Can these patterns help us measure shapes and changes that resist direct counting?

## Act III — The Shape of the Shore

**Question:** What were those half-remembered ideas about angles, geometry, and sine and cosine actually describing?

- **13. A Map Made of Numbers** — Ordered pairs, coordinates, displacement, and signed directions.
- **14. The Shortest Walk** — Squares, the Pythagorean relationship, and numerical square-root approximations.
- **15. The Circle We Cannot Square with Fractions** — Circles, circumference-to-diameter experiments, and approximations to π.
- **16. Turning Without a Protractor** — Rotations as transformations of coordinates; right angles and quarter-turns.
- **17. A New Kind of Number** — Represent a point by a pair of numbers; construct the multiplication rule for complex numbers and explain why i² = −1.
- **18. Fractions That Rotate** — Pythagorean triples and rational points on the unit circle; repeated complex multiplication as turning.

**Earned:** coordinates, numerical distance, π as a geometric target, complex arithmetic, rotation.  
**Open question:** Can the arithmetic of growth also describe rotation?

## Act IV — The Compounding Tide

**Question:** What happens when the same total growth is broken into ever smaller compounded steps?

- **19. One Harvest, Many Intervals** — Compare (1 + 1/n)^n for finite choices of n, using only arithmetic.
- **20. The Number Hiding in Compounding** — Compute increasingly accurate estimates of e; investigate why the values cluster and how to bound them.
- **21. Another Road to the Same Number** — Expand finite powers, discover binomial coefficients and factorial terms; compare finite sums with compounding estimates without assuming their exact equivalence.
- **22. Growth by Any Amount** — Build finite approximations to exponential behavior for a chosen x; investigate addition of inputs versus multiplication of outputs.
- **23. What If Growth Turns Sideways?** — Substitute complex increments; multiply out finite expressions and track real and imaginary parts.
- **24. Two Patterns Around a Circle** — Construct finite even- and odd-power sums and compare them numerically with circle coordinates.
- **25. Half a Turn** — Numerically investigate e^(iπ) ≈ −1 and formulate Euler's identity as a conjecture awaiting proof.

**Earned:** algorithms for e, exponential approximation, complex exponential approximation, numerical trigonometric patterns.  
**Open question:** How can the same machinery calculate change at a single instant?

> **Important:** At this stage Euler's identity is a numerical discovery, **not yet a proved equality**. Any exact use of e, π, sine, cosine, or an infinite series must be marked as provisional until Act VI.

## Act V — Measuring the Unmeasurable

**Question:** How do we measure something that changes while we measure it?

- **26. How Fast Was the Canoe?** — Average speed over a chosen interval; construct difference quotients.
- **27. Smaller Intervals, Better Guesses** — Compare forward, backward, and centered numerical rates.
- **28. Finding the Steepest Path** — Finite differences of tables and powers; discover familiar derivative patterns empirically.
- **29. Counting the Space Under a Curve** — Approximate area using finite rectangles.
- **30. Better Rectangles** — Left, right, midpoint, and trapezoidal estimates; compare errors.
- **31. Does Accumulation Undo Change?** — Compare numerical rates with accumulated sums and discover the relationship that will become the fundamental theorem.
- **32. Predicting Tomorrow** — Step-by-step numerical solutions to changing systems, including elementary motion and growth models.

**Earned:** numerical differentiation, numerical integration, discrete models, numerical solutions of differential equations.  
**Open question:** When can finite approximations establish something exact?

## Act VI — The Rules Behind the Rules

**Question:** What must be true for increasingly refined arithmetic to justify a mathematical theorem?

- **33. How Close Is Close Enough?** — Precise error bounds and what it means to guarantee an approximation.
- **34. Numbers Our Fractions Approach** — Construct the idea of convergence and the real-number setting it needs.
- **35. The Meaning of a Limit** — Formalize the pattern of numerical refinement only now.
- **36. When Small Changes Stay Small** — Continuity.
- **37. The Exact Rate of Change** — Define derivatives and prove selected rules motivated in Act V.
- **38. The Exact Total** — Define integrals and establish the relationship between accumulation and rates.
- **39. Why the Exponential Is Special** — Prove the central exponential properties and justify the appropriate series representations.
- **40. Why Turning and Growing Are One Calculation** — Establish the complex exponential, sine and cosine connection, and prove Euler's identity.

**Earned:** the foundational methods of single-variable calculus and a rigorous route to Euler's identity.  
**Open question:** Which additional assumptions, constructions, and proof techniques are required to extend the island's mathematics further?

---

## Standard chapter structure

Each chapter should be written in this order:

1. **The scene** — A short, plausible castaway episode posing a concrete problem.
2. **The notebook: what we know** — Only previously earned operations and facts.
3. **The notebook: an attempt** — Calculate a small example by hand.
4. **The discovery** — Identify the reusable pattern.
5. **The invention** — Introduce a name or notation only after the need is clear.
6. **The challenge** — A concrete numerical problem for the reader to solve independently.
7. **The ledger** — Record what is proved, what is observed, and what remains unresolved; update the concept tracker.

## Editorial decisions to settle together

- **Narrator:** settled — a short castaway story followed by a direct mathematical notebook.
- **Scope:** stop at foundational single-variable calculus, or add vectors, multivariable calculus, linear algebra, and differential equations as later volumes?
- **Proof policy:** do we postpone all formal convergence arguments until Act VI, or permit elementary finite bounds earlier?
- **Geometry order:** should the circle and complex numbers come before exponential growth, or should the discovery of e come first?
- **Exercises:** a short numerical challenge after every discovery, or longer end-of-act expeditions?
- **Tone:** settled — playful but restrained narrative; exacting numerical notebook.

## Current status

- [x] Book title and premise
- [x] Introductory README
- [x] Initial six-act roadmap
- [ ] Revise early chapters to emphasize justification rather than first discovery
- [ ] Agree on act order and chapter count
- [x] Agree on narrator and style
- [x] Create dependency graph and lesson mastery tracker
- [ ] Draft Chapter 01
- [ ] Review and revise Chapter 01 together
