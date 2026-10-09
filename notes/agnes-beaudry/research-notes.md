# Agnès Beaudry: research notebook

Checked 2026-10-09. Independent notes and exercises, not a proof audit or a claim to have read the whole publication list. The spelling **Agnès Beaudry** follows the public author page; some arXiv metadata omits the accent.

## Reading status and primary sources

- [Author-maintained research page](https://sites.google.com/colorado.edu/agnesbeaudry/): broad publication and collaborator inventory inspected. Its published/unpublished grouping is not automatically current; individual records can be newer.
- Agnès Beaudry and Jonathan A. Campbell, [A guide for computing stable homotopy groups](https://arxiv.org/pdf/1801.07530): introduction, contents, and bibliography inspected; selected computational discussion located. The numerous Adams-chart figures have not been audited.
- Agnès Beaudry, Chloe Lewis, Clover May, Sabrina Pauli, and Elizabeth Tatum, [A Guide to Equivariant Parametrized Cohomology](https://arxiv.org/html/2410.13971): abstract, organizational outline, selected final examples, and bibliography inspected.
- Agnès Beaudry, [The Algebraic Duality Resolution at p=2](https://arxiv.org/abs/1412.2822): abstract and version metadata inspected.
- Agnès Beaudry, Irina Bobkova, Paul G. Goerss, Hans-Werner Henn, Viet-Cuong Pham, and Vesna Stojanoska, [The Exotic K(2)-Local Picard Group at the Prime 2](https://arxiv.org/abs/2212.07858): February 2026 revision metadata and abstract inspected.
- Daniel D. Spiegel, Marvin Qi, David T. Stephen, Michael Hermele, Markus J. Pflaum, and Agnès Beaudry, [A Classifying Space for Phases of Matrix Product States](https://arxiv.org/abs/2501.14241): January 2026 revision and abstract inspected. This author order follows that revision, which explicitly changes the order to match condensed-matter conventions.
- Maria Basterra, Kristine Bauer, Agnès Beaudry, Rosona Eldred, Brenda Johnson, Mona Merling, and Sarah Yeakel, [Unbased calculus for functors to chain complexes](https://arxiv.org/abs/1409.1553): abstract inspected; see the Yeakel collection for the existing discussion.

The two guide bibliographies are completely covered at the level of names in [ACKNOWLEDGMENTS](../researchers/ACKNOWLEDGMENTS.md). The other bibliographies remain pending.

## 1. Three useful entrances

Our reading map has three entrances: explicit stable-homotopy calculations; equivariant families and local coefficients; and families of quantum states. The first is closest to the title of this repository, but the other two clarify why spectra and classifying spaces are useful rather than merely technical constructions.

Beaudry's computational guide with Campbell is organized around spectra, the Steenrod algebra, the Adams spectral sequence, and examples motivated by classification of invertible phases. The quantum motivation does not mean that every intermediate spectrum is itself a physical space of states. [Guide](https://arxiv.org/pdf/1801.07530).

## 2. A working Adams-chart model

The following is an independent explanatory exercise, not a transcription of one of the guide's charts.

In a suitable bounded-below, finite-type setting, the mod-2 Adams spectral sequence has the schematic form

    E2^(s,t) = Ext_A^(s,t)(H^*(X; F2), F2)
             => pi_(t-s)(X completed at 2).

A is the mod-2 Steenrod algebra. Filtration is s; internal degree is t; the stable stem is t-s. The completion and convergence hypotheses must be recorded in an actual application.

A differential has bidegree (r,r-1):

    d_r : E_r^(s,t) -> E_r^(s+r,t+r-1).

Thus on a chart whose horizontal coordinate is t-s and vertical coordinate is s, the arrow moves one step left and r steps up. These two coordinate systems should never be silently interchanged.

### A small algebra calculation that produces a tower

Take the graded algebra A0 = F2[epsilon]/(epsilon^2), with epsilon in degree 1, and its augmentation module F2. The repeated multiplication-by-epsilon resolution has one free generator in each successive shifted degree. Applying Hom_A0(-,F2) makes the differentials zero because epsilon acts trivially on F2.

Hence one gets a class in every bidegree (s,t)=(s,s), and the Ext algebra is the polynomial algebra on a class h0 in bidegree (1,1). On the stem/filtration chart this is a vertical tower at stem zero.

This calculation is about A0-modules. It does not by itself compute the sphere spectrum's homotopy groups. A chart can be algebraically correct but attached to the wrong spectrum. Even after the appropriate E2 page is identified, differentials, additive extensions, multiplicative extensions, and convergence are separate obligations.

### What a useful chart interface must retain

A dot should know its source module, bidegree, filtration, page, and whether it is only a candidate permanent cycle. An extension should be represented separately from a differential. The display should distinguish a proven zero from an uncomputed entry. A sparsity argument should identify the range and the possible source/target groups it rules out.

A pair of F2 pieces in an associated graded group does not, on its own, decide between Z/4 and Z/2 plus Z/2. This elementary ambiguity explains why an E-infinity page is not always the final answer.

## 3. Height two at the prime two

**Paper:** Beaudry, *The Algebraic Duality Resolution at p=2*. It constructs a finite resolution of the trivial completed group-ring module using modules induced from finite subgroups of the norm-one Morava stabilizer group. The abstract credits the earlier construction to **Paul Goerss, Hans-Werner Henn, Mark Mahowald, and Charles Rezk**, and describes the precision needed for explicit calculations. [Primary record](https://arxiv.org/abs/1412.2822).

### Independent orientation to the objects

A standard height-two Morava E-theory coefficient ring at p=2 is written

    E_2,* = W(F4)[[u1]][u, u^(-1)],

with a chosen convention such as degree(u)=-2. The coefficient ring, its continuous stabilizer action, a resolution used to compute group cohomology, and the spectrum being reconstructed are four different layers.

The subscript 2 in K(2) denotes chromatic height; the separate prime is also 2 in this collection. A visualization should make those two choices explicit. Neither the page number in a spectral sequence nor the number of variables in a picture is the chromatic height.

The useful finite-group input in a duality resolution does not make the entire stabilizer group finite. One must retain the completed group ring and continuous action. A finite complex of induced modules is a computational replacement, not an assertion that all profinite information has disappeared.

### Related sequence of work located

The author index connects the algebraic resolution to the dissertation, K(2)-local Moore-spectrum calculations, chromatic splitting, and later topological duality resolutions. The 2026-updated paper with **Irina Bobkova and Hans-Werner Henn**, *The duality resolution at n=p=2*, now has a dedicated [focused notebook](duality-resolution-n-p-2.md). It upgrades the older resolution from the norm-one stabilizer subgroup to the Galois-extended norm-one group and explicitly does **not** resolve the entire K(2)-local sphere.

## 4. Exotic invertible spectra: an algebraic invariant can miss an object

**Authors:** Agnès Beaudry, Irina Bobkova, Paul G. Goerss, Hans-Werner Henn, Viet-Cuong Pham, and Vesna Stojanoska. The inspected 2026 revision of *The Exotic K(2)-Local Picard Group at the Prime 2* states

    kappa_2 = (Z/8)^2 × (Z/2)^3,

a group of order 512, and uses several construction methods including a J-homomorphism from real representations of finite quotients of the stabilizer group. This is the **exotic subgroup**, not a claim that the entire K(2)-local Picard group has 512 elements. [Primary record](https://arxiv.org/abs/2212.07858).

### Independent arithmetic and conceptual checks

The stated order follows from 8*8*2*2*2=512. A convenient abstract coordinate system has five coordinates, with addition modulo 8,8,2,2,2 respectively. An element can have order 8; the group is not merely a nine-dimensional F2-vector space.

For study, separate an invertible spectrum, its image under an algebraic invariant, and the possible kernel of that invariant. Equality of images is not equality of the original spectra. The word 'exotic' names that detection issue in its specific setting; it should not be used as a visual style or a generic synonym for complicated.

The proof constructing and detecting these elements has not been audited here. A finite abelian-group calculator would illustrate the answer, not implement the classification proof.

## 5. Parametrized cohomology: local behavior and transport belong in the degree

**Authors:** Agnès Beaudry, Chloe Lewis, Clover May, Sabrina Pauli, and Elizabeth Tatum. Their guide explains the Costenoble–Waner theory, extending RO(G)-grading to representations of the equivariant fundamental groupoid, RO(Pi B). It treats ordinary local coefficients when G is trivial, develops finite-group examples, and warns by example that RO(Pi B) need not be free. [Primary text](https://arxiv.org/html/2410.13971).

### Independent example: a sign local system on a circle

Give the circle one vertex and one oriented edge. Put Z in the coefficient fiber, with transport T around the circle. The cellular cochain complex has the form

    Z --(T-1)--> Z.

With trivial transport T=1, its cohomology is Z in degrees zero and one. With sign transport T=-1, the differential is multiplication by -2, so H0=0 and H1=Z/2.

Every fiber is still abstractly Z. The different result comes from transport, not from changing the fiber's cardinality or rank. This is a small model of why a family must retain its gluing information.

The guide's equivariant theory has additional stabilizers, representations, restrictions, and transfers. It is not just this ordinary local-system example with a group label attached. Read its definitions of the equivariant fundamental groupoid and stable orbit category before attempting that extension.

**Direct connection to Malkiewich:** the guide cites both *Parametrized spectra, a low-tech approach* and *A convenient category of parametrized spectra*. **Direct connection to Bohmann:** Mackey-functor-style coefficient data and representation grading reappear, though the guide is not an application of every theorem in Bohmann's papers.

## 6. Quantum-state families: a concrete bridge back to Eilenberg–MacLane spaces

**Authors, in the January 2026 revision order:** Daniel D. Spiegel, Marvin Qi, David T. Stephen, Michael Hermele, Markus J. Pflaum, and Agnès Beaudry. *A Classifying Space for Phases of Matrix Product States*, Communications in Mathematical Physics 407, 17 (2026).

For their space of translation-invariant injective matrix product states, allowing all physical and bond dimensions, the abstract gives weak homotopy type

    K(Z,2) × K(Z,3).

It constructs the space as a gauge quotient and proves the projection from a contractible tensor space is a quasifibration. The claimed classification concerns families in this specified setting, not all quantum many-body phases. [Primary record](https://arxiv.org/abs/2501.14241).

### Independent consequences for simple parameter spaces

Using the displayed classifying-space type, a family parametrized by a CW space X has the corresponding pair of cohomological labels in H2(X;Z) and H3(X;Z). For X=S2, only the H2 label can be nonzero; for X=S3, only the H3 label can be nonzero. For X=S2 × S1, the elementary Künneth calculation supplies one Z in each of degrees two and three.

These are labels for **families**. A picture of one tensor network at one parameter value does not exhibit either invariant. A better proposed display would show a parameter space, local tensor representatives, the gauge changes between them, and a separate invariant panel. A network diagram without its equivalence relation cannot stand in for the classifying space.

## 7. Broad work inventory and collaborators

The following inventory follows the author page for discovery. Shortened titles identify reading targets; they are not detailed result summaries. Publication metadata should be refreshed from the individual record when the paper is studied. Coauthors are thanked individually rather than hidden behind 'et al.'.

### Chromatic calculations and duality

- Dissertation on the duality-resolution spectral sequence for the Moore spectrum at the prime 2; *The Algebraic Duality Resolution at p=2*; *Towards the homotopy of the K(2)-local Moore spectrum at p=2*; *The chromatic splitting conjecture at n=p=2*; and work on the alpha family. These are individual-author entries.
- Chromatic splitting of the K(2)-local sphere: with **Paul G. Goerss and Hans-Werner Henn**.
- Duality resolution at n=p=2: with **Irina Bobkova and Hans-Werner Henn**.
- Cohomology of the Morava stabilizer group through that resolution: with **Irina Bobkova, Paul G. Goerss, Hans-Werner Henn, Viet-Cuong Pham, and Vesna Stojanoska**.
- Dualizing spheres and compact p-adic analytic groups: with **Paul G. Goerss, Michael J. Hopkins, and Vesna Stojanoska**.
- Determinant sphere and Tate twist: with **Tobias Barthel, Paul G. Goerss, and Vesna Stojanoska**.
- Gross–Hopkins duals of higher real K-theory: with **Tobias Barthel and Vesna Stojanoska**.
- Invertible K(2)-local E2-modules in C4-spectra: with **Irina Bobkova, Michael A. Hill, and Vesna Stojanoska**.
- Orbits for the Lubin–Tate ring: with **Naiche Downey, Connor McCranie, Luke Meszar, Andy Riddle, and Peter Rock**.

### Bordism, tmf, and explicit spectral sequences

- Models of Lubin–Tate spectra from Real bordism, and transchromatic extensions in motivic bordism: with **Michael A. Hill, XiaoLin Danny Shi, and Mingcong Zeng**.
- Quotient rings of HF2 smash HF2, and slice spectral sequences for quotients of norms of Real bordism: with **Michael A. Hill, Tyler Lawson, XiaoLin Danny Shi, and Mingcong Zeng**.
- tmf calculations for RP2 and RP2 smash CP2: with **Irina Bobkova, Viet-Cuong Pham, and Zhouli Xu**.
- E2-term of the bo-Adams spectral sequence, and a paper titled *The telescope conjecture at height 2 and the tmf resolution*: with **Mark Behrens, Prasit Bhattacharya, Dominic Culver, and Zhouli Xu**. The latter title is not a license to assert that the general telescope conjecture was proved there; no current general status claim is made in these notes.

### Exposition, calculus, and Galois theory

- *Chromatic structures in stable homotopy theory*: with **Tobias Barthel**.
- Computational guide: with **Jonathan A. Campbell**.
- Motivic homotopical Galois extensions: with **Kathryn Hess, Magdalena Kędziorek, Mona Merling, and Vesna Stojanoska**.
- Unbased calculus: with **Maria Basterra, Kristine Bauer, Rosona Eldred, Brenda Johnson, Mona Merling, and Sarah Yeakel**. The key abstract-level issue is obtaining the actual cotriple identities in chain complexes, not merely weak equivalences. [Primary record](https://arxiv.org/abs/1409.1553).

### Parametrized quantum systems and nearby work

- Homotopical foundations for parametrized quantum spin systems: with **Michael Hermele, Juan Moreno, Markus J. Pflaum, Marvin Qi, and Daniel D. Spiegel**.
- Continuous dependence in Kadison transitivity and the GNS construction: with **Daniel Spiegel, Juan Moreno, Marvin Qi, Michael Hermele, and Markus J. Pflaum**.
- Higher Berry curvature and a bulk-boundary correspondence: with **Xueda Wen, Marvin Qi, Juan Moreno, Markus J. Pflaum, Daniel Spiegel, Ashvin Vishwanath, and Michael Hermele**.
- Charting ground-state spaces with tensor networks: with **Marvin Qi, David T. Stephen, Xueda Wen, Daniel Spiegel, Markus J. Pflaum, and Michael Hermele**.
- Generalized symmetries of singularity-free nonlinear sigma models: with **Salvatore D. Pace, Chenchang Zhu, and Xiao-Gang Wen**.
- The excitation-detector principle and planon-only abelian fracton orders: with **Evan Wickenden, Wilbur Shirley, and Michael Hermele**, located as [arXiv:2506.21773](https://arxiv.org/abs/2506.21773). Full text not read in this pass.

In these informal collaborator lists, order is not claimed to reproduce each paper's byline. Formal citations should use the actual paper and version. In particular the matrix-product-state paper's revised author order is recorded explicitly above.

## 8. Reading priorities and remaining work

Start with Beaudry–Campbell's guide and reproduce one complete small Ext calculation with the convergence assumptions stated. Next work through the ordinary local-coefficient example and a C2 example in the parametrized guide. The duality-resolution papers then offer a concrete computational spine for the chromatic branch; the matrix-product-state paper offers a different route from familiar tensor diagrams to classifying spaces.

Remaining work includes proof-level notes on those resolutions, bibliography traversal for each inventory item, figure-by-figure checking of the Adams charts, and verification of exact hypotheses before any visualization is described as computing an invariant. These are recorded gaps, not work claimed to be running elsewhere.

## Thanks

Thank you to Agnès Beaudry and every collaborator named above, and to the authors and named contributors in the two guide bibliographies listed in [the acknowledgments ledger](../researchers/ACKNOWLEDGMENTS.md). Thanks also to Paul Goerss, Hans-Werner Henn, Mark Mahowald, and Charles Rezk for the construction explicitly credited in the algebraic-duality-resolution abstract. Acknowledgment does not imply that anyone reviewed or endorsed these notes.
