# Sarah Yeakel: worked examples and connections

Checked 2026-10-09. This supplements, rather than replaces, [the paper-by-paper research notebook](research-notes.md) and [the existing Goodwillie/imagery notes](goodwillie-and-imagery.md). The examples below are independently written preparations for reading the papers. None is advertised as a formalization or a proof of their main theorems.

The [author's research page](https://sites.google.com/view/syeakel/research) identifies the research papers, dissertation, and expository material. Its warning about errors in the older cross-effects argument remains essential. Do not turn the historical seminar title 'A chain rule for Goodwillie calculus' into evidence that every version of the proposed theorem is valid.

## 1. Equivariant and isovariant are visibly different

**Sources:** Sarah Yeakel, [An isovariant Elmendorf's theorem](https://arxiv.org/abs/1907.12135); Inbar Klang and Sarah Yeakel, [Isovariant homotopy theory and fixed point invariants](https://arxiv.org/abs/2110.07853). The existing notebook records their abstract-level scope; the examples here are elementary deductions from the definitions.

Let C2 act on the interval [-1,1] by reflection. The stabilizer of 0 is all of C2; the stabilizer of every other point is the identity subgroup.

The constant map c(x)=0 is equivariant: reflecting before or after applying c gives the same answer. It is not isovariant. For x not equal to zero, its stabilizer changes from the identity subgroup to C2.

The map f(x)=x^3 is equivariant because (-x)^3=-x^3. It is also isovariant: the only input sent to zero is zero. The map x↦x^2 is not equivariant for this action on both source and target, because (-x)^2=x^2 while reflection of x^2 is -x^2.

A stabilizer check therefore carries more information than a test that two drawings look symmetric.

### An equivariant contraction that is not an isovariant homotopy

Consider H_t(x)=(1-t)x for 0≤t≤1. Every H_t is equivariant. For t<1 it preserves the two stabilizer types, but H_1 collapses the interval to its fixed point and fails isovariance away from zero.

This illustrates why an ordinary equivariant contraction cannot simply be imported into the isovariant setting. A formal terminal object in a model-category construction is additional categorical structure; it does not make every geometric collapse preserve stabilizers.

### Two different meanings of a fixed point

For the isovariant self-map f(x)=x^3, the self-map equation f(x)=x has solutions -1,0,1. Only 0 is fixed by the whole acting group. The points -1 and 1 form a free orbit but are individually fixed by f.

A display should have separate indicators for:

- the group stabilizer G_x;
- the equation f(x)=x, or f^n(x)=x when studying iterates.

The Klang–Yeakel fixed-point theorem concerns eliminating self-map fixed points through permitted homotopies under stated manifold dimension and codimension assumptions. The interval example above is not asserted to satisfy those hypotheses.

## 2. Subgroup chains and the stability problem

**Source:** Inbar Klang and Sarah Yeakel, [An isovariant Blakers–Massey theorem](https://arxiv.org/abs/2506.21259). Abstract and introductory statements were inspected in the original notebook. The paper develops an isovariant Blakers–Massey theorem, higher-cubical versions, and a suitable suspension by a trivial representation sphere, leading to an isovariant Freudenthal theorem.

For C4, the strict chains

    {e} < C4
    {e} < C2 < C4

have the same first and last subgroup but are not the same chain. A data model that records only endpoints loses the intermediate stratum. This is an elementary reason to retain the chain-indexed data appearing in the isovariant theory rather than summarizing all connectivity by one integer.

A proposed picture can display orbit-type strata and links between them, with a separate chain selector. It must distinguish an actual chain from a repeated entry and record which connectivity assertion applies to it. This is a design proposal, not an assertion that a drawn stratification has already supplied the complete linking-orbit data used in the papers.

**Important boundary:** suspension by a trivial representation in this construction is not a finished theory of inversion of every representation sphere. Do not identify it with a complete genuine RO(G)-graded stable category without further work.

## 3. A small cross-effect calculation

**Sources:** the original Yeakel calculus papers and the joint [Unbased calculus for functors to chain complexes](https://arxiv.org/abs/1409.1553). The calculation below is in elementary linear algebra, not a claim about an arbitrary homotopy functor.

Over a field, take F(V)=V tensor V. Expanding a direct sum gives

    F(V plus W)
      = (V tensor V)
        plus (V tensor W)
        plus (W tensor V)
        plus (W tensor W).

The summands involving both variables are

    cr_2 F(V,W) = (V tensor W) plus (W tensor V).

They measure the part not already accounted for by F(V) and F(W). Each mixed summand is linear in each variable separately, even though F is quadratic in one variable.

For one-dimensional V and W, F(V plus W) has dimension 4, while the two unmixed pieces account for only 2 dimensions. The other 2 dimensions are the mixed terms. A picture with four labelled tiles makes this decomposition testable.

This example does not justify transporting a formula between algebraic, discrete, and Goodwillie calculi without checking definitions. In particular, a cotriple-based degree condition and n-excision are not interchangeable merely because both are called polynomial behavior.

## 4. Why the injection category is more than an integer counter

**Source:** Sarah Yeakel, [A Monoidal Model for Multilinearization, revised arXiv version](https://arxiv.org/html/1706.06915v2), published as *A lax monoidal model for multilinearization*. The corrected construction and complete bibliography were inspected.

Write I for the category of finite sets and injections. Between a one-element set and a two-element set are two injections; between a two-element set and a three-element set are six. A finite n-element set also has n! automorphisms. Replacing I by the ordered list 0,1,2,... discards this information.

The injection-indexed stabilization has the schematic form

    D_1 F(X) = hocolim_(U in I) Omega^U F(Sigma^U X).

U labels the suspension and loop coordinates. A permutation of U changes their order, so coherent symmetric information belongs to the construction. Agreement with an ordinary linearization requires the hypotheses in the paper; the formula is not an unrestricted theorem for arbitrary F.

The revised lax-monoidal result concerns multilinearization of the specified multipointed symmetric functor sequences, evaluated at the zero-sphere. 'Lax monoidal' supplies coherent comparison maps, not automatic isomorphisms. The missing cross-effects step must not be silently restored to claim that the whole derivative functor has been proved monoidal in that paper.

### Minimal finite test data

For a future combinatorial exercise, enumerate all injections among sets of sizes at most three and verify composition. For instance, a particular injection {1,2}→{1,2,3} followed by a permutation of the target may give a different injection. Such a test checks the indexing category. It does not check the homotopy colimit or the lax-monoidal theorem.

## 5. Chain complexes: identities up to weak equivalence are not enough

**Authors:** Maria Basterra, Kristine Bauer, Agnès Beaudry, Rosona Eldred, Brenda Johnson, Mona Merling, and Sarah Yeakel. [Unbased calculus for functors to chain complexes](https://arxiv.org/abs/1409.1553).

The abstract singles out a concrete obstruction to reusing the spectrum-target argument: the relevant functor must be part of a cotriple, and the required identities must hold at the stronger level used in that construction, not merely after passing to weak equivalence. The paper uses explicit iterated-fiber models and also constructs deloopings for specified first-stage values.

For orientation, a comonad T has counit epsilon:T→Id and comultiplication delta:T→T*T. Its two counit identities and coassociativity are equations between natural transformations. Knowing that the source and target of two composites happen to be quasi-isomorphic does not prove those equations.

A formal sketch should therefore distinguish: an actual chain map; a chain homotopy; a quasi-isomorphism; and an equality of natural transformations. Collapsing all four into one notion of 'equivalent' would remove precisely the issue the authors had to solve.

This is a direct Beaudry–Yeakel collaboration. It should be cross-linked, not treated as two unrelated papers with similar titles.

## 6. Operads, stabilization, and group completion

**Authors for both papers:** Maria Basterra, Irina Bobkova, Kate Ponto, Ulrike Tillmann, and Sarah Yeakel.

- [Infinite loop spaces from operads with homological stability](https://arxiv.org/abs/1612.07791).
- [Inverting operations in operads](https://arxiv.org/abs/1611.00715).

The first uses homological-stability conditions to obtain infinite-loop-space structure after group completion of appropriate algebras. The second constructs a homotopical localization for a chosen submonoid of unary operations, adapting hammock localization. These are abstract-level reading notes; their full bibliographies are not yet checked in this pass.

### Three operations that should not be confused

A gluing operation may take two inputs to one output. A stabilization can be a selected one-input operation. Group completion can make an additive monoid group-like. These are related mechanisms but are not the same construction.

At the most elementary level, completing the monoid of nonnegative integers under addition produces Z. That statement concerns components of a toy example. It does not manufacture all deloopings or prove an infinite-loop recognition theorem.

Likewise, a tree node with two inputs should not acquire a strict inverse node merely because a theorem inverts selected unary operations. A unary operation may be inserted along an edge, while a multi-input vertex changes the input profile. The arity belongs in the type.

A geometric study could use labelled cobordism-gluing diagrams, with stabilization marked separately. It would then have to add the actual stability assumptions, group-completion map, and coherent operadic structure before claiming to illustrate the theorem rather than its motivating geometry.

## 7. Connections to the other notebooks

| Connection | What is established | What is only a proposed comparison |
| --- | --- | --- |
| Beaudry | Shared authorship of the unbased-calculus paper | Relating an explicit cotriple model to the later equivariant-family computational workflows |
| Bohmann | Both collections involve equivariant structure and operads | A translation between categorical Mackey constructions and isovariant diagrams; no equivalence is claimed |
| Malkiewich | Trace/fixed-point and parametrized themes intersect; Kate Ponto and Inbar Klang occur in nearby collaborations | A common visual language for periodic-point and isovariant obstructions, with hypotheses kept distinct |
| VanKoughnett material | Suspension, fibers, cofibers, and spectra supply prerequisites | These research notes are not claims about a particular recorded lecture |

## Thanks and remaining bibliography work

Thank you to Sarah Yeakel; Maria Basterra; Kristine Bauer; Agnès Beaudry; Rosona Eldred; Brenda Johnson; Mona Merling; Irina Bobkova; Kate Ponto; Ulrike Tillmann; and Inbar Klang. Thank you to **Randy McCarthy** for the doctoral supervision identified in the institutional dissertation record.

The complete sixteen-entry bibliography of the corrected multilinearization paper is mapped to individual names in [the shared acknowledgments ledger](../researchers/ACKNOWLEDGMENTS.md). It preserves entries marked 'in preparation' as historical references, not as verified published papers. The pre-existing [user-guide acknowledgments](../users-guides/ACKNOWLEDGMENTS.md) cover additional material from the earlier traversal. The other Yeakel paper bibliographies must still be checked individually; no blanket assertion of completed coverage is made.
