# Sarah Yeakel: public handwritten scan notes

[Reading hub](README.md) · [K-theory and trace methods](k-theory-and-trace-methods.md) · [Goodwillie guide](goodwillie-and-imagery.md)

Checked 2026-10-09. These are notes from the **actual scanned pages** linked from [Sarah Yeakel's research page](https://sites.google.com/view/syeakel/research). The PDFs were pulled from their public Drive files and the page images were inspected directly. This corrects the earlier inventory that incorrectly stopped at “image-only / unread.”

These are Yeakel's handwritten conference notes. They are necessarily compressed records of live talks; the summaries below should not be treated as substitutes for the speakers' papers or as claims that every formula in a scan was copied perfectly.

## 1. Michael Ching minicourse at UIUC — March 2015

Source: the public 12-page scan ching.PDF.

### Talk 1: classification of Taylor towers

The first page starts from Goodwillie calculus for functors between pointed spaces and spectra:

$$
F\to\cdots\to P_nF\to P_{n-1}F\to\cdots\to P_1F
$$

with layers

$$
D_nF=\operatorname{hofib}(P_nF\to P_{n-1}F)
$$

classified by spectra $\partial_nF$ with $\Sigma_n$-action. The notes record the familiar expression for a homogeneous layer in terms of

$$
(\partial_nF\wedge X^{\wedge n})_{h\Sigma_n}.
$$

The organizing question is stronger than “what are the derivatives?”:

> **What structure on the symmetric sequence $\partial_*F$ is needed to recover the Taylor tower?**

The notes move immediately to the chain rule and monoidal composition of symmetric sequences. They record that $\partial_*\mathrm{Id}$ is an operad and that derivatives of other functors carry module/bimodule structures.

### Koszul duality and the identity functor

The derivative of the identity is presented through partition complexes and then related, by bar/cobar or Koszul-duality ideas, to a spectral analogue of the Lie operad. The notes explicitly connect:

- the commutative operad/cooperad;
- bar-cobar duality;
- the derivatives of the identity;
- right modules and bimodules over $\partial_*\mathrm{Id}$.

This is the conceptual route behind Arone–Ching's classification machinery: the derivatives are not an unordered list of coefficient spectra.

### Talk 2: Waldhausen A-theory and homotopic descent

The second lecture turns to Waldhausen's $A$-theory functor. The notes discuss calculated derivatives of $A$, a natural comparison to a more linear functor, and the Arone–Ching adjunction from functors to bimodules. The tower is recovered through mapping objects in the module category, with coalgebra/divided-power structure appearing when one asks for a genuine classification rather than only the associated layers.

### Talk 3: cross-effects

The third lecture is explicitly headed **cross effects**. The notes record Goodwillie's comparison of derivatives with multilinearized cross-effects and then ask how the cross-effect symmetric sequence itself carries the structure needed for the tower. Divided-power module structures and Koszul duality appear again.

This is particularly relevant to Yeakel's later correction history: cross-effects are exactly where her old thesis/user-guide claims needed repair. The 2015 notes are useful historical context, not evidence that the old version was correct.

### Talk 4: framed manifolds and $KE_n$-module structure

The final pages ask when derivatives carry $KE_n$-module structures and use little-disks/framed-manifold geometry as a source. The notes discuss configuration spaces of framed embeddings, pointed framed manifolds, and how framed embedding data induces module structure on derivatives.

### Why this minicourse matters here

The minicourse puts the following chain on one blackboard:

$$
\text{Taylor tower}
\to
\text{derivatives}
\to
\text{symmetric sequence}
\to
\text{operad/module structure}
\to
\text{Koszul duality}
\to
\text{reconstruction}.
$$

That is a better map of Yeakel's thesis environment than treating “Goodwillie calculus” as a single topic.

---

## 2. Functor Calculus Workshop — Ohio State, 2019

Source: the public 17-page scan functorcalcnotes.pdf.

The scan is especially valuable because it records several neighboring calculi side by side.

### Brenda Johnson — abelian functor calculus

The notes begin with cross-effects for functors between abelian categories and the Johnson–McCarthy notion of degree. They record Taylor towers and the universal property of polynomial approximation in the abelian setting.

This is the branch Yeakel returned to in her own workshop talk on **chain rules and operads in abelian functor calculus**.

### Michael Weiss — manifold calculus

Weiss's pages define polynomial functors on open subsets of a manifold and model them by values on unions of small disks. Embedding spaces are the running geometric example. The notes emphasize connectivity estimates and the way increasingly large finite unions of disks approximate the full embedding functor.

A later Weiss section develops the same geometry through configuration categories.

### Thomas Goodwillie — origins of functor calculus

Goodwillie's pages start with pseudoisotopy/embedding questions and multiple-disjunction connectivity. They show the historical path from geometric connectivity estimates to the abstract notion of a Taylor tower.

A second block returns to manifold calculus and pseudoisotopy. The notes explicitly connect stable pseudoisotopy with $A$-theory and ask for calculational descriptions of the resulting layers.

### Ayelet Lindenstrauss — Taylor tower of relative K-theory

These pages are one of the strongest direct K-theory links in the scan. The notes begin with relative algebraic K-theory and stabilization, then move to the Goodwillie tower, derivatives, and multi-reduced functors. The goal is to understand layers of relative $K$-theory through multilinear constructions.

The handwritten notes are compressed enough that theorem statements should be checked against Lindenstrauss/McCarthy sources before reuse, but the conceptual placement is clear: **algebraic K-theory is an important nonlinear functor to which the calculus is being applied.**

### Michael Ching — pro-operads

Ching's workshop talk returns to classification of Taylor towers. The notes present derivatives of a functor as symmetric sequences and discuss a pro-operad/pro-module formalism designed to retain the extension data needed to reconstruct the tower.

### John Klein — Poincaré calculus

The final pages develop a manifold-calculus-like theory for Poincaré spaces and embeddings, using intersection/disjunction problems and homotopy-theoretic replacements for smooth differential-topological data.

### Cross-connection

The scan makes a useful six-way comparison:

- abelian calculus;
- manifold calculus;
- Goodwillie calculus;
- relative $K$-theory;
- operadic tower classification;
- Poincaré calculus.

The common pattern is **approximation by polynomial/excisive behavior plus extra structure needed to recover nonlinear information**.

---

## 3. Infinity-Operads and Applications — Osnabrück, July 2017

Source: the public 36-page scan inftyoperadnotes.pdf.

The public workshop program identifies the minicourse lecturers as **Javier J. Gutiérrez, Gijs Heuts, and Ieke Moerdijk**, with talks by **Pedro Boavida, Philip Hackney, Rune Haugseng, Brice Le Grignou, and Marcy Robertson**.

### Dendroidal sets

The first lectures build the dendroidal category $\Omega$ from finite rooted trees. The notes treat:

- colored operads;
- representable dendroidal sets $\Omega[T]$;
- faces, degeneracies, boundaries, and horns;
- inner Kan conditions;
- the operadic model structure.

The analogy is systematic:

$$
\Delta \quad\leadsto\quad \Omega,
$$

with linear trees recovering simplicial ideas and arbitrary rooted trees encoding operations with many inputs.

### Goodwillie calculus and the derivatives of the identity

The Gijs Heuts portion begins from Goodwillie towers and homogeneous layers and then focuses on

$$
\partial_*\mathrm{Id}.
$$

The scan records the partition-complex description and the fact that the derivatives form an operad. It explicitly notes the relationship with the Lie operad and Koszul duality.

A handwritten remark says, in substance, that **Yeakel gave a more direct construction of an operad structure on the derivatives**. Because this is a conference-note remark, the corrected status of Yeakel's later paper still governs what can safely be asserted as a theorem.

### Pedro Boavida — little disks and mapping spaces

Boavida's pages discuss $E_n$, spaces of embeddings, configuration categories, and mapping spaces between little-disks operads. The notes connect these mapping spaces to embedding-calculus questions.

### Rune Haugseng — infinity-operads as polynomial monads

The scan develops ordinary operads as monoids in symmetric sequences, then moves to polynomial functors/monads as an infinity-categorical model for operads. This is joint work with **David Gepner and Joachim Kock**.

### Brice Le Grignou — linear operads up to homotopy

These pages develop bar/cobar constructions, curved/cooperadic structures, and homotopy operads in chain complexes.

### Philip Hackney — cyclic operads

The notes replace rooted trees by unrooted trees in order to encode cyclic operads, where the input/output distinction is relaxed. Profinite completion also appears in the workshop's cyclic-operad branch.

### Marcy Robertson — genus-zero curves and Grothendieck–Teichmüller

The later pages discuss genus-zero surface/moduli operads and the Grothendieck–Teichmüller group, together with profinite completion of operadic objects.

### Ieke Moerdijk — model structures and dendroidal homotopy theory

Several lectures return to Reedy/covariant model structures, dendroidal spaces, complete Segal-type objects, and comparison functors among models of infinity-operads.

### Why this belongs beside VanKoughnett

This workshop makes the tree combinatorics behind operads concrete enough to visualize. A useful future interface could show:

- an operation as a rooted tree;
- grafting as operadic composition;
- inner-edge contraction as a face;
- horns as incomplete coherent compositions;
- dendroidal Segal conditions as reconstruction from vertex operations.

That is a much better graphical entry point to operadic Goodwillie structure than starting from a wall of symmetric-sequence formulas.

---

## 4. Manifolds, K-Theory, and Related Topics — Dubrovnik, June 2014

Sources: the two public scans croconf1.PDF (21 pages) and croconf2.PDF (17 pages).

The first page preserves the conference schedule; the handwritten pages then cover a large fraction of the talks.

### K-theory / THH / chromatic cluster

**Kathryn Hess — Waldhausen K-theory via comodules.**  
The notes discuss Waldhausen categories, $A(X)$, categories of comodules, and comparisons designed to preserve K-theory.

**Bjørn Ian Dundas — Higher THH.**  
The notes develop higher-order topological Hochschild homology and explicitly label its **chromatic importance**, with calculations around iterated THH and truncated-polynomial examples.

**Charles Rezk — power operations / Morava E-theory.**  
The notes discuss unstable algebras, power operations, cotangent constructions, and Morava $E$-theory.

**Christian Schlichtkrull — graded Thom spectra and logarithmic THH.**  
The scan records graded/log structures and THH of Thom-spectrum-type objects.

**Ulrike Tillmann — commutative K-theory and generalized cohomology.**  
The notes discuss filtrations of classifying spaces and a commutative refinement of K-theoretic constructions.

**Randy McCarthy — a case for the unbased setting.**  
These pages are particularly close to Yeakel's own work: cross-effects/derivatives in an unbased setting, base-change lemmas, associative versus commutative input categories, and de Rham–Witt-type structures arising from composition of Taylor towers.

### Goodwillie / embedding / operad cluster

**Michael Ching** discusses derivatives, Koszul duality, framed manifolds, and module structure over Koszul duals of little-disks operads.

**Nicholas Kuhn** discusses the Whitehead conjecture and the Goodwillie tower of the circle, including the relationship to periodic/chromatic homotopy.

**David Ayala**, jointly with **John Francis**, discusses Poincaré/Koszul duality and factorization homology. For $n=1$, THH appears as the circle case of factorization homology.

**Ralph Cohen** gives historical context from pseudoisotopy through Waldhausen $A$-theory and the development of functor calculus.

**Michael Weiss**, jointly with **Pedro Boavida de Brito**, treats smooth embedding spaces through operads and configuration categories.

**Emanuele Dotto** discusses equivariant/excisive ideas and genuine versus naive equivariant phenomena.

### Homological stability / categorical cluster

The scans also include talks by **Nathalie Wahl**, **Jérôme Scherer**, **Wojciech Chachólski**, **John Klein**, **Boris Chorny**, and others on homological stability, cellularity/excision, idempotent symmetries, intersection theory, and classification of linear functors.

### A useful historical observation

This 2014 conference already puts **Yeakel's developing classification problem** in a room with:

- Goodwillie calculus;
- algebraic K-theory;
- THH;
- Morava $E$-theory;
- chromatic homotopy;
- operads and Koszul duality;
- manifold/embedding calculus.

So the repeated mixing of “K,” spectra, derivatives, THH, and chromatic terminology in later memory is not surprising. They were literally neighboring talks.

---

## 5. Midwest notes — Fall 2013

Source: the public 17-page scan mwf13.pdf.

This scan is particularly relevant to the original attempt to remember a woman working around K-theoretic/chromatic spectra.

### Kristen Mazur — extra structure on Mackey functors

The first pages develop Mackey functors, transfers/restrictions, Tambara-like norm structure, and symmetric monoidal constructions.

### Agnès Beaudry — chromatic localization and Morava theories

Pages 5–9 are headed **Agnès Beaudry**.

The notes begin with Bousfield localization $L_E X$, compare rational and mod-$p$ examples, and then move to Morava $K$-theory:

$$
K(n).
$$

They discuss:

- chromatic convergence;
- the localized sphere;
- Morava $E$-theory $E_n$;
- the height-2 case;
- stabilizer-group actions;
- spectral-sequence calculations toward $K(2)$-local homotopy.

This is a **much closer literal match to a fuzzy memory involving “K-something spectrum”** than the generic Goodwillie material is. It does not establish that Beaudry was the person originally remembered, but it should stay in the candidate trail.

### Craig Westerland

The next section is headed **Craig Westerland** and concerns distributional/arithmetic problems and homology of moduli-type spaces; the scan itself has relatively little written detail on this talk.

### Marcy Robertson — schematic homotopy types of operads

The notes mention schematization/rationalization and operadic homotopy types.

### John Klein — disjunction and intersection

Klein's pages develop disjunction problems for submanifolds, multi-relative versions, Blakers–Massey-style connectivity, and obstruction/intersection invariants.

### David Gepner — stable homotopy functors

The last pages ask for a stable homotopy theory of geometric objects over a base and discuss motivic/Morel–Voevodsky-style constructions, stable homotopy functors, monoidal structures, and transfer formalisms.

---

## 6. MSRI Summer Workshop — 2013 archive

The public Drive item is not one PDF but a tar archive containing six scanned PDFs:

- shipley.pdf
- hill.pdf
- carlsson.pdf
- blumberg.pdf
- behrens.pdf
- students.pdf

The first five named lecture files were opened and their initial sections inspected. The much larger students.pdf remains only partially inspected.

### Brooke Shipley — introduction to stable homotopy and spectra

The notes start from homotopy groups and Whitehead's theorem, then build suspension and stable ranges through Freudenthal and homotopy excision. This is a clean elementary bridge into spectra.

### Mike Hill — introduction to equivariant stable homotopy

The notes develop $G$-spaces, orbit and fixed-point constructions, adjunctions involving induction/restriction, $G$-CW complexes, and equivariant obstruction theory.

### Gunnar Carlsson — the shape of data / applied topology

Carlsson's notes connect persistent homology with the geometry of data sets. Vietoris–Rips constructions, persistence diagrams, barcode-style invariants, and examples involving image patches appear.

### Andrew Blumberg — introduction to algebraic K-theory

The first lecture begins with the slogan “study a ring via its category of modules,” passes through projective modules and $K_0$, and then uses chain complexes/CW-complex analogies to explain why higher K-theory is a homotopical enhancement rather than just another Grothendieck group.

### Mark Behrens — computational techniques in stable homotopy

The notes begin from computing stable homotopy groups of spheres and move into cohomology operations, Steenrod algebra ideas, and the Adams spectral sequence.

### Why this archive matters

Taken together, these files supply a compact “pre-Goodwillie” foundation:

$$
\text{stable homotopy}
\to
\text{equivariant stable homotopy}
\to
\text{algebraic K-theory}
\to
\text{Adams/chromatic computation},
$$

with Carlsson's persistent-homology lectures as a separate applied-topology branch.

---

## 7. Reading limits and source discipline

- The 2015 Ching scan, 2019 functor-calculus scan, 2017 infinity-operad scan, both 2014 Dubrovnik scans, and the 2013 Midwest scan were visually inspected page by page at notebook scale.
- The MSRI archive was successfully unpacked; the opening portions of the five named lecture files were visually inspected. students.pdf is much larger and has not been read end to end.
- Handwriting sometimes makes a symbol or short attribution ambiguous. Where a precise theorem statement matters, follow the linked speaker/paper rather than treating this notebook as a transcription.
- No scan is mirrored into the repository. These are independent summaries and source links.

## Thanks

Thank you to **Sarah Yeakel** for making these conference notebooks public, and to the lecturers whose mathematics they record, including **Michael Ching, Brenda Johnson, Michael Weiss, Thomas Goodwillie, Ayelet Lindenstrauss, John Klein, Javier J. Gutiérrez, Gijs Heuts, Ieke Moerdijk, Pedro Boavida, Philip Hackney, Rune Haugseng, Brice Le Grignou, Marcy Robertson, Kathryn Hess, Bjørn Ian Dundas, Nathalie Wahl, Charles Rezk, Wojciech Chachólski, Nicholas Kuhn, David Ayala, John Francis, Ralph Cohen, Christian Schlichtkrull, Ulrike Tillmann, Randy McCarthy, Emanuele Dotto, Kristen Mazur, Agnès Beaudry, Craig Westerland, David Gepner, Brooke Shipley, Mike Hill, Gunnar Carlsson, Andrew Blumberg, and Mark Behrens**.

Additional collaborators named in individual talks are credited in the relevant sections above. A full citation-by-citation audit of every handwritten bibliography/reference remark remains separate work.
