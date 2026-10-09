# Agnès Beaudry — parametrized quantum phases and matrix-product-state classifying spaces

Checked 2026-10-09. This is a focused continuation of [research-notes.md](research-notes.md). Beaudry's chromatic-homotopy work remains central to the overview notebook; this file follows the newer mathematical-physics branch in detail.

## Primary sources

- Agnès Beaudry, Michael Hermele, Juan Moreno, Markus J. Pflaum, Marvin Qi, Daniel D. Spiegel, [*Homotopical Foundations of Parametrized Quantum Spin Systems*](https://arxiv.org/abs/2303.07431), Rev. Math. Phys. 36 (2024).
- Agnès Beaudry, Michael Hermele, Markus J. Pflaum, Marvin Qi, Daniel D. Spiegel, David T. Stephen, [*A Classifying Space for Phases of Matrix Product States*](https://arxiv.org/abs/2501.14241) (2025).
- Xueda Wen, Marvin Qi, Agnès Beaudry, Juan Moreno, Markus J. Pflaum, Daniel Spiegel, Ashvin Vishwanath, Michael Hermele, *Flow of higher Berry curvature and bulk-boundary correspondence in parametrized quantum systems*, Phys. Rev. B 108 (2023).
- Beaudry's [University of Colorado research page](https://www.colorado.edu/math/agnes-beaudry) for the connection to chromatic and equivariant stable homotopy.

The complete 37-entry bibliography of the 2025 MPS classifying-space paper is credited entry-by-entry in [../researchers/ACKNOWLEDGMENTS.md](../researchers/ACKNOWLEDGMENTS.md).

## 1. The homotopy-theoretic question

A single gapped quantum ground state is not the whole object of interest. One can have a **family** of quantum systems parametrized by a topological space \(X\). The family may return to the same local Hamiltonian data after going around a loop while accumulating global topological information.

The natural classification problem is

\[
\{\text{families over }X\}/\text{deformation}
\quad\leftrightarrow\quad
[X,\mathcal Q],
\]

for a suitable classifying space \(\mathcal Q\) of phases.

Kitaev's proposed picture goes further: spaces of invertible phases in different spatial dimensions should fit together into a spectrum. Stable homotopy is therefore more than borrowed vocabulary; the spectrum is meant to encode dimensional suspension/looping of phases.

## 2. Quantum state types

The 2024 foundations paper defines **quantum state types** as certain lax-monoidal functors from finite-dimensional Hilbert spaces to topological spaces.

The monoidal structure records **stacking** of quantum systems. If two states live on Hilbert spaces \(\mathcal H_1\) and \(\mathcal H_2\), stacking corresponds to tensor product on

\[
\mathcal H_1\otimes\mathcal H_2.
\]

Passing to large on-site Hilbert spaces and imposing invertibility gives an \(E_\infty\)-type multiplication. For an invertible quantum state type, the resulting space is an infinite loop space and therefore the zero space of a loop spectrum.

The paper also proves that the pure-state space of a UHF algebra is simply connected, an initial calculation toward understanding the universal state-type space.

## 3. Why matrix product states are a tractable test case

In one spatial dimension, injective **matrix product states (MPS)** give a concrete finite-tensor description of an important class of gapped ground states.

An MPS tensor has components

\[
A^i_{\alpha\beta},
\]

where \(i\) is the physical index and \(\alpha,\beta\) are bond indices. For an injective tensor, the matrices \(A^i\) span the full matrix algebra on the bond space.

Two tensors may describe the same physical state because of gauge freedom. In a normalized form, the essential gauge action includes a phase and unitary conjugation.

This makes the moduli problem explicit enough to topologize.

## 4. Allowing dimensions to vary

A fixed bond dimension is too rigid for a global classifying space: continuous families can pass through descriptions with different bond dimensions.

The 2025 paper constructs a large tensor space \(\mathcal E\) by embedding finite tensors in infinite arrays with only finitely many nonzero entries. It then takes the appropriate gauge quotient to form

\[
p:\mathcal E\longrightarrow\mathcal B.
\]

The construction is designed so physical and bond dimensions can change along a path.

This is a crucial choice: the topology must see families, not just classify individual finite tensors up to algebraic equivalence.

## 5. The total space is contractible

The authors prove

\[
\mathcal E\simeq *.
\]

If \(p\) were an ordinary fiber bundle with a fixed fiber \(F\), one would immediately expect the base to behave like \(BF\). But the fibers change their concrete presentation with essential rank, so \(p\) is not globally a fiber bundle.

The replacement is the next key theorem.

## 6. The quotient map is a quasifibration

They prove

\[
p:\mathcal E\to\mathcal B
\]

is a **quasifibration**.

A quasifibration allows nontrivial variation in the fibers but still gives the long exact homotopy sequence as though one had a fibration.

For a point of essential rank \(\chi\), the fiber has homotopy type

\[
\mathcal F(\chi)
\simeq
U(1)\times BU(1)
\simeq
K(\mathbb Z,1)\times K(\mathbb Z,2),
\]

independent of \(\chi\) at the level of homotopy type.

Since the total space is contractible, this shifts the fiber's homotopy groups up by one in the base.

## 7. Main classifying-space theorem

The classifying space has weak homotopy type

\[
\boxed{
\mathcal B\simeq_w K(\mathbb Z,2)\times K(\mathbb Z,3)
}
\]

and therefore

\[
\pi_n(\mathcal B)=
\begin{cases}
\mathbb Z,&n=2,3,\\
0,&\text{otherwise}.
\end{cases}
\]

For a parameter space \(X\), homotopy classes of families are consequently classified by

\[
[X,\mathcal B]
\cong
H^2(X;\mathbb Z)\times H^3(X;\mathbb Z)
\]

in the translation-invariant injective-MPS setting of the paper.

## 8. Meaning of the two classes

### \(H^2\)

The \(H^2\)-class is a **Chern number per unit cell**. It persists here because the construction imposes translation invariance. The authors note that without translation invariance one expects this part can be pushed to the boundary/infinity; that broader statement is motivation, not yet their theorem.

### \(H^3\)

The \(H^3\)-class is the **Kapustin–Spodyneiko invariant**, interpretable as a higher Berry-curvature flow. It is the genuinely one-dimensional part emphasized by the Chern-number-pump example.

Thus the product \(K(\mathbb Z,2)\times K(\mathbb Z,3)\) has two geometric/physical invariants behind it.

## 9. The \(S^2\) and \(S^3\) generators

The paper gives maps

\[
\psi_2:S^2\to\mathcal B,
\qquad
\psi_3:S^3\to\mathcal B.
\]

The \(S^2\) family generates \(\pi_2(\mathcal B)\) and corresponds to a zero-dimensional Chern-type phase repeated at every site.

The \(S^3\) family is the **Chern number pump** and generates

\[
\pi_3(\mathcal B)\cong\mathbb Z.
\]

In the long exact sequence of the quasifibration, the generator can be recognized through the \(BU(1)\simeq\mathbb CP^\infty\) part of the fiber.

This is an unusually concrete stable-homotopy example: one can draw or numerically animate an actual family of tensors parameterized by a sphere and know which homotopy group it represents.

## 10. Gauge freedom and topology

For fixed bond dimension, normalized injective MPS tensors are quotiented by gauge freedom involving \(U(1)\) and unitary changes of bond basis.

The global construction has to enlarge this because bond dimension changes. Tensor representatives live in a contractible ambient space, while the quotient retains topology of the gauge ambiguity.

This is analogous to familiar classifying-space constructions

\[
EG\to BG
\]

with contractible \(EG\), but the MPS map is technically a quasifibration rather than a single free group action with constant fiber. Treating it literally as a principal bundle would be wrong.

## 11. Topology of the pure-state space

The authors map their MPS quotient into the pure-state space of the quasi-local \(C^*\)-algebra. A subtlety is that the natural weak-* topology on pure states is not always fine enough for the MPS quotient map to be an embedding.

They exhibit behavior related to interpolation toward a product state/AKLT-type state where the quotient topology detects a discontinuity associated with a phase transition.

This warns that choosing the “obvious topology” on the physical state space can erase exactly the family information a homotopy classification is supposed to retain.

## 12. Relation to Beaudry's chromatic work

Beaudry's other work includes:

- height-two Morava stabilizer groups and duality resolutions;
- the chromatic splitting conjecture at \(n=p=2\);
- dualizing spheres for compact \(p\)-adic analytic groups with Paul Goerss, Michael Hopkins, and Vesna Stojanoska;
- Lubin–Tate models via real bordism with Michael Hill, XiaoLin Danny Shi, and Mingcong Zeng;
- computational guides to Adams spectral sequences with Jonathan Campbell.

The quantum-phase project is not an application of Morava \(E\)-theory in the 2025 paper. The connection is methodological: use stable homotopy and classifying spaces to organize families and invertible objects.

Do not collapse the two branches into “chromatic quantum phases” without an explicit theorem doing so.

## 13. Visual and computational opportunities

### MPS gauge orbit

Show a tensor \(A\), its unitary conjugates, and the quotient point they represent. Let physical/bond dimensions change along a path.

### Quasifibration picture

Draw \(\mathcal E\) as a contractible total space over \(\mathcal B\), with fibers homotopy equivalent to \(U(1)\times BU(1)\). Animate how different finite-rank presentations still have the same fiber homotopy type.

### Sphere families

Display the \(S^2\) and \(S^3\) parameter spaces and track Berry/Chern data around them. The \(S^3\) pump is especially suitable for a rotatable three-dimensional parameter visualization.

### Cohomology classifier

For a chosen finite CW parameter space \(X\), compute \(H^2(X;\mathbb Z)\) and \(H^3(X;\mathbb Z)\) and display corresponding labels for MPS families.

## 14. Credit and provenance

The classifying-space paper is joint work of **Agnès Beaudry, Michael Hermele, Markus J. Pflaum, Marvin Qi, Daniel D. Spiegel, and David T. Stephen**. The authors thank **Michael Hopkins, Alexei Kitaev, and Bruno Nachtergaele** for helpful conversations.

Its complete 37-entry bibliography is credited in the central ledger, including translators and editors where the source names them. Particularly important antecedents include work of **Ian Affleck, Tom Kennedy, Elliott Lieb, Hal Tasaki; M. Fannes, B. Nachtergaele, R. F. Werner; Jutho Haegeman, Michaël Mariën, Tobias Osborne, Frank Verstraete; Anton Kapustin, Lev Spodyneiko; Shuhei Ohyama, Shinsei Ryu; Marvin Qi and collaborators**, and the other authors named there.

## 15. Reading order

1. Read the quantum-state-type definition in the 2024 foundations paper.
2. Understand why stacking produces \(E_\infty\)-structure and why invertibility produces an infinite loop space.
3. In the 2025 paper, understand injective MPS and the gauge relation first.
4. Follow the construction of \(\mathcal E\) and \(\mathcal B\).
5. Read contractibility of \(\mathcal E\) and the quasifibration theorem.
6. Derive \(K(\mathbb Z,2)\times K(\mathbb Z,3)\) from the fiber.
7. Work the \(S^2\) and Chern-pump \(S^3\) examples.
