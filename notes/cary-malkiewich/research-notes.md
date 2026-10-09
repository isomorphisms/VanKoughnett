# Cary Malkiewich: research notebook

Checked 2026-10-09. Independent study notes, not the author's prose, not lecture transcripts, and not a proof audit. This is a substantial first survey, not a claim to have read every paper. Bibliography coverage is stated separately in [the acknowledgments ledger](../researchers/ACKNOWLEDGMENTS.md).

## Sources and reading depth

- [Author-maintained research and exposition index](https://people.math.binghamton.edu/malkiewich/): publication discovery, coauthors, version warnings, and links to the works listed below.
- [On higher scissors congruence, arXiv:2210.08082v4](https://arxiv.org/html/2210.08082): abstract, introduction, section structure, and selected concluding material inspected; not a verification of its proof.
- [A trace map on higher scissors congruence groups, arXiv:2303.08172v2](https://arxiv.org/html/2303.08172v2): abstract, the universal-measure example, and complete bibliography inspected.
- [A convenient category of parametrized spectra, arXiv:2305.15327](https://arxiv.org/abs/2305.15327): abstract and version metadata inspected.
- [Periodic points and topological restriction homology, arXiv:1811.12871](https://arxiv.org/abs/1811.12871): abstract and version metadata inspected.
- [Spectra and stable homotopy theory, May 2026 draft](https://people.math.binghamton.edu/malkiewich/spectra_book_draft.pdf): located, not read end to end. Treat the draft as a source to study, not as material already summarized here.

## 1. A map of the mathematics

Malkiewich offers several routes out of the introductory spectra material in this repository. One route starts with spaces varying over a base and asks for a workable stable theory of those families. Another starts with cutting polytopes into pieces and asks what a spectrum remembers beyond the familiar scissors-congruence group. A third starts with fixed or periodic points and asks what a trace can obstruct. The author's publication index connects these routes through algebraic K-theory, topological Hochschild homology, equivariance, and coherence.

Our organizing questions are therefore: what is the geometric input; what information survives stabilization; what comparison turns the resulting spectrum into something computable; and which information is lost by replacing the spectrum with its degree-zero group?

## 2. Scissors congruence: relations versus relations between relations

**Paper:** Cary Malkiewich, *On higher scissors congruence*. The inspected revision is dated 11 September 2026; older references use *Scissors congruence K-theory is a Thom spectrum*.

The paper identifies Zakharevich's scissors-congruence spectrum with a Thom-spectrum construction based on homotopy orbits of a Tits complex. It settles the higher problem for one-dimensional geometries and reduces higher-dimensional questions to group homology. This is not a claim that all the higher-dimensional group homology has been computed. [Primary text](https://arxiv.org/html/2210.08082).

### An elementary model to keep beside the theorem

For a dissection of a polygon P into pieces P1 and P2, write

    [P] = [P1] + [P2].

That equation describes an additive invariant. It does not retain the actual cutting process, the chosen congruences, or a comparison between two sequences of cuts. An independent visualization should maintain both layers: a formal additive expression, and the diagram of actual refinements and reassemblies from which it arose.

For example, cut a rectangle vertically, or first cut it horizontally and then refine both halves vertically. The two descriptions admit a common four-piece refinement. Draw the refinement diagram rather than declaring the two algorithms identical. This is only a finite toy diagram: a loop in a hand-drawn graph of cuts is not automatically a nonzero K1 class. The passage to the assembler and its K-theory must be made explicit.

**Implementation questions, not implemented results:** represent a polytope, an allowed geometry group, a covering family, and an isometry as different types; reject overlaps or gaps when a purported covering is checked; retain a certificate of common refinement; distinguish an invariant value from the proof that it respects a covering relation.

The Tits-complex viewpoint suggests a second visualization, based on flags of subspaces and their incidence rather than on moving solid pieces. An incidence complex and a physical dissection are different presentations of the problem. A useful display could show the correspondence where it has been established without pretending they are literally the same picture.

## 3. The shared scissors trace: the direct Bohmann connection

**Authors:** Anna Marie Bohmann, Teena Gerhardt, Cary Malkiewich, Mona Merling, and Inna Zakharevich. *A trace map on higher scissors congruence groups*, IMRN (2024). [Primary text](https://arxiv.org/html/2303.08172v2).

Example 7.10 uses the universal measure to obtain

    K_i(C_hG) -> H_i(G; K_0(C)).

For the specified polytope category, the paper combines this construction with Malkiewich's result to obtain a rational isomorphism. The hypotheses and rationalization matter: this is not an integral classification of every assembler's K-theory, nor does it say that arbitrary traces are equivalences. The complete bibliography of this paper is credited in the shared ledger.

### Independent algebraic exercise

Take a trivial action of the infinite cyclic group on the abelian group Z. Its standard two-term resolution gives H0 = Z, H1 = Z, and higher homology zero. This is a small group-homology calculation, not a computation of a particular scissors-congruence spectrum. To apply the trace theorem one would still have to identify the actual group action and coefficient module.

That separation is useful in code: a group-homology calculation may be correct while the proposed identification of its inputs with a geometric problem is wrong. Keep the input identification as a separate obligation.

## 4. Parametrized spectra: families, not a collection with the labels erased

**Paper:** Cary Malkiewich, *A convenient category of parametrized spectra*. The 2023 article condenses the earlier *Parametrized spectra, a low-tech approach*. Its stated contribution is a point-set setting with convenient classes of objects preserved by common operations, and a direct construction of the bicategory of parametrized spectra. The abstract credits the bridge from Dold's index theory to work of May and Sigurdsson, Ponto, and Shulman. [Primary record](https://arxiv.org/abs/2305.15327).

### Independent introductory model

Start with a retractive space over B:

    B --section--> E --projection--> B,
    projection(section(b)) = b.

Each fiber has a chosen basepoint. For B consisting of two isolated points, this is just a pair of based spaces. A map selecting one of those points pulls the family back to one fiber. A map exchanging the two points exchanges the fibers. These elementary examples explain why a family should retain its base and base-change maps.

For a non-discrete base, a collection of fiber homotopy types does not by itself describe the family. Transport around a loop can matter. The analogue of a twisted line bundle already warns against replacing a family by one chosen fiber without tracking monodromy.

At the spectrum level, keep separate: the base B; the fiberwise suspension coordinate; a change of base; and the replacement needed to derive a construction. A formula involving pullback or smash products must specify whether it is a point-set construction or a derived one. This distinction is precisely why the paper's convenient point-set framework is useful, but the framework has not been reconstructed or formally checked here.

**Cross-reading:** Beaudry, Chloe Lewis, Clover May, Sabrina Pauli, and Elizabeth Tatum's guide to equivariant parametrized cohomology explicitly cites both versions of Malkiewich's work. See [Beaudry's notebook](../agnes-beaudry/research-notes.md).

## 5. Periodic points, traces, and what can actually be removed

**Authors:** Cary Malkiewich and Kate Ponto. *Periodic points and topological restriction homology*. The abstract establishes, in a specified dimension range, the completeness of an equivariant Reidemeister-trace obstruction to removing n-periodic points, and places the obstruction in topological restriction homology. It addresses conjectures of John R. Klein and Bruce Williams. It also provides a fiberwise generalization. [Primary record](https://arxiv.org/abs/1811.12871).

### Independent dynamical exercise

For a rotation of the circle by angle theta, the equation f^n(z) = z is equivalent to n*theta being an integer multiple of 2*pi. If theta/(2*pi) is irrational, no positive iterate has a fixed point. If it is rational with reduced denominator q, every point has period q.

This elementary test concerns a particular map. A homotopy obstruction asks a different question: can the map be deformed so that the unwanted points disappear? Moreover, fixed points of f^n include points whose least period divides n. A visual periodic-point counter should not label all of them as least-period-n points.

The circle example is not presented as an instance of the paper's completeness theorem: its dimension hypotheses have not been checked here. Its role is to distinguish the mathematical questions before applying the machinery.

## 6. Other research strands: inventory, not substitute abstracts

The following clusters were located in the author's index. Entries in this section are discovery records; full arguments and bibliographies remain to be inspected. The grouping is ours, not the author's classification.

### Equivariance and h-cobordisms

With **Mona Merling**: *Equivariant A-theory*; *Coassembly is a homotopy limit map*; and *Equivariant parametrized h-cobordism theorem, the non-manifold part*. With **Thomas Goodwillie, Kiyoshi Igusa, and Mona Merling**: work on functoriality of the space of equivariant smooth h-cobordisms. Reading question: how do categorical fixed-point data and geometric cobordisms meet, and which part of the comparison is genuinely equivariant rather than an ordinary statement applied separately at each subgroup?

### THH, cyclotomic structure, and free loops

Individual papers include *Cyclotomic structure in the topological Hochschild homology of DX* and *Topological cyclic homology of the dual circle*. With **John Lind**: *Morita equivalence between parametrized spectra and module spectra* and *The transfer map of free loop spaces*. A comparison of cyclotomic THH models is joint with **Emanuele Dotto, Irakli Patchkoria, Steffen Sagave, and Calvin Woo**. Reading question: does a comparison preserve the cyclotomic structure, or only the underlying spectrum? A nonequivariant equivalence alone does not answer that question.

### Endomorphisms and trace constructions

With **Jonathan Campbell, John Lind, Kate Ponto, and Inna Zakharevich**: *K-theory of endomorphisms, the TR-trace, and zeta functions* and work on spectral Waldhausen categories, the S-construction, and the Dennis trace. With **John R. Klein**: K-theoretic torsion and zeta functions. Reading question: where is composition of endomorphisms retained, and where does a trace deliberately identify cyclic reorderings?

### Coherence

With **Kate Ponto**: *Coherence for bicategories, lax functors, and shadows*; *Coherence for indexed symmetric monoidal categories*; and periodic-point structures on parametrized spectra. Reading question: which diagrams commute strictly in a chosen presentation, which have specified natural isomorphisms, and which require a higher coherence theorem? A drawing with equal endpoints is not itself a coherence proof.

### Newer scissors-congruence work

With **Alexander Kupers, Ezekiel Lemann, Jeremy Miller, and Robin J. Sroka**: the scissors automorphism-group series, including homological stability/K-theory and Solomon–Tits themes. With **Inbar Klang, Josefien Kuijper, David Mehrle, and Thor Wittich**: higher spherical scissors congruence and Hopf-algebra work, including a comparison between model-category and infinity-category Hopf algebras. These are leads for further paper-level notes, not claims to have read every version. A bibliography's announcement of a forthcoming sequel is not proof that a public full text exists.

### Other foundations

With **Maru Sarazola**: a concise proof concerning the stable model structure on symmetric spectra. Earlier individual work includes *Coassembly and the K-theory of finite groups* and *A tower connecting gauge groups to string topology*. The dissertation and its errata should be read together.

## 7. Corrections are part of the record

The author explicitly marks a mistake in *The transfer is functorial*. Do not repeat the old general claim as established by that paper. The index links an erratum and the later paper **John R. Klein, Cary Malkiewich, and Maxime Ramzi**, *On the multiplicativity of the Euler characteristic*. A corrected statement about Euler characteristics is not automatically a corrected theorem about all transfer maps. [Author's current index and warning](https://people.math.binghamton.edu/malkiewich/).

## 8. Expository reading route

Begin with the author's short notes on homotopy pushouts, fibrations, the bar construction/BG, and the stable homotopy category; then the introductory G-spectra material and parametrized-spectra user's guide; then the THH expositions and trace pictures. The much larger spectra textbook draft can be used as a reference after this orientation. These materials are linked in the [author's exposition index](https://people.math.binghamton.edu/malkiewich/), but their individual chapters are not represented as read in this pass.

**Questions for the next close reading:** spell out one complete low-dimensional assembler; identify its coefficient module in the trace; read the periodic-point dimension range before using its obstruction; and compare one base-change diagram in the two parametrized-spectra treatments.

## Thanks and attribution

Thank you to Cary Malkiewich and every collaborator named above. Thank you also to **Mona Merling, David White, Luke Wolcott, and Carolyn Yarnall**, coauthors with Malkiewich of work on the user's-guide project and the experiential context of mathematics. The individual source-bibliography credits in [the shared ledger](../researchers/ACKNOWLEDGMENTS.md) are additional thanks, not a claim that those scholars reviewed, endorsed, or coauthored these notes. No private contact information is reproduced.
