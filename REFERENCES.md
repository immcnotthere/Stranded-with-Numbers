# References and Verification Notes

*Stranded with Numbers* uses references to **check definitions, theorems, counterexamples, and foundational claims**. The castaway's scenes, examples, and exposition are original. References are cited at the point of use by IDs linking here. This list was checked against accessible source pages on **2026-11-17**.

## Citation standard

- **Introduces** — The source defines, illustrates, or states a fact; do not portray it as proving the foundational theorem.
- **Proves / develops** — The source provides a derivation or construction, or sufficiently advanced treatment to support ours. Our written proof remains our own reconstruction.
- **Context / limitation** — The source establishes that a familiar law requires hypotheses, or supplies philosophical interpretation.
- **Not covered** — A source cannot be used to support an advanced claim merely because it discusses adjacent elementary material.

## O1
**OpenStax, *Prealgebra 2e*, §1.2, "Add Whole Numbers."**  
https://openstax.org/books/prealgebra-2e/pages/1-2-add-whole-numbers

*Introduces:* models of whole-number addition and the commutative property. **Does not establish** addition from Peano recursion.

## O2
**OpenStax, *Prealgebra 2e*, §7.2, "Commutative and Associative Properties."**  
https://openstax.org/books/prealgebra-2e/pages/7-2-commutative-and-associative-properties

*Introduces/states:* the order and regrouping laws for usual arithmetic. **Does not provide** our induction proofs.

## O3
**OpenStax, *Prealgebra 2e*, §7.4, "Properties of Identity, Inverses, and Zero."**  
https://openstax.org/books/prealgebra-2e/pages/7-4-properties-of-identity-inverses-and-zero

*Introduces:* additive identities, additive inverses, and zero. Used primarily as a preview of Chapters 02–03.

## O4
**OpenStax, *Contemporary Mathematics*, §1.1, "Basic Set Concepts."**  
https://openstax.org/books/contemporary-mathematics/pages/1-1-basic-set-concepts

*Introduces:* finite sets and cardinality.

## O5
**OpenStax, *Contemporary Mathematics*, §1.4, "Set Operations with Two Sets."**  
https://openstax.org/books/contemporary-mathematics/pages/1-4-set-operations-with-two-sets

*States and illustrates:* inclusion-exclusion; for disjoint finite sets, |A∪B|=|A|+|B|. Distinguish this **ordinary union** from a **tagged disjoint union**.

## O6
**OpenStax, *Calculus Volume 2*, §5.5, "Alternating Series."**  
https://openstax.org/books/calculus-volume-2/pages/5-5-alternating-series

*Develops with examples:* absolute versus conditional convergence and rearrangement of infinite real series. Identifies the Riemann rearrangement theorem but notes that its full proof is beyond its scope.

## U1
**University of Strathclyde, CS208 Logic & Algorithms, "Arithmetic and Induction."**  
https://personal.cis.strath.ac.uk/robert.atkey/cs208/induction.html

*Develops:* Peano-style arithmetic, formal equality, induction, and proof methodology. This is the appropriate level for the formal method rather than an introductory OpenStax arithmetic section.

## U2
**Dumas and McCarthy, *Transition to Higher Mathematics*, §8.2, "The Integers," via Mathematics LibreTexts.**  
https://math.libretexts.org/Bookshelves/Mathematical_Logic_and_Proof/Transition_to_Higher_Mathematics_(Dumas_and_McCarthy)/08:_New_Page/8.02:_New_Page

*Constructs:* integers as equivalence classes of natural-number pairs, addition on representatives, and additive inverses.

## S1
**Stanford Encyclopedia of Philosophy, "Set Theory," §2.**  
https://plato.stanford.edu/entries/set-theory/

*Develops:* set-theoretic foundations of numbers, natural numbers as finite ordinals, integers and rationals by equivalence classes.

## S2
**Stanford Encyclopedia of Philosophy, "Set Theory > Basic Set Theory."**  
https://plato.stanford.edu/archives/spr2022/entries/set-theory/basic-set-theory.html

*Develops:* bijections, finite cardinality, von Neumann natural numbers. This is an **archived** edition used for its detailed elementary construction.

## S3
**Stanford Encyclopedia of Philosophy, "Algebra."**  
https://plato.stanford.edu/archives/sum2026/entries/algebra/

*Develops:* algebraic structures, free algebras, monoids and free commutative monoids, including the single-generator case.

## S4
**Wolfram MathWorld, "Ordinal Addition."**  
https://mathworld.wolfram.com/OrdinalAddition.html

*Context / limitation:* ordinal addition is associative but not commutative; shows the difference between 1+ω and ω+1.

## S5
**Oracle, *Java Language Specification*, §15.18.2, "Additive Operators."**  
https://docs.oracle.com/javase/specs/jls/se20/html/jls-15.html#jls-15.18.2

*Context / limitation:* floating-point addition is not associative under finite-precision computation. The binary64 example in the interlude is a directly reproducible numerical illustration, not a quotation from the specification.

## S6
**Stanford Encyclopedia of Philosophy, "Structuralism in the Philosophy of Mathematics."**  
https://plato.stanford.edu/entries/structuralism-mathematics/

*Context:* mathematics as study of structures rather than a unique material representation.

## S7
**Stanford Encyclopedia of Philosophy, "Platonism in the Philosophy of Mathematics."**  
https://plato.stanford.edu/entries/platonism-mathematics/

*Context:* the claim that mathematical objects exist independently of our thought and language.

## S8
**Stanford Encyclopedia of Philosophy, "Formalism in the Philosophy of Mathematics."**  
https://plato.stanford.edu/entries/formalism-mathematics/

*Context:* different formalist conceptions of mathematics; **not all formalism** reduces truth to mere string manipulation.

## S9
**Stanford Encyclopedia of Philosophy, "Gödel's Incompleteness Theorems."**  
https://plato.stanford.edu/entries/goedel-incompleteness/

*Develops:* first-order PA as a formal axiomatic theory and the hypotheses and scope of incompleteness. Incompleteness is not a failure of elementary proofs of commutativity or associativity.

## Verification gaps / boundaries

- **Universality:** The standard Peano proofs in Interlude 01A are independently written here. U1 checks the formal framework; it is not a claim that OpenStax contains those proofs.
- **Free commutative monoid universal property:** S3 supports the terminology and one-generator case; the precise map f(n)=nx is explained and may be independently proved as a mastery exercise.
- **Recursion theorem:** In a set-theoretic or second-order Peano construction, recursion is justified by an appropriate recursion theorem. In usual **first-order PA**, addition is instead a primitive function symbol constrained by recursive axioms. Do not conflate these presentations.
- **Real completeness:** The claim that rational/real number systems can be constructed is a preview, not an actual construction of the real numbers in Chapter 01A.
- **Citation scope:** OpenStax is our main pedagogical spine; specialized sources are needed for Peano recursion, universal constructions, ordinal arithmetic, and foundational philosophy.
