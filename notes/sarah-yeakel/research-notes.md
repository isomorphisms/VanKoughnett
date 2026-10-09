# Sarah Yeakel: research notebook

Checked 2026-10-09. Independently written study notes, not transcripts, a proof audit, or an identification of the person remembered in the original conversation.

Scope: the seven research papers and one dissertation listed on [Sarah Yeakel's research page](https://sites.google.com/view/syeakel/research). The expository guide has its own [reading note](goodwillie-and-imagery.md). These are first-pass notes; reading depth is stated for each item.

## 1. Unbased calculus for functors to chain complexes

**Maria Basterra, Kristine Bauer, Agnès Beaudry, Rosona Eldred, Brenda Johnson, Mona Merling, and Sarah Yeakel.** Preprint 2014; *Women in Topology: Collaborations in Homotopy Theory*, Contemporary Mathematics 641 (2015).

[Primary record](https://arxiv.org/abs/1409.1553) · [Text](https://arxiv.org/html/1409.1553)

**Read:** abstract and introduction.

The goal is a discrete calculus tower for functors from an unbased simplicial model category to chain complexes over a fixed commutative ring. The delicate point is not merely drawing the tower: an explicit homotopy-limit construction must support the strict identities needed for a cotriple. An argument for a simplicial target cannot simply be reused for chain complexes.

Keep the discrete tower, written with Γ, distinct from Goodwillie's n-excisive tower. The introduction explicitly distinguishes degree n from n-excision; the implications are not automatically reversible.

**Study question:** construct the first discrete approximation for a concrete algebraic functor, recording which identities are strict and which hold only up to weak equivalence.

## 2. Goodwillie calculus and I — dissertation

**Sarah Yeakel.** University of Illinois at Urbana–Champaign, 2016; adviser **Randy McCarthy**.

[Official dissertation record](https://www.ideals.illinois.edu/handle/2142/90811)

**Read:** institutional metadata and abstract; author-maintained description and warning. The dissertation itself has not been read end to end.

The institutional title is *Goodwillie calculus and I*. Yeakel's website labels the link *Goodwillie calculus and injections*. Here I denotes the indexing category of finite sets and injections, not an unidentified spectrum.

The thesis studies an injection-indexed model for functor calculus and a classification of certain finitary n-excisive functors to spectra using modules over a spectral monoid.

**Author warning:** Yeakel explicitly flags errors concerning cross-effects. The old abstract's monoidal-derivative and chain-rule claims must not be imported as established theorems. The 2018 revision below has a narrower conclusion. The warning does not, by itself, establish which other thesis results survive; that needs a separate proof-level check.

## 3. A lax monoidal model for multilinearization

**Sarah Yeakel.** *Homology, Homotopy and Applications* 22(1) (2020), 319–331. The arXiv v2 title is *A Monoidal Model for Multilinearization*; the 2017 version and guide used *A Monoidal Model for Goodwillie Derivatives*.

[Version history and correction notice](https://arxiv.org/abs/1706.06915) · [2018 revision, full text](https://arxiv.org/html/1706.06915v2)

**Read:** introduction, definitions 2.1 and 3.1, lemma 2.4, theorem 3.2, remark 3.3, conclusion, and bibliography. Not a complete verification of the proof.

The corrected theorem concerns **multilinearization of multipointed symmetric functor sequences**, evaluated at the zero-sphere. That functor is lax monoidal. An injection-indexed linearization is

$$\mathbb D_1F(X)=\operatorname*{hocolim}_{U\in\mathbb I}\Omega^U F(\Sigma^U X).$$

Here U is a finite set, and its size counts suspension and loop coordinates. Agreement with ordinary multilinearization requires the stated connectivity hypotheses. Lax monoidal means coherent comparison maps, not automatic equivalences.

The remaining cross-effects step is explicitly conditional in the revised conclusion. Do not replace this theorem by the stronger assertion that the entire Goodwillie-derivative functor has been proved monoidal in this paper.

## 4. Infinite loop spaces from operads with homological stability

**Maria Basterra, Irina Bobkova, Kate Ponto, Ulrike Tillmann, and Sarah Yeakel.** Preprint 2016; *Advances in Mathematics* 321 (2017), 391–430. Yeakel's site shortens the title to *Operads with Homological Stability*.

[Primary record](https://arxiv.org/abs/1612.07791)

**Read:** abstract and author summary; bibliography leads surfaced, but not audited against the full paper.

Suitable homological-stability conditions on an operad imply that group completions of its algebras are infinite loop spaces. This generalizes the surface-operad setting and admits examples from moduli spaces of even-dimensional manifolds. An action on middle-dimensional homology yields an infinite-loop map to algebraic K-theory.

**Connection to the seminar:** this goes from geometric operations to infinite loop spaces and spectra, rather than starting with a spectrum and forgetting structure.

**Study question:** distinguish surface gluing, stabilization, group completion, and infinite delooping. A picture of pants composition alone does not certify the stability hypotheses or the resulting infinite-loop structure.

## 5. Inverting operations in operads

**Maria Basterra, Irina Bobkova, Kate Ponto, Ulrike Tillmann, and Sarah Yeakel.** Preprint 2016; *Topology and its Applications* 235 (2018), 130–145.

[Primary record](https://arxiv.org/abs/1611.00715)

**Read:** abstract and author summary.

Given an operad and a submonoid of its unary operations, the construction makes those operations homotopy invertible. The construction adapts the Dwyer–Kan hammock localization, and relates algebras over the original and localized operads by an appropriate universal property. Yeakel's summary also records preservation of operads with homological stability.

The scope is **specified unary operations**, not indiscriminately inverting every multi-input operation. “Homotopy invertible” must not be displayed as a strict two-sided inverse without the required homotopies.

**Study question:** begin with labelled operation trees and selected reversible unary edges; then explain what coherent localization adds beyond reversing arrows in a graph.

## 6. An isovariant Elmendorf's theorem

**Sarah Yeakel.** Preprint 2019; *Documenta Mathematica* 27 (2022), 613–628.

[Primary record](https://arxiv.org/abs/1907.12135)

**Read:** abstract and author summary.

An isovariant map is equivariant and preserves each point's stabilizer exactly. For a finite group, Yeakel develops a model-categorical account and a diagram-category comparison analogous to Elmendorf's theorem. The later work explains the need to adjoin a formal terminal object to the isovariant category.

**Elementary distinction:** equivariance implies that the stabilizer of x is contained in that of its image; isovariance requires equality. Sending a free orbit into a fixed point is therefore excluded.

**Study question:** use a reflection action on a disk, with its fixed diameter marked. Show stabilizer types separately from their geometric location. Orbit-type information alone should not be asserted to contain the complete link data used by the theorem.

## 7. Isovariant homotopy theory and fixed point invariants

**Inbar Klang and Sarah Yeakel.** Preprint 2021; *Advances in Mathematics* 433 (2023), 109298.

[Primary record](https://arxiv.org/abs/2110.07853)

**Read:** abstract and author summary.

For a compact smooth manifold with a finite-group action, the paper investigates eliminating fixed points of self-maps by isovariant homotopy. Under dimension and codimension conditions on fixed-point subspaces, the equivariant Reidemeister trace is a complete obstruction to this elimination. The work also develops isovariant tools including a Whitehead theorem.

Two uses of “fixed” must remain separate: a point fixed by the self-map and a point fixed by a subgroup of the acting group.

**Study question:** maintain separate displays for the self-map equation f(x)=x and for the stabilizer of x. Do not present vanishing trace as sufficient when the geometric hypotheses have not been checked.

## 8. An isovariant Blakers–Massey theorem

**Inbar Klang and Sarah Yeakel.** Preprint 2025; *Journal of Homotopy and Related Structures* (2026).

[Primary record](https://arxiv.org/abs/2506.21259) · [Text](https://arxiv.org/html/2506.21259)

**Read:** abstract and introduction, including the stated theorem and suspension difficulty.

The authors prove isovariant Blakers–Massey and higher-cubical versions, then an isovariant Freudenthal theorem. Connectivity is indexed by strictly increasing subgroup chains, not just one integer. They construct a suitable suspension by a trivial representation sphere; this is not a completed theory of suspension by all representations.

A conceptual obstruction matters: a point is not terminal among ordinary G-spaces with isovariant maps. One cannot blindly reuse the usual suspension construction through maps to a point.

**Connection to the seminar:** revisit the relationship among suspension, homotopy pushouts, homotopy pullbacks, and eventual stability, now with stabilizer constraints.

## Attribution and reading limits

Thank you to each named author for these papers and public explanations. Bibliography-level acknowledgments and the exact limits of the linked-source traversal are recorded in [the attribution ledger](../users-guides/ACKNOWLEDGMENTS.md) and [coverage log](../users-guides/crawl-log.md).

Nothing in this notebook identifies the originally remembered “K-bar spectrum.” The mathematical interest in Yeakel's work does not depend on that identification.
