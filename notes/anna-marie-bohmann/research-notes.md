# Anna Marie Bohmann: research notebook

Checked 2026-10-09. Independent mathematical notes, with worked examples written for this repository. This is a first research survey, not a claim that every listed paper has been read. The [author's Vanderbilt research page](https://math.vanderbilt.edu/bohmanar/research.html) is a useful discovery source but is not treated as a complete current publication list.

## Primary sources inspected

1. Anna Marie Bohmann and Angélica M. Osorno, [Constructing equivariant spectra via categorical Mackey functors](https://arxiv.org/html/1405.6126), arXiv:1405.6126v2; AGT 15 (2015). Abstract, introduction, construction outline, final application, and bibliography inspected.
2. Vigleik Angeltveit and Anna Marie Bohmann, [Graded Tambara functors](https://arxiv.org/html/1504.00668), arXiv:1504.00668v3; JPAA 222 (2018). Abstract, introduction, section structure, and bibliography inspected.
3. Anna Marie Bohmann, Teena Gerhardt, and Brooke Shipley, [Topological coHochschild Homology and the Homology of Free Loop Spaces](https://arxiv.org/html/2105.02267), arXiv:2105.02267. Abstract, selected final computations, and bibliography inspected.
4. Anna Marie Bohmann, Teena Gerhardt, Cary Malkiewich, Mona Merling, and Inna Zakharevich, [A trace map on higher scissors congruence groups](https://arxiv.org/html/2303.08172v2). Abstract, universal-measure example, and bibliography inspected.
5. Anna Marie Bohmann and Markus Szymik, [Boolean algebras, Morita invariance, and the algebraic K-theory of Lawvere theories](https://arxiv.org/abs/2011.11755), updated primary record inspected.

Complete bibliography-name checks for items 1–4 appear in [ACKNOWLEDGMENTS](../researchers/ACKNOWLEDGMENTS.md). Bibliographies of the remaining inventory are still pending.

## 1. Why ordinary group actions do not contain all the equivariant information

The Bohmann–Osorno construction takes categorical Mackey data to genuine equivariant spectra. It uses the Guillou–May model of G-spectra and a spectrally enriched construction built from K-theory of permutative categories. The applications include equivariant Eilenberg–MacLane spectra and suspension spectra of finite G-sets. [Paper 1](https://arxiv.org/html/1405.6126).

The following example is our elementary preparation for reading that construction, not a reconstruction of its enriched-category proof.

### The Burnside-ring example for a reflection group

Let G = C2, with identity e and nonidentity element tau. A finite C2-set splits into fixed singleton orbits and free two-element orbits. Let 1 denote a singleton fixed orbit, and let t denote a free orbit. Disjoint union gives addition, and Cartesian product with the diagonal action gives multiplication.

The product of two free orbits has four elements and no fixed points, hence two free orbits. Therefore

    t*t = 2*t,
    A(C2) = Z[t]/(t*t - 2*t).

An element a + b*t records virtual fixed and free orbits. Forgetting the action gives the restriction

    res(a + b*t) = a + 2*b.

Inducing an ordinary finite set to a free C2-set gives the additive transfer

    tr(n) = n*t.

Consequently res(tr(n)) = 2*n. The two maps cannot be identified: restriction forgets symmetry; transfer builds symmetry into the input.

For a proposed display, a point with a fixed-point badge and a paired orbit must remain different objects even when their total cardinalities agree. Two fixed points and one free orbit both contain two points, but the C2-sets are not isomorphic.

### What categorification adds

This elementary Burnside calculation uses isomorphism classes. A categorical construction retains objects, isomorphisms, and coherence information before applying K-theory. The paper's contribution is not merely the observation that a group acts on a category. Its Mackey-style input has compatible contravariant and covariant behavior, encoded with enriched structure. Do not substitute an arbitrary category with a C2-action and claim to have implemented the theorem.

A useful future specification would separate finite G-sets, equivariant maps, spans, pullback composition, and the categorical values assigned to them. Associativity of span composition up to canonical isomorphism is a coherence issue, not an excuse to erase the isomorphisms.

## 2. Tambara functors: multiplication indexed by an orbit

Angeltveit and Bohmann construct RO(G)-graded Tambara functors from G-spectra equipped with norm multiplication. The grading and its coherence are part of the theorem. A Mackey functor already has restrictions and additive transfers; a Tambara structure also records multiplicative norms and their distributivity laws. [Paper 2](https://arxiv.org/html/1504.00668).

### Independent finite-set calculation of a norm

Let S be a set with k elements, with k nonnegative. Form S × S, with C2 exchanging its two coordinates. Exactly k points lie on the diagonal and are fixed. The remaining k*k-k points occur in free pairs. Thus the multiplicative norm in this finite-set model is

    N(k) = k + (k*(k-1)/2)*t.

For k = 2, N(2) = 2 + t. Its underlying set has 2 + 2 = 4 elements. Compare this with the additive transfer tr(2) = 2*t: its underlying set also has four elements, but it has no fixed points. Equal cardinality does not imply equal equivariant data.

Expanding the same formula gives

    N(k+l) = N(k) + N(l) + k*l*t.

The extra term is the mixed-coordinate part. This calculation makes the difference between additive and multiplicative transfer visible without invoking any spectral machinery.

### Why representation grading matters

For C2, write sigma for the one-dimensional sign representation. A representation a*1 + b*sigma has underlying dimension a+b but fixed-subspace dimension a. Recording only a+b forgets data relevant to equivariant suspension. A degree should therefore retain the representation, not merely its ordinary dimension.

For an H-representation V, an indexed norm changes the suspension coordinate through an induced G-representation. It should not be typed as a degree-preserving endomorphism of an ungraded list. The full paper handles more coherence than this sketch; the sketch only identifies a concrete error that a model should prevent.

## 3. coTHH and free loops: do not confuse the graded module with a loop product

Bohmann, Gerhardt, and Shipley's Theorem 7.9 computes a free-loop-space homology group, under its simply-connected and odd-generator hypotheses, with underlying graded module

    H_*(LX; k) = Lambda_k(y) tensor k[w],
    degree(y) = degree(x),
    degree(w) = degree(x)-1,

when H^*(X;k) is exterior on the specified odd-degree generator x. Their following remark recovers odd-dimensional spheres and explicitly credits Wolfgang Ziller's earlier Morse-theoretic calculation. This should not be advertised as their first discovery of the sphere answer. [Paper 3, Theorem 7.9 and Remark 7.10](https://arxiv.org/html/2105.02267).

### Independent example: the graded sizes for LS3

Specialize the displayed module formula to degree(y)=3 and degree(w)=2. A basis consists of

    1, w, w^2, w^3, ...
    y, y*w, y*w^2, y*w^3, ...

The first row occupies degrees 0,2,4,6,... and the second 3,5,7,9,.... Therefore degree 1 is empty, and each degree at least 2 has one basis element over k. The formal size series is

    (1 + z^3)/(1 - z^2).

This is a deduction from the stated graded-module result. It does not identify a Chas–Sullivan product, a coproduct, or every extension in every spectral sequence. A program should label exactly which structure its calculation establishes.

Geometrically, a free loop has no preferred starting point fixed in X; a based loop does. A visualizer can mark a moving evaluation point on a free loop to expose the distinction. The appearance of loop-space homology does not turn an arbitrary animation of curves into a computation of that homology.

## 4. The scissors trace and the connection to Malkiewich

The joint paper of **Bohmann, Teena Gerhardt, Cary Malkiewich, Mona Merling, and Inna Zakharevich** constructs a trace from higher scissors-congruence groups to group homology. Its universal-measure case becomes a rational comparison of the specified polytope K-theory with group homology. See [Malkiewich's notebook](../cary-malkiewich/research-notes.md) for the distinction between a formal cutting relation and its higher comparison data, and [the primary text](https://arxiv.org/html/2303.08172v2) for the hypotheses.

This is a genuine shared paper, not just a thematic association between the two researchers. It also gives the repository a direct connection to Inna Zakharevich's assembler program.

## 5. Lawvere theories: an important version correction

The author research page still uses the combined title *Assembly and Morita invariance in the algebraic K-theory of Lawvere theories*. The updated [arXiv:2011.11755 record](https://arxiv.org/abs/2011.11755) separates that earlier work: the Morita/Boolean-algebra material has the title *Boolean algebras, Morita invariance, and the algebraic K-theory of Lawvere theories*, while assembly material moved to [arxiv:2112.07003](https://arxiv.org/abs/2112.07003). The former appeared in Mathematical Proceedings of the Cambridge Philosophical Society 175 (2023), 253–270.

Both records credit **Anna Marie Bohmann and Markus Szymik**. This pass inspected the version notice, not all arguments of the two resulting papers. Keep the split in the source ledger; do not cite the old combined title as though it were two separate original discoveries.

A reading question relevant to the language projects: what information about an algebraic theory is preserved by changing its presentation, and what additional structure does its K-theory detect? Morita equivalence, equivalence of chosen presentations, and a superficial similarity of syntax must not be conflated.

## 6. Remaining publication map

The following are author-index discovery records and prompts for close reading. They are not claims to have verified each result or inspected each bibliography.

| Strand | Located work and collaborators | Question to carry into the paper |
| --- | --- | --- |
| Equivariant detection | *Equivariant generating hypothesis*; *A presheaf interpretation of the generalized Freyd conjecture*, with **J. Peter May** | When does vanishing on homotopy groups imply that a map is zero, and what is the precise finite-object hypothesis? |
| Global structure | *Global orthogonal spectra* | How is compatibility across different groups encoded, beyond studying one group at a time? |
| Norm comparisons | *A comparison of norm maps*, with an appendix by **Bohmann and Emily Riehl** | Does the comparison respect all required multiplicative and change-of-group data? |
| Categorical models | *A model structure on GCat*, with **Kristen Mazur, Angélica Osorno, Viktoriya Ozornova, Kate Ponto, Carolyn Yarnall** | Which weak equivalences and fixed-point tests define the model? |
| K-theory constructions | *A multiplicative comparison of Waldhausen and Segal K-theory*, with **Angélica Osorno** | Does the equivalence preserve multiplication and coherence, not merely underlying groups? |
| coTHH tools | *Computational tools for topological coHochschild homology*, with **Teena Gerhardt, Amalie Høgenhaven, Brooke Shipley, Stephanie Ziegenhagen** | What are the input coalgebra, convergence assumptions, and extensions? |
| Rational equivariant K-theory | Naive-commutative and genuine-commutative structure papers, with **Christy Hazel, Jocelyne Ishak, Magdalena Kędziorek, Clover May** | Which norms survive the algebraic model, and why are the two notions of commutativity different? |
| Witt structures | *Equivariant Witt complexes and twisted topological Hochschild homology*, with **Teena Gerhardt, Cameron Krulewski, Sarah Petersen, Lucy Yang** | How do norms and the twisted Hochschild construction organize restriction, Frobenius, and Witt-type data? |

The Witt-complex paper is a newer discovery, beyond the older author-page inventory: [Vanderbilt institutional publication record](https://facultyprofiles.vanderbilt.edu/esploro/outputs/journalArticle/Equivariant-Witt-complexes-and-twisted-topological/991044674863203276?institution=01VAN_INST). Its abstract/metadata were located; its full bibliography is not checked here.

## 7. A reading route connected to this repository

After the existing spectrum definitions, first work through the finite C2-set example and learn why Mackey functors are the right coefficient objects. Then read Bohmann–Osorno's categorical construction. Next compare additive transfers with the finite-set norm above before starting Angeltveit–Bohmann. The coTHH paper offers a different route, through a recognizable space and a checkable graded answer. The rational K-theory and Witt papers belong after those distinctions, not before them.

Possible exercises are: compute the Burnside ring for another small group; enumerate restrictions of orbit types; verify the finite-set norm formula for k=0,1,2,3; and generate the graded basis for LS3 without asserting any additional product structure. These are proposed mathematical exercises, not implemented features.

## Thanks and names

Thank you to Anna Marie Bohmann and every collaborator individually named here. The primary coTHH paper spells **Amalie Høgenhaven**; that spelling is retained rather than an inconsistent older webpage spelling. The [shared bibliography ledger](../researchers/ACKNOWLEDGMENTS.md) also thanks the authors and explicitly named contributors in the four fully inspected bibliographies. Those thanks do not imply endorsement of these independent notes. Unread bibliographies remain explicitly pending.
