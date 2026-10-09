# Cary Malkiewich: a friendly bridge from spectra to algebraic K-theory

[Guide catalogue](README.md) · [Yeakel K-theory trail](../sarah-yeakel/k-theory-and-trace-methods.md) · [Followed references](followed-references.md)

Checked 2026-10-09. This is a close reading of all four parts of **Cary Malkiewich's 2015 Enchiridion user's guide** to _Coassembly and the K-theory of finite groups_, together with the source-paper abstract. It is especially useful after Sarah Yeakel's material because it turns several nearby abstractions—spectra, algebraic K-theory, assembly/coassembly, transfer, norm, and (K(n))-localization—into concrete pictures.

[Enchiridion landing page](https://mathusersguides.com/enchiridion-vol-1-2015-cary-malkiewich/) · [Source paper](https://arxiv.org/abs/1503.06504)

## 1. The spectrum picture

Malkiewich starts with a spectrum as a sequence

[
X_0,;X_1,;X_2,ldots
]

with structure maps (Sigma X_n	o X_{n+1}).

His useful mental move is to talk about an “element” of a spectrum as a compatible stable family of sphere maps

[
S^nlongrightarrow X_n.
]

Degree (k) elements are represented by compatible maps (S^{n+k}	o X_n). Their homotopy classes are (pi_kX).

This language is deliberately informal, but it gives a good bridge from ordinary elements of an abelian group to stable homotopy classes. Addition comes from pinching spheres, with the choices becoming coherently commutative in the stable range.

### Picture caution

A spectrum is **not** literally the ordinary colimit of its spaces, and an element is not literally one point simultaneously living in every level. The compatible-sphere picture is a model for stable homotopy classes, useful precisely because suspension shifts the geometry from level to level.

## 2. Ring spectra and perfect modules

If (R) is a ring spectrum, an (R)-module spectrum behaves like a generalized module whose generators and relations can occupy different degrees. A perfect (R)-module is built, up to retract, from finitely many (R)-cells.

This is the spectrum-level analogue of a finitely generated projective module over an ordinary ring.

That gives a concrete input category for algebraic K-theory:

[
K(R)=K(mathrm{Perf}(R)).
]

## 3. What (K(R)) remembers

At the zeroth-space level, points represent perfect modules and paths represent equivalences. The Waldhausen construction then adds higher cells encoding additivity. In a cofiber sequence

[
Alongrightarrow Xlongrightarrow X/A,
]

algebraic K-theory remembers the relation

[
[X]=[A]+[X/A].
]

So (K(R)) is not merely a moduli space of modules. It is a homotopy-coherent group-completion-type construction that forces additivity across cofiber sequences.

This is one reason computation becomes difficult: the object is designed to retain subtle global information while imposing many coherent relations.

## 4. Group rings as families over (BG)

For a topological group (G), modules over (R[G]) can be viewed as families of (R)-modules over the classifying space (BG), with (G)-action encoded as monodromy around loops.

That turns

[
K(R[G])
]

into something that can be approached as K-theory of parametrized (R)-modules over (BG).

This is the key geometric change of coordinates in the guide.

## 5. Assembly

The assembly map is

[
BG_+wedge K(R)longrightarrow K(R[G]).
]

At a concrete module level, start with a perfect (R)-module (M). Inducing it up to the group ring produces roughly a (G)-indexed collection of copies of (M), with the group action remembering how those copies permute.

From the functor-calculus viewpoint, assembly is also the universal **linear/homological approximation** to the relevant functor on spaces. This is the direct bridge back to Goodwillie calculus.

## 6. Coassembly

The dual construction takes a parametrized family and asks for its fibers pointwise:

[
G^R(R[G])longrightarrow F(BG_+,K(R)).
]

The finiteness condition matters. A perfect (R[G])-module need not automatically have a perfect underlying (R)-module in arbitrary situations. The correct source is therefore Swan theory (G^R(R[G])), with a Cartan map from ordinary K-theory in the finite-group setting.

A good mental picture is:

- assembly: build a global family from local/module data;
- coassembly: inspect a global family through its fibers.

They are not inverse maps.

## 7. Transfer as “sum all the preimages”

For a finite covering, there is generally no continuous way to choose one preimage of every point. But a spectrum lets us **sum all the preimages**.

As the basepoint travels around a loop, those preimages can be permuted. The transfer remembers this monodromy rather than trying to order the fiber once and for all.

This is one of the cleanest places where symmetric-group coherence becomes visible geometrically.

## 8. The norm

For a spectrum (X) with a finite-group action, the equivariant norm compares homotopy orbits and homotopy fixed points:

[
N:X_{hG}longrightarrow X^{hG}.
]

The guide's main theorem identifies the composite

[
BG_+wedge K(R)
longrightarrow K(R[G])
longrightarrow G^R(R[G])
longrightarrow F(BG_+,K(R))
]

with the norm on (K(R)) with trivial (G)-action.

The intuitive reason is additivity: inducing (M) produces a (G)-fold sum of copies of (M), and transfer/norm constructions are also coherent (G)-fold sums with monodromy.

The proof is not merely “both maps look like sums.” A substantial part of the paper constructs compatible models and checks the monodromy and transfer identifications.

## 9. Why (K(n)) appears

For finite (G), the norm becomes an equivalence after suitable chromatic localization, because the corresponding Tate construction vanishes (K(n))-locally. Malkiewich therefore gets splitting results for assembly and coassembly after (K(n))-localization.

This is worth keeping visibly separate from two other uses of K:

- (K(R)): **algebraic K-theory** of a ring or ring spectrum;
- (K(n)): **Morava K-theory**, a chromatic homology theory used for localization.

The paper contains both notations in close proximity. That is exactly the kind of setting in which a remembered “K-bar spectrum” could drift, but it still does not identify the original recollection.

## 10. A structural parallel with Yeakel

The two projects are not the same, but they share a useful design lesson.

### Yeakel

A sequential indexing category forgets too much permutation data. Enlarge it to finite sets and injections so composition can retain the symmetry needed for coherent operations.

### Malkiewich

A transfer cannot continuously pick one point from a finite fiber. Instead, add **all** points in the fiber, and retain the monodromy that permutes them.

In both cases, the symmetry is not an annoyance to quotient away. It is part of the mathematical object that makes the construction coherent.

This is a potentially useful design principle for visualizations in this repository: **show the permutation/monodromy rather than freezing an arbitrary ordering.**

## 11. The development story is mathematically useful

Malkiewich's Topic 3 records a route through several failed conjectures and changes of model:

- contravariant Goodwillie calculus suggested looking at coassembly;
- a proposed dual Novikov statement proved too optimistic;
- learning THH, TC, genuine (G)-spectra, and (p)-completion produced more tractable intermediate calculations;
- a THH splitting did not automatically lift to TC or K-theory;
- reinterpreting the maps as an equivariant norm and then lifting the argument to finite sets produced the cleaner final K-theory argument.

This is a good complement to Yeakel's own development story. In both, the important work consists partly in learning **which attractive formal analogy fails**, then changing the model until the coherence or finiteness problem is actually represented.

## 12. Reading order

For the quickest route:

1. Topic 2.1: the “elements of spectra” picture;
2. Topic 2.2: K-theory as additivity/group completion of perfect modules;
3. Topic 2.3: assembly and coassembly through bundles over (BG);
4. Topic 2.4: transfer and norm;
5. Topic 1: return for the exact theorem and hypotheses;
6. Topic 3: read the false starts after the mathematics is recognizable;
7. the source paper for proofs.

This is one of the friendliest bridges in the Enchiridion collection from basic stable-homotopy language to a real chromatic/K-theoretic result.

## Credits from the guide

The guide and its story directly invoke or cite work of **J. F. Adams, Ian Hambleton, Laurence R. Taylor, Bruce Williams, Daniel S. Kahn, Stewart B. Priddy, Cary Malkiewich, J. Peter May, Johann Sigurdsson, Friedhelm Waldhausen, Bruce Williams, John Klein, Daniel Litt, Ralph Cohen, Gunnar Carlsson, Mark Behrens, and Randy McCarthy**.

Thank you to all of them. Bibliographic acknowledgment here means the source used or discussed their work; it does not imply that every cited paper has been read in this notebook.
