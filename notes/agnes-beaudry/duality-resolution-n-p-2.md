# Agnès Beaudry — the duality resolution at \(n=p=2\)

Checked 2026-10-09. Focused notes on **Agnès Beaudry, Irina Bobkova, and Hans-Werner Henn, *The duality resolution at \(n=p=2\)*, arXiv:2502.03141**. The inspected HTML is dated 2026-08-24.

The paper's complete eleven-entry bibliography is credited in [../researchers/ACKNOWLEDGMENTS.md](../researchers/ACKNOWLEDGMENTS.md).

## 1. What is being resolved?

Fix height \(2\) and prime \(2\). Let \(E=E_2\) be Morava \(E\)-theory over \(\mathbb F_4\). The extended Morava stabilizer group is

\[
\mathbb G_2=\mathbb S_2\rtimes \operatorname{Gal}(\mathbb F_4/\mathbb F_2),
\]

and \(\mathbb G_2^1\) is the norm-one subgroup.

The target of the paper is the homotopy-fixed-point spectrum

\[
E^{h\mathbb G_2^1}.
\]

This is closely related to, but is **not**, the entire \(K(2)\)-local sphere

\[
L_{K(2)}S^0\simeq E^{h\mathbb G_2}.
\]

That distinction is essential.

## 2. Main topological resolution

The paper constructs a finite resolution

\[
E^{h\mathbb G_2^1}
\longrightarrow
E^{hG_{48}}
\longrightarrow
E^{hG_{12}}
\longrightarrow
E^{hG_{12}}
\longrightarrow
\Sigma^{48}E^{hG_{48}}.
\]

Here \(G_{48}\) and \(G_{12}\) are finite subgroups of the extended stabilizer group described in the paper.

The last term is not guessed from numerical periodicity: the authors construct a final cofiber \(X\), identify its Morava module with that of \(E^{hG_{48}}\), and then prove

\[
X\simeq \Sigma^{48}E^{hG_{48}}.
\]

So the resolution turns a spectrum defined using the large profinite group \(\mathbb G_2^1\) into a finite sequence involving homotopy fixed points by finite subgroups.

## 3. What this upgrades

Earlier work supplied a duality resolution for

\[
E^{h\mathbb S_2^1},
\]

where \(\mathbb S_2^1\) is the norm-one subgroup of the stabilizer group *without* adjoining the Galois action.

The new paper upgrades that construction to

\[
E^{h\mathbb G_2^1}
\]

and therefore keeps track of

\[
\operatorname{Gal}(\mathbb F_4/\mathbb F_2).
\]

This sounds like “just add Galois fixed points,” but that is precisely what does **not** work: the maps in the older resolution are not Galois-equivariant. The new resolution has to be constructed from scratch with Galois-twisted module structure built into it.

That is the conceptual center of the paper.

## 4. Algebraic resolution first

The topological construction is preceded by an exact sequence of complete Galois-twisted modules over the completed group ring.

Very schematically,

\[
0\to \mathcal D_3\to \mathcal D_2\to
\mathcal D_1\to \mathcal D_0\to \mathbb W\to 0,
\]

with

\[
\mathcal D_0=
\mathbb W\uparrow^{P\mathbb G_2^1}_{PG_{48}},
\qquad
\mathcal D_1=
\mathbb W\uparrow^{P\mathbb G_2^1}_{PG_{12}},
\]

\[
\mathcal D_2=
\mathbb W\uparrow^{P\mathbb G_2^1}_{PG_{12}},
\qquad
\mathcal D_3=
\mathbb W\uparrow^{P\mathbb G_2^1}_{PG'_{48}}.
\]

The notation \(\uparrow\) denotes completed induction from the indicated finite subgroup.

The procedure therefore has two distinct levels:

1. build an exact algebraic resolution of the trivial/Galois-twisted module;
2. realize that algebraic resolution by actual maps of homotopy-fixed-point spectra.

A visualization or formalization should not merge these levels. Exactness of completed modules is not automatically a topological cofiber sequence.

## 5. Why finite subgroups help

The Morava stabilizer group is profinite and complicated. Finite subgroups such as \(G_{48}\) and \(G_{12}\) are much more rigid computational inputs.

The resolution gives a spectral-sequence machine: information about the homotopy of the finite-subgroup fixed-point spectra can be assembled into information about \(E^{h\mathbb G_2^1}\).

This is the same broad strategy behind the prime-\(3\) Goerss–Henn–Mahowald–Rezk resolution, but the prime-\(2\) geometry and Galois bookkeeping differ.

## 6. Why the full \(K(2)\)-local sphere is not obtained

The authors explicitly warn that the resolution cannot simply be doubled to resolve

\[
E^{h\mathbb G_2}\simeq L_{K(2)}S^0.
\]

At \(p=2\), resolving the full group requires a larger construction, such as Henn's centralizer resolution.

Thus the phrase “duality resolution at \(n=p=2\)” should not be abbreviated in our notes to “a finite resolution of the \(K(2)\)-local sphere.” The paper resolves the norm-one half \(E^{h\mathbb G_2^1}\).

## 7. The two formal-group models

The paper works with either

- the height-two Honda formal group \(\Gamma_H\), or
- the formal group \(\Gamma_E\) of the supersingular elliptic curve
  \[
  y^2+y=x^3.
  \]

Their stabilizer groups \(\mathbb S_2(\Gamma_H)\) and \(\mathbb S_2(\Gamma_E)\) are isomorphic in the manner described in the paper. But a warning immediately follows: that isomorphism is not compatible with the Galois action, and

\[
\mathbb G_2(\Gamma_H)\not\cong \mathbb G_2(\Gamma_E)
\]

in the corresponding way.

This is another place where “the underlying groups are isomorphic” does not mean all equivariant structure can be transported without cost.

## 8. A small algebraic model for why equivariance matters

Suppose an exact sequence of abelian groups

\[
0\to A\to B\to C\to 0
\]

has an involution on each object. Taking fixed points is left exact but need not preserve surjectivity. Even before any spectra appear, “take the old resolution and then take fixed points” can fail.

The paper's problem is much richer—completed group rings, twisted modules, and a Galois action—but this elementary fact explains why the obstruction is structurally plausible.

The correct lesson is not that fixed points are bad. It is that an equivariant resolution must encode equivariance in its maps.

## 9. Relation to Beaudry's earlier work

This paper sits at the end of a long chain:

- **Goerss–Henn–Mahowald–Rezk**: prime-\(3\) duality resolution;
- **Beaudry**: algebraic duality resolution at \(p=2\);
- **Bobkova–Goerss**: topological realization for \(E^{h\mathbb S_2^1}\);
- **Beaudry–Goerss–Henn**: chromatic splitting calculations using this machinery;
- **Beaudry–Bobkova–Goerss–Henn–Pham–Stojanoska**: exotic \(K(2)\)-local Picard group;
- **Beaudry–Bobkova–Henn**: the Galois-compatible resolution for \(E^{h\mathbb G_2^1}\).

So the new resolution is not a separate theme from the older Beaudry material. It is a structural upgrade of a computational machine that already powered several of those calculations.

## 10. What to visualize

### Resolution as a finite machine

Display the five spectra in a row and attach, below each, the finite subgroup producing it. A second row should show the corresponding induced Morava modules. Vertical arrows distinguish “realization” from horizontal resolution maps.

### Group inclusions

Show

\[
\mathbb S_2^1\subset \mathbb G_2^1\subset \mathbb G_2
\]

with the Galois quotient marked separately. This makes it difficult to accidentally identify the old and new resolutions.

### Algebraic/topological toggle

For each stage, let the display switch between the completed induced module and the homotopy-fixed-point spectrum. A successful implementation should never allow the two to share the same type merely because one realizes the other.

## 11. Credit and provenance

The paper is joint work of **Agnès Beaudry, Irina Bobkova, and Hans-Werner Henn**.

The authors explicitly thank **Mark Behrens, Paul Goerss, Vesna Stojanoska, and Viet-Cuong Pham** for many conversations related to the work.

Its eleven bibliography entries are individually credited in the central ledger. These notes paraphrase the paper and distinguish inspected results from independent explanatory examples.

## 12. Reading order

1. Read the introduction through Theorem 1.2 and the warning about the full \(K(2)\)-local sphere.
2. Review the distinction \(\mathbb S_2^1\) versus \(\mathbb G_2^1\).
3. Read the finite-subgroup section and make a subgroup diagram.
4. Read Theorem 3.4 as an algebraic statement before looking at the topological realization.
5. Follow the three short exact sequences used to splice the algebraic resolution.
6. Read Section 4 only after the module-level maps are clear.
7. Finish with the proof that the final cofiber is \(\Sigma^{48}E^{hG_{48}}\).
