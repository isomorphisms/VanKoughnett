# Sarah Yeakel — from isovariant spaces toward isovariant stable homotopy

Checked 2026-10-09. This is a focused continuation of [research-notes.md](research-notes.md) and the existing Goodwillie-calculus files. It follows Yeakel's isovariant program through the 2026 Blakers–Massey paper.

## Primary sources

- Sarah Yeakel, [*An isovariant Elmendorf's theorem*](https://arxiv.org/abs/1907.12135), Documenta Math. 27 (2022), 613–628.
- Inbar Klang and Sarah Yeakel, [*Isovariant homotopy theory and fixed point invariants*](https://arxiv.org/abs/2110.07853), Advances in Mathematics 433 (2023).
- Inbar Klang and Sarah Yeakel, [*An isovariant Blakers–Massey theorem*](https://arxiv.org/abs/2506.21259), published electronically in Journal of Homotopy and Related Structures in 2026.
- For the other major branch of Yeakel's work: [*A Monoidal Model for Multilinearization*](https://arxiv.org/abs/1706.06915), plus the operad papers with Maria Basterra, Irina Bobkova, Kate Ponto, and Ulrike Tillmann.

The complete 22-entry bibliography of the Blakers–Massey paper is credited entry-by-entry in [../researchers/ACKNOWLEDGMENTS.md](../researchers/ACKNOWLEDGMENTS.md).

## 1. Equivariant versus isovariant

Let \(G\) act on spaces \(X\) and \(Y\). An equivariant map \(f:X\to Y\) satisfies

\[
f(gx)=g f(x).
\]

That implies only

\[
G_x\le G_{f(x)}
\]

for stabilizer groups. A point may move into a stratum with *more* symmetry.

An **isovariant** map imposes the stronger condition

\[
G_x=G_{f(x)}
\]

for every \(x\). It preserves the isotropy group exactly.

This changes the homotopy theory drastically. Ordinary equivariant homotopy is organized by fixed-point spaces \(X^H\). Isovariant homotopy also cares about how exact-isotropy strata fit together.

## 2. The smallest useful example

Let \(C_2\) act on \(\mathbb R\) by reflection \(x\mapsto -x\).

- \(0\) has stabilizer \(C_2\);
- every nonzero point has trivial stabilizer.

The constant map \(f(x)=0\) is equivariant, but it is not isovariant because a generic point with stabilizer \(e\) is sent to a point with stabilizer \(C_2\).

So equivariance permits collapse across isotropy strata; isovariance forbids it.

## 3. Isovariant Elmendorf theorem

Classical Elmendorf theory says equivariant homotopy theory for \(G\)-spaces can be modeled by diagrams over the orbit category.

Yeakel proves an isovariant analogue for finite groups:

1. construct a model structure on \(G\)-spaces with isovariant maps;
2. identify diagrammatic data that sees the relevant isotropy-stratum mapping spaces;
3. establish a Quillen equivalence between the isovariant category and the diagram category.

Exact preservation of isotropy changes the test objects and mapping spaces that detect weak equivalences; this is not a word-for-word substitution into the ordinary Elmendorf proof.

## 4. Manifolds need better isovariant cells

In the Klang–Yeakel fixed-point paper, the authors develop new isovariant cells suited to smooth \(G\)-manifolds. Smooth manifolds have tubular-neighborhood geometry around isotropy strata that arbitrary \(G\)-spaces need not possess.

They prove, for finite \(G\), that smooth \(G\)-manifolds can be built from these cells and satisfy suitable lifting properties. This yields an **isovariant Whitehead theorem**: for smooth \(G\)-manifolds, an isovariant weak equivalence is an isovariant homotopy equivalence.

## 5. Fixed points and Reidemeister traces

The same paper studies an isovariant self-map

\[
f:M\to M
\]

of a compact smooth \(G\)-manifold. Under suitable dimension and codimension hypotheses, the fixed points of \(f\) can be removed by an isovariant homotopy exactly when the equivariant Reidemeister-trace obstruction vanishes.

In that range, the isovariant fixed-point problem reduces to the equivariant one.

This creates a direct bridge to the parametrized-spectrum/Reidemeister-trace literature. It also helps explain why Cary Malkiewich's parametrized-spectra exposition appears in the later isovariant bibliography.

Important distinction: equality of the obstructions under these manifold hypotheses does **not** mean isovariant and equivariant homotopy theories are the same.

## 6. Why Blakers–Massey is the next step

Blakers–Massey controls the connectivity of a homotopy pushout square by the connectivities of its incoming maps. Higher versions control \(n\)-cubes.

This theorem is foundational for unstable-to-stable passage because it underlies excision estimates, Freudenthal suspension, and Goodwillie-style connectivity arguments.

Klang and Yeakel prove an isovariant Blakers–Massey theorem and an \(n\)-cubical generalization. This is substantial groundwork for an isovariant stable homotopy theory.

## 7. Isovariant suspension and Freudenthal

The paper defines a suspension operation in the isovariant category using a **trivial representation sphere** and proves an isovariant Freudenthal suspension theorem.

A subtle point is that isovariant suspension is not interchangeable with ordinary representation-sphere suspension. Two spaces can be equivariantly weakly equivalent while retaining different exact-isotropy-stratum data and therefore fail to be isovariantly weakly equivalent.

In a future formalization, representation suspension and the isovariant suspension functor should be different typed operations.

## 8. Worked \(C_2\) example from the 2026 paper

Let \(\sigma\) be the sign representation of \(C_2\).

For the vector space \(\sigma\):

- exact trivial isotropy: \(\sigma_{\{e\}}=\mathbb R-\{0\}\);
- \(C_2\)-isotropy: \(\sigma_{C_2}=\{0\}\).

For the one-point compactification \(S^\sigma\), the fixed-isotropy piece is \(S^0\), while the linking data around it comes from a punctured tubular neighborhood. Klang and Yeakel compute the resulting pieces after their suspension operation.

The geometric lesson is the key one: isovariant theory remembers not just the fixed set but how the free stratum approaches it.

## 9. Worked \(C_3\) example

Let \(\rho\) be the real regular representation of \(C_3\):

\[
\rho\cong\mathbb R\oplus\lambda,
\]

where \(\lambda\) is the 2-dimensional rotation representation.

In the one-point compactification \(S^\rho\),

\[
(S^\rho)_{C_3}=S^1,
\]

while the trivial-isotropy part is \(S^3-S^1\simeq S^1\). A punctured tubular neighborhood of the fixed circle is homotopy equivalent to

\[
S^1\times S^1.
\]

After suspension, the torus splitting

\[
\Sigma(S^1\times S^1)
\simeq
S^2\vee S^2\vee S^3
\]

produces different connectivity data on different isovariant diagram objects.

A single “dimension of the representation” therefore cannot encode isovariant connectivity.

## 10. Connection back to Goodwillie calculus

Yeakel's earlier Goodwillie work and newer isovariant work meet conceptually at **cubical connectivity**.

In Goodwillie calculus:

- excisive functors are tested on homotopy cocartesian cubes;
- Blakers–Massey estimates convert cocartesian information into cartesian connectivity;
- stabilization and multilinearization rely on such estimates.

The 2026 isovariant \(n\)-cubical theorem therefore supplies exactly the kind of input one would expect to need for a future **isovariant functor calculus**.

That is a plausible research direction, not a theorem claimed in the paper.

## 11. Connection to operads

A separate Yeakel branch, joint with Maria Basterra, Irina Bobkova, Kate Ponto, and Ulrike Tillmann, studies operads with homological stability and localization of unary operations.

Their theorem that group-completed algebras over an operad with homological stability become infinite loop spaces is another unstable-to-stable machine. It should not be identified with isovariant stabilization, but the parallel is useful:

- operadic branch: stability in genus/geometry yields infinite loop spaces;
- isovariant branch: connectivity and suspension theorems build a route toward stabilization;
- Goodwillie branch: polynomial approximation and multilinearization extract stable derivatives.

Yeakel's corpus repeatedly asks how structured unstable data acquires stable structure.

## 12. Potential visualization

An isovariant diagram wants to be drawn as a **stratified space plus links**.

For each isotropy type \(H\):

1. draw the stratum of points with exact stabilizer \(H\);
2. draw arrows for allowed incidence \(H<K\);
3. attach a link/tubular-neighborhood object describing how the \(H\)-stratum approaches the \(K\)-stratum;
4. label maps by connectivity.

This makes the Blakers–Massey estimates more inspectable than a page of subgroup-indexed symbols.

## 13. Credit and provenance

The 2026 anchor paper is joint work of **Inbar Klang and Sarah Yeakel**. Its 22 bibliography entries are fully credited in the central ledger. It explicitly cites foundations by **Alexander Bykov and Raúl Juárez Flores; A. L. Blakers and W. S. Massey; William Browder and Frank Quinn; Emanuele Dotto; Daniel Dugger; Graham Ellis and Richard Steiner; Hans Freudenthal; Thomas Goodwillie; H. Hauschild; Mark Hovey; S. Illman; Wolfgang Lück; L. Gaunce Lewis Jr.; Cary Malkiewich; J. Peter May and the named contributors to his CBMS volume; Mona Merling; Brian Munson; Ismar Volić; Unni Namboodiri; Richard Palais; Charles Rezk**, as well as Yeakel and Klang's earlier work.

The bibliography ledger preserves each printed entry rather than collapsing repeated people.

## 14. Reading order

1. Keep the \(C_2\) reflection example in hand.
2. Read Yeakel's isovariant Elmendorf theorem for the model category and diagram language.
3. Read the cell-structure and Whitehead sections of Klang–Yeakel 2023.
4. Read the fixed-point/Reidemeister-trace application.
5. Read the 2026 Blakers–Massey theorem, first in the square case and then for cubes.
6. Work the \(C_2\) and \(C_3\) representation examples.
7. Only then speculate about an isovariant stabilization or calculus.
