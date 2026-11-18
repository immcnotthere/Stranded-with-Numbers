# Interlude 01A — The Laws Beneath the Stones

*An extended story-and-notebook companion to [Chapter 01](01-one-thing-two-things.md). It is a foundational deep dive, not a claim that all of mathematics follows from addition.*

## The stone that belonged to two piles

By afternoon the castaway had made a mistake.

He had counted four stones beside the fire and five near the shelter, then written **nine** in his ledger. But one flat stone had been moved from the fire to the shelter after the first count. He could find only eight.

He had not forgotten how to add. He had forgotten to ask what his numbers referred to.

> A number is not a substitute for identifying what has been counted.

He separated the stones, marked the two groups with pieces of rope, and began again. If the groups did not overlap, combining them gave a reliable count. If they overlapped, the same object might be counted twice.

The problem was no longer how to obtain an answer. It was how to **defend** one.

## Notebook A — What sort of thing is addition?

We must name the domain. A *binary operation* on a set \(X\) is a function \(X\times X\to X\): every ordered pair of elements has exactly one output in \(X\). **Closure** is built into this definition.

Ordinary addition of natural numbers, integers, rational numbers, real numbers, complex numbers, and vectors shares several laws. Other operations called *addition* need not share them all.

| Law or distinction | Statement | Status |
|---|---|---|
| Closure / totality | \(a+b\in X\) and is uniquely defined for each \(a,b\in X\) | Part of being a binary operation on \(X\) |
| Right identity | \(a+0=a\) | Defining recursion clause on \(\mathbb N\) |
| Left identity | \(0+a=a\) | Theorem from recursion and induction |
| Successor recursion | \(a+S(b)=S(a+b)\) | Defining recursion clause |
| Associativity | \((a+b)+c=a+(b+c)\) | Theorem on \(\mathbb N\) |
| Commutativity | \(a+b=b+a\) | Theorem on \(\mathbb N\) |
| Cancellation | \(a+c=b+c\Rightarrow a=b\) | Theorem on \(\mathbb N\); not universal |
| Additive inverses | \(a+(-a)=0\) | Available in \(\mathbb Z,\mathbb Q,\mathbb R,\mathbb C\), not all of \(\mathbb N\) |
| Order translation | \(a<b\Rightarrow a+c<b+c\) | For compatible ordered additive structures |
| Distributivity | \(a(b+c)=ab+ac\) | Connects addition to multiplication; not a law of addition alone |
| Finite sums | \(\sum_{k=1}^{n}a_k\) | Repeated addition; grouping is licensed by associativity |
| Infinite series | \(\sum_{k=1}^{\infty}a_k\) | A limit of finite sums; requires additional foundations |

**Question to keep asking:** Is a claim a definition, an axiom, a theorem, or an interpretation?

## Notebook B — Two rigorous constructions

### B1. Counting by correspondence

For finite sets \(A\) and \(B\), write \(|A|\) and \(|B|\) for their numbers of elements. Two sets have the same finite cardinality if there is a *bijection*: a matching that uses each element of each set exactly once.

Use a **tagged disjoint union** \(A\sqcup B\), so that an object appearing in both source sets is still represented as two distinctly tagged entries. Define addition of finite cardinalities by

\[
|A|+|B|=|A\sqcup B|.
\]

Swapping tags gives a bijection \(A\sqcup B\cong B\sqcup A\): this explains commutativity. Retagging gives \((A\sqcup B)\sqcup C\cong A\sqcup(B\sqcup C)\): this explains associativity. The empty set is the identity.

For physical stones, however, **do not tag the same stone twice** if you mean to count unique stones. The formal disjoint union counts occurrences; the physical union counts distinct objects. The difference explains his mistaken ledger.

### B2. Zero, successor, and induction

We now make a deliberate foundational detour. This is not a tool the castaway already possesses: it is a theory he is proposing to justify counting.

Let \(\mathbb N\) include \(0\). Assume a successor operation \(S\), with \(0\) not a successor, distinct numbers having distinct successors, and an induction principle. A standard Peano formulation also states that \(0\in\mathbb N\) and every natural number has a successor.

**Define** addition recursively:

\[
a+0=a,\qquad a+S(b)=S(a+b).
\]

A recursion theorem (whose proof uses the natural-number foundations) ensures that these equations determine a unique operation. We have not smuggled in commutativity or associativity.

For instance,

\[
2+3=2+S(2)=S(2+2)=S(S(2+1))=S(S(S(2)))=5.
\]

### B3. Proof of left identity

Base case: \(0+0=0\). If \(0+n=n\), then

\[
0+S(n)=S(0+n)=S(n).
\]

By induction, \(0+n=n\) for every \(n\).

### B4. Proof of associativity

Fix \(a,b\), and induct on \(c\). At \(c=0\), both sides equal \(a+b\). If \((a+b)+c=a+(b+c)\), then

\[
\begin{aligned}
(a+b)+S(c)
&=S((a+b)+c)\\
&=S(a+(b+c))\\
&=a+S(b+c)\\
&=a+(b+S(c)).
\end{aligned}
\]

Thus \((a+b)+c=a+(b+c)\).

### B5. Proof of commutativity

First prove by induction on \(b\) that

\[
S(a)+b=S(a+b).
\]

At \(b=0\), both sides equal \(S(a)\). If it holds at \(b\), then

\[
S(a)+S(b)=S(S(a)+b)=S(S(a+b))=S(a+S(b)).
\]

Now fix \(a\), and induct on \(b\). At zero, \(a+0=0+a\). Assuming \(a+b=b+a\),

\[
a+S(b)=S(a+b)=S(b+a)=S(b)+a.
\]

Therefore \(a+b=b+a\).

### B6. Proof of cancellation

Induct on \(c\). If \(a+0=b+0\), then \(a=b\). If

\[
a+S(c)=b+S(c),
\]

then \(S(a+c)=S(b+c)\). Injectivity of successor gives \(a+c=b+c\), and the inductive hypothesis gives \(a=b\).

**Notice:** Associativity and commutativity alone do not imply cancellation. A monoid can lack it.

### B7. Order and monotonicity

Define \(a<b\) on natural numbers when there exists a **positive** natural number \(k\) such that \(b=a+k\). Positivity here means \(k\ne0\). Then

\[
b+c=(a+k)+c=(a+c)+k,
\]

so \(a+c<b+c\). The non-strict version follows similarly. The proof uses associativity and the definition of order; it does not make sense for arbitrary unordered objects.

## The third morning: a debt of stones

He promised a neighbor three stones and delivered five. In his notebook he wrote a balance of *two stones beyond the promise*. But what if he had delivered only one? He needed a way to represent *two stones short*.

Natural-number addition could combine counts, but it could not always undo them.

## Notebook C — From monoids to groups

A **magma** is a set with a closed binary operation. A **semigroup** has an associative operation. A **monoid** also has an identity. A **group** also has inverses. An **abelian group** is a commutative group.

The natural numbers with \(+\) and \(0\) form a **commutative monoid**, not a group: \(3+x=0\) has no natural-number solution.

Construct integers from pairs of natural numbers. Interpret \((a,b)\) as a formal difference, and declare

\[
(a,b)\sim(c,d)\iff a+d=b+c.
\]

This is an equivalence relation, using cancellation to prove transitivity. Define

\[
[(a,b)]+[(c,d)]=[(a+c,b+d)].
\]

One must check this operation is **well-defined**: replacing a pair by an equivalent representative leaves the resulting equivalence class unchanged. The inverse of \([(a,b)]\) is \([(b,a)]\), and zero is \([(0,0)]\). This construction is the **group completion** of \((\mathbb N,+)\).

For example, \([(1,3)]\) represents two stones owed; \([(5,2)]\) represents three stones in surplus. Adding them produces a net surplus of one.

The identity in a monoid is unique: if \(e\) and \(f\) are both two-sided identities, then \(e=e+f=f\). In a group, inverses are also unique, by associativity and the identity laws.

### The next extensions

Rational numbers can be constructed as equivalence classes of integer numerator–nonzero-denominator pairs. Real numbers require an additional completeness construction, such as Dedekind cuts or Cauchy sequences of rationals. Their additive operations inherit or extend the relevant group laws, but their construction and completeness are **not** consequences of the addition laws alone.

Multiplication introduces new structure. For natural numbers, one may define \(a\cdot0=0\) and \(a\cdot S(b)=a\cdot b+a\); distributivity is then proved by induction. Distributivity links two operations and should not be misclassified as an axiom of addition by itself.

## Notebook D — What the abstract view buys us

The natural numbers with addition are the **free commutative monoid on one generator**. Given any commutative monoid \(M\) and any \(x\in M\), there is a unique monoid homomorphism \(f:\mathbb N\to M\) with \(f(1)=x\), defined by \(f(n)\) as \(n\) copies of \(x\) added together (and \(f(0)\) as the identity).

This *universal property* tells us what counting does in every commutative monoid. It characterizes the structure by its relationships, rather than by the material from which its elements are made.

Set theory offers another foundation. In the von Neumann construction, \(0=\varnothing\), \(S(n)=n\cup\{n\}\), so \(1=\{0\}\), \(2=\{0,1\}\), and so forth. This represents natural numbers as sets. The representation is a construction, **not** a claim that the physical number two literally consists of two stones.

## Notebook E — Where addition's laws fail

Knowing a theorem includes knowing its hypotheses.

1. **Ordinal addition is not commutative.** If \(\omega\) is the order type of the natural numbers, then \(1+\omega=\omega\) but \(\omega+1>\omega\). Adding a first element differs from appending a last element.
2. **Infinite cardinal addition does not have cancellation.** \(1+\aleph_0=2+\aleph_0=\aleph_0\), although \(1\ne2\).
3. **Floating-point addition need not be associative.** In IEEE 754 binary64 with round-to-nearest, \((10^{16}+(-10^{16}))+1=1\), while \(10^{16}+((-10^{16})+1)=0\). The machine computes rounded approximations, not exact real addition.
4. **Infinite sums require convergence.** A series is defined through a sequence of finite partial sums. Conditionally convergent real series can change value under rearrangement; absolute convergence is a sufficient safeguard.
5. **Order is extra structure.** Ordinary real addition preserves order under translation. Complex numbers cannot be given an order making them an ordered field.

None of these contradict the natural-number proofs. They concern different domains, different operations, or additional rules.

## Notebook F — Can arithmetic justify itself?

He watched two waves meet and become one.

If two drops of water joined three drops and made one larger drop, had \(2+3=5\) failed? No. The physical objects being counted had changed. Arithmetic describes a model; the model must match the phenomenon.

Four philosophical readings are useful:

- **Platonism:** arithmetic describes truths about abstract mathematical objects.
- **Formalism:** proofs follow from explicit axioms and rules in a formal system.
- **Constructivism:** mathematical assertions are justified by constructions or proofs.
- **Structuralism:** what matters is the role of numbers in a structure, not their particular representation.

These are philosophical positions, not four alternative calculations.

**Truth, definition, and proof are different notions.** The recursive equations *define* addition on the natural numbers. Commutativity is then a *theorem*. A claim's truth in a structure is conceptually distinct from its provability in a particular formal theory.

We cannot prove every premise without using some premises and rules of inference. Peano arithmetic and set theory make different starting assumptions. Gödel's incompleteness theorems concern sufficiently expressive, consistent, effectively axiomatized systems; they do **not** undermine our elementary proofs of addition.

## Notebook G — The defense

If someone asks, *“Why should I believe addition works?”*, the castaway can now answer:

> First specify what is being added. For finite collections, disjoint union and one-to-one correspondence explain the counting interpretation. For natural numbers, successor, induction, and recursive definition give an exact operation whose identity, associativity, commutativity, and cancellation laws we can prove. The integers extend that operation by constructing additive inverses. Abstract algebra records which laws survive in other settings. Where the hypotheses change, the laws may fail.

He had not discovered a formula for everything. He had learned how to know **which** formulas he was entitled to use.

## Proof obligations and exercises

1. Prove the left identity law from the recursion clauses.
2. Prove associativity by induction, indicating the inductive hypothesis.
3. Prove the auxiliary successor lemma and use it to prove commutativity.
4. Prove cancellation; explain exactly where successor injectivity enters.
5. Construct a bijection between \((A\sqcup B)\sqcup C\) and \(A\sqcup(B\sqcup C)\).
6. Verify that integer-pair addition respects the equivalence relation.
7. Prove uniqueness of identity and uniqueness of additive inverse.
8. Explain why \(1+\omega\ne\omega+1\) does not contradict commutativity of natural-number addition.
9. Explain the floating-point counterexample without saying that real addition is nonassociative.
10. Defend the distinction between a physical count, a mathematical definition, and a theorem.

**Mastery:** Being able to repeat a proof is level 2. Proving the laws independently and solving a fresh example is level 3. Explaining their assumptions, constructing a counterexample outside those assumptions, and defending the foundations is level 4.

## Invention ledger

**Justified in this interlude:** finite cardinal addition; recursive natural-number addition; left identity, associativity, commutativity, cancellation, order translation; the algebraic classifications and the integer extension, subject to the stated constructions.

**Not established merely by this interlude:** completeness of the reals, the convergence of an arbitrary series, the foundations of all set theory, or a single addition law valid in every possible structure.

**Continue:** [Chapter 02 — The Empty Basket](02-the-empty-basket.md) *(forthcoming)*, where zero becomes a concrete problem before we return to its formal role.
