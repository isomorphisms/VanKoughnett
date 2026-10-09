# Anna Marie Bohmann — equivariant Witt complexes and twisted THH

Checked 2026-10-09. This is a focused continuation of [research-notes.md](research-notes.md), centered on the 2024–2025 equivariant Witt-complex work and its relation to Bohmann's earlier Tambara, norm, and K-theory projects.

## Primary source

Anna Marie Bohmann, Teena Gerhardt, Cameron Krulewski, Sarah Petersen, and Lucy Yang, [*Equivariant Witt Complexes and Twisted Topological Hochschild Homology*](https://arxiv.org/abs/2409.05965), submitted 2024-09-09 and revised 2025-03-07.

The complete 39-entry bibliography of that version is credited entry-by-entry in [../researchers/ACKNOWLEDGMENTS.md](../researchers/ACKNOWLEDGMENTS.md).

## 1. Why THH carries more algebra than an ordinary graded ring

For an ordinary ring spectrum \(R\), topological Hochschild homology \(\operatorname{THH}(R)\) has an \(S^1\)-action. Fixed points under cyclic subgroups \(C_{p^m}\subset S^1\), together with restriction, Frobenius, transfer/Verschiebung, multiplication, and the circle operator, encode the algebra behind topological cyclic homology.

Hesselholt and Madsen organized this structure using **Witt complexes**. In degree zero, Witt vectors already appear. A Witt complex records the extra compatibility needed in all homotopy degrees.

Bohmann and collaborators ask for the corresponding object when the input ring is itself equivariant.

## 2. Norms make THH equivariant

A central insight in modern equivariant homotopy theory is that ordinary THH can be regarded as a norm from the trivial group to \(S^1\):

\[
\operatorname{THH}(R)\simeq N_e^{S^1}R.
\]

For a genuine \(C_n\)-equivariant ring spectrum, the analogous construction is a **twisted THH**

\[
\operatorname{THH}_{C_n}(R)\simeq N_{C_n}^{S^1}R.
\]

The norm technology grows out of Hill–Hopkins–Ravenel and the extension of norms to the circle by Angeltveit, Blumberg, Gerhardt, Hill, Lawson, and Mandell.

The important point is that multiplication is no longer just multiplication. Genuine equivariance remembers restrictions to subgroups, additive transfers, and multiplicative norms, so the algebra naturally lives in Green and Tambara functors.

## 3. Tambara functors as the degree-zero algebra

A Tambara functor can be thought of as a Mackey functor with coherent multiplicative norm maps. For a finite group \(G\), it packages three types of operations:

- restriction along subgroup inclusions;
- additive transfer;
- multiplicative norm.

Bohmann's earlier paper with Vigleik Angeltveit on **graded Tambara functors** supplies part of this background. Her work with Angélica Osorno on categorical Mackey functors addresses another part: how genuine equivariant stable-homotopy data can be constructed or modeled from categorical algebra.

The Witt-complex paper sits downstream of those ideas. It asks what algebra all homotopy groups of twisted THH carry, not just \(\underline\pi_0\).

## 4. Main theorem: an equivariant Witt complex

Let \(n>0\), let \(p\) be an odd prime with \(p\nmid n\), and let \(\underline R\) be a \(C_n\)-Tambara functor satisfying the stated \(\mathbb Z_{(p)}\)-algebra hypotheses at every orbit.

The paper proves that the graded Green functors

\[
\left\{
\underline{\pi}_*^{C_{p^m n}}
\operatorname{THH}_{C_n}\underline R
\right\}_{m\ge 0}
\]

assemble into a \(C_n\)-**equivariant Witt complex** over \(\underline R\).

When \(n=1\), their definition recovers the classical Hesselholt–Madsen notion. Thus the classical theory occurs as the trivial-equivariance special case.

## 5. What has to be compatible

The useful mental model is a tower indexed by powers of \(p\). Between levels live variants of:

- restriction maps;
- Frobenius-like maps;
- additive transfers/Verschiebung-like maps;
- multiplicative Teichmüller-type lifts;
- the differential coming from the circle action;
- subgroup restriction and transfer internal to the \(C_n\)-equivariant Green functors.

The equivariant Witt-complex axioms specify relations among these operations. The hard part is not naming the maps; it is showing that the geometry of the twisted cyclic bar construction forces the expected algebraic identities.

## 6. A small Tambara warm-up: \(C_2\)

For \(C_2\), the Burnside Tambara functor is a concrete model for the distinction between additive transfer and multiplicative norm. At the group level, restriction forgets symmetry, transfer adds an orbit of copies, while norm multiplies over an orbit.

If an underlying element is \(a\), the norm should be pictured schematically as

\[
N_e^{C_2}(a)=a\cdot g(a),
\]

not as the additive expression \(a+g(a)\). For a trivial action this simplifies numerically to \(a^2\), but the construction retains equivariant information lost by simply squaring an integer.

That distinction is exactly why ordinary commutative algebra is too small for genuine equivariant THH.

## 7. Why Witt vectors appear

Classically, the fixed-point tower of THH is tied to Witt vectors because restriction/Frobenius/transfer maps satisfy arithmetic patterns that define Witt-vector coordinates and ghost maps.

In the equivariant setting there are two interacting subgroup structures:

1. the \(C_{p^m}\) tower coming from the circle/cyclotomic direction;
2. the original \(C_n\)-equivariance of the input.

The equivariant Witt complex is the algebraic object that simultaneously remembers both.

## 8. Relation to algebraic K-theory

THH and topological cyclic homology matter because of trace maps from algebraic K-theory. The Witt-complex paper situates twisted THH near **Mona Merling's equivariant algebraic K-theory of \(G\)-rings** and later trace-method work.

A useful route through Bohmann's corpus is:

\[
\text{Mackey/Tambara algebra}
\to
\text{equivariant norms}
\to
\text{twisted THH}
\to
\text{Witt-complex structure}
\to
\text{trace methods for equivariant K-theory}.
\]

This complements the separate scissors-congruence trace project with Gerhardt, Malkiewich, Merling, and Zakharevich: both use stable categorical structure to manufacture trace-like invariants, but they start from different K-theories.

## 9. Relation to coTHH

Bohmann, Gerhardt, and Brooke Shipley study **topological coHochschild homology** and free loop spaces. It is useful not to conflate coTHH with the twisted-THH story:

- THH starts from multiplication and cyclic bar constructions;
- coTHH is a coalgebraic/cobar-side analogue;
- both are places where circle/free-loop phenomena appear;
- their input hypotheses and algebraic structures are different.

The common theme is not “everything is THH,” but that stable homotopy exposes algebraic structure carried by loops, norms, traces, and equivariance.

## 10. Lawvere theories and structural K-theory

Bohmann's work with Markus Szymik on K-theory of Lawvere theories is another structural branch. Lawvere theories encode algebraic operations abstractly. Morita-style questions ask when different presentations produce the same algebraic K-theory.

This branch belongs beside the equivariant work because it reflects the same methodological interest: determine which algebraic/categorical structure survives passage to a stable invariant.

## 11. Things worth formalizing or visualizing

### Subgroup lattice

For \(C_{p^m n}\), draw the subgroup tower vertically and mark restriction, transfer, Frobenius, and norm arrows with distinct arrow types. Many Witt relations become statements that two paths in this diagram agree.

### Orbit-level algebra

A Tambara functor can be displayed as data attached to each orbit \(G/H\). A typed diagram can make each map know whether it is restriction, additive transfer, or norm, preventing accidental identification of the three.

### Cyclic bar picture

The twisted cyclic bar construction has a geometric rotation built into it. A visual model could show how the \(C_n\)-twist changes the gluing at the cyclic seam.

These expose the actual extra equivariant structure better than a generic spectrum picture.

## 12. Current research-page map

Bohmann's public research page also lists work on:

- categorical Mackey functors with Angélica Osorno;
- global orthogonal spectra;
- graded Tambara functors with Vigleik Angeltveit;
- computational tools for coTHH with Teena Gerhardt, Amalie Høgenhaven, Brooke Shipley, and Stephanie Ziegenhagen;
- coTHH and free loop spaces with Gerhardt and Shipley;
- K-theory of Lawvere theories with Markus Szymik;
- rational genuine-commutative K-theory with collaborators including Christy Hazel, Jocelyne Ishak, Magdalena Kędziorek, and Clover May.

The overview notebook keeps the broader inventory; this file records the mathematical path through the newest Witt-complex paper.

## 13. Credit and provenance

The anchor paper is joint work of **Anna Marie Bohmann, Teena Gerhardt, Cameron Krulewski, Sarah Petersen, and Lucy Yang**. Its 39 bibliography entries are individually credited in the central ledger. Among the foundational lines explicitly used are work of **Lars Hesselholt and Ib Madsen**, **Michael Hill, Michael Hopkins, and Douglas Ravenel**, and **Vigleik Angeltveit, Andrew Blumberg, Teena Gerhardt, Michael Hill, Tyler Lawson, and Michael Mandell**.

The notes do not imply that every cited paper has been read. The bibliography ledger distinguishes credit traversal from full-paper reading.

## 14. Reading order

1. Graded Tambara functors: learn restriction/transfer/norm vocabulary.
2. Read the introduction to twisted THH as a norm.
3. Read the definition of equivariant Witt vectors.
4. Read the definition of equivariant Witt complexes and compare it with the \(n=1\) classical case.
5. Read the proof section relation-by-relation, keeping a subgroup-lattice diagram beside it.
6. Then return to trace methods and equivariant algebraic K-theory.
