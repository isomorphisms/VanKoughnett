# User's guides: a reading map reached through Sarah Yeakel

[Back to seminar notes](../README.md) · [Yeakel notebook](../sarah-yeakel/README.md) · [Followed references](followed-references.md) · [Coverage](crawl-log.md) · [Credits](ACKNOWLEDGMENTS.md)

Checked 2026-10-09. This catalogue covers **all 13 guides listed in the three volumes of [Enchiridion](https://mathusersguides.com/)**: five from 2015, five from 2016, and three from 2017. Luke Wolcott wrote two different guides. The site's label “current issue” refers to September 2017, not a new 2026 issue.

These are author-written companions to research papers. Their four sections discuss the main ideas, mental imagery, development story, and a colloquial explanation. The notes below are first-pass orientation from guide sections and primary abstracts, not complete proof reviews. Picture suggestions are our own unless explicitly attributed.

## Suggested paths from the seminar

**Homotopy constructions:** the seminar's [fibers and cofibers](../02-fibers-and-cofibers.md) → Dugger's primer in [followed references](followed-references.md) → Yeakel → Beardsley.

**Symmetry:** Merling → Mazur → Yarnall → Yeakel's later isovariant work in the [research notebook](../sarah-yeakel/research-notes.md).

**Chromatic structure and K-theory:** Frankland and Lorman → Larson → Malkiewich → Wolcott's localized-spectra guide. Read the telescope-conjecture update before treating the historical discussion as current.

**Geometry and stochastic processes:** Catanzaro offers a separate route through cellular chains, currents, and low-temperature limits. It need not wait for the entire spectra route.

## Volume 3 — September 2017

### 01. Sarah Yeakel — Goodwillie calculus and multilinearization

[Guide page](https://mathusersguides.com/enchiridion-vol-3-2017-sarah-yeakel/) · [Research paper and version history](https://arxiv.org/abs/1706.06915) · [Expanded notebook](../sarah-yeakel/goodwillie-and-imagery.md)

**Question:** how can a model for linearizing several variables retain the symmetry needed for composition? The guide explains the finite-sets-and-injections indexing category through its motivations and pictures.

**Version warning:** the old title *A monoidal model for Goodwillie derivatives* and its cross-effects claims predate a substantial correction. The corrected paper establishes a lax monoidal result for multilinearization under its stated assumptions; the old full-derivative claim must not be imported unchanged. The expanded notebook includes worked examples and distinguishes ordinary fibers from homotopy fibers.

### 02. Jon Beardsley — Relative Thom spectra via operadic Kan extensions

[Guide page](https://mathusersguides.com/enchiridion-vol-3-2017-jon-beardsley/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2017/09/ug3-beardsley.pdf) · [Paper](https://arxiv.org/abs/1601.04123)

**Author of source paper:** Jonathan Beardsley.

A Thom spectrum can be approached as a homotopy-colimit construction. The paper studies iterated constructions and relative Thom isomorphisms using operadic Kan extensions. This puts geometric bundle intuition alongside structured algebra.

**Picture to work on:** gluing with an action, then gluing in stages. The guide's group-action viewpoint is useful, but a homotopy quotient is not an ordinary orbit set. Coherent multiplication and the hypotheses for iterating the construction are part of the mathematical content, not decorations on the picture.

### 03. Don Larson — The Adams–Novikov E₂-term for Behrens' spectrum Q(2) at the prime 3

[Guide page](https://mathusersguides.com/enchiridion-vol-3-2017-don-larson/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2017/09/ug3-larson.pdf) · [Paper](https://arxiv.org/abs/1407.3423)

The problem is a particular spectral-sequence calculation connected with detecting periodic families. Its specificity matters: Q(2), the prime 3, and the E₂ page are not interchangeable with an arbitrary spectrum, prime, or final answer.

The guide's building-and-floors imagery offers a way to think about filtration. A display could track a class through pages, but must separate an E₂ class from a surviving homotopy class. Differentials and extension problems remain. Source-era detection conjectures are not marked as independently verified current results here.

## Volume 2 — September 2016

### 04. Mike Catanzaro — Dynamics and fluctuations of cellular cycles on CW complexes

[Guide page](https://mathusersguides.com/enchiridion-vol-2-2016-mike-catanzaro/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2016/09/ug2-catanzaro.pdf) · [Author's publication list](https://catanzaromj.github.io/publications/)

**Research collaborators:** Michael J. Catanzaro, Vladimir Y. Chernyak, John R. Klein.

The guide relates stochastic motion of cellular cycles to higher-dimensional currents, Kirchhoff-type constructions, and low-temperature adiabatic limits. A moving cycle can sweep out a chain one dimension higher. A useful display would retain orientations and coefficients: a cellular chain is not merely an unweighted subset of a mesh.

**Source repair:** the guide labels its source link and abstract temporary. Catanzaro's publication list supplies the related article [*On fluctuations of cycles in a finite CW complex*](https://arxiv.org/abs/1710.07995), listed as published in 2022 under the title *Fluctuations of cycles in a finite CW complex*. Its abstract states fractional quantization of average current. We have not established that this later article is word-for-word the manuscript intended by the old provisional title. The listed [2016 dissertation](https://digitalcommons.wayne.edu/oa_dissertations/1433) remains another lead; its full text was not retrieved.

### 05. Martin Frankland — Completed power operations for Morava E-theory

[Guide page](https://mathusersguides.com/enchiridion-vol-2-2016-martin-frankland/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2016/09/ug2-frankland1.pdf) · [Paper](https://arxiv.org/abs/1311.7123)

**Source authors:** Tobias Barthel and Martin Frankland.

Power operations package more structure than ordinary multiplication. Completion becomes essential in the Morava E-theory setting, and the paper develops the appropriate completed algebraic operations.

**Starting question:** what information does a power operation carry beyond taking a power of an element? The height-one relation ψ(x)=xᵖ+pθ(x) is a useful algebraic foothold discussed in the guide. Keep derived/L-completion distinct from naive completion; the hypotheses behind their comparison are not automatic. A formal-series picture is motivation, not a replacement for the completed-category argument.

### 06. Vitaly Lorman — Landweber flat real pairs and ER(n)-cohomology

[Guide page](https://mathusersguides.com/enchiridion-vol-2-2016-vitaly-lorman/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2016/09/ug2-lorman.pdf) · [Paper](https://arxiv.org/abs/1603.06865)

**Source authors:** Nitu Kitchloo, Vitaly Lorman, W. Stephen Wilson.

The paper develops comparison methods for Real Johnson–Wilson cohomology using suitable real pairs and Landweber-flatness assumptions. A Bockstein spectral sequence is central to passing between the relevant theories.

**Picture to work on:** follow named classes and maps across successive approximation stages, with uncertainty about differentials displayed rather than concealed. The result is not a base-change recipe for every space. “Real” here names the equivariant refinement, not cohomology with real-number coefficients.

### 07. Kristen Mazur — An equivariant tensor product on Mackey functors

[Guide page](https://mathusersguides.com/enchiridion-vol-2-2016-kristen-mazur/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2016/09/ug2-mazur.pdf) · [Paper](https://arxiv.org/abs/1508.04062)

The work constructs norm functors and an equivariant monoidal structure in the cyclic p-group setting. Tambara functors emerge as the appropriately equivariant commutative algebra objects.

**Picture to work on:** a subgroup ladder with different arrows for restriction, additive transfer, and multiplicative norm. A norm is not an additive transfer with a new label. Nor does an ordinary commutative monoid under the usual box product automatically contain the extra norm structure of a Tambara functor. The group hypotheses belong in every example.

### 08. F. Luke Wolcott — Variations of the telescope conjecture and Bousfield lattices for localized categories of spectra

[Guide page](https://mathusersguides.com/enchiridion-vol-2-2016-luke-wolcott/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2016/09/ug2-wolcott.pdf) · [Paper](https://arxiv.org/abs/1307.3351)

Bousfield classes compare the spectra killed by smashing with a given object. The paper studies these classes and versions of telescope/smashing questions inside localized categories.

A useful organizing picture is a collection of annihilation tests, not a literal spatial partition of every spectrum. Compactness and strong dualizability need not agree in these settings, so they should remain separate labels.

**Historical update:** the original Ravenel telescope conjecture cannot still be called open at heights at least two: see [Burklund–Hahn–Levy–Schlank](https://arxiv.org/abs/2310.17459). This does not automatically decide each distinct localized-category conjecture studied by Wolcott. Details are in [followed references](followed-references.md).

## Volume 1 — October 2015

### 09. Cary Malkiewich — Coassembly and the K-theory of finite groups

[Guide page](https://mathusersguides.com/enchiridion-vol-1-2015-cary-malkiewich/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2015/07/ug1-malkiewich1.pdf) · [Paper](https://arxiv.org/abs/1503.06504)

The paper relates assembly and coassembly to a norm map, with applications involving algebraic K-theory and chromatic localization. The guide supplies interpretations in terms of modules and group actions.

**Starting question:** which construction gathers local information, and which tests or distributes global information? Do not turn this useful contrast into the false assertion that coassembly is the inverse of assembly. Also keep K(R), algebraic K-theory of a ring or ring spectrum, distinct from Morava K(n).

### 10. Mona Merling — Categorical models for equivariant classifying spaces

[Guide page](https://mathusersguides.com/enchiridion-vol-1-2015-mona-merling/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2015/07/ug1-merling.pdf) · [Paper](https://arxiv.org/abs/1201.5178)

**Source authors:** Bertrand J. Guillou, J. Peter May, Mona Merling.

Category-level constructions yield models for equivariant classifying spaces and bundles. This offers a route from familiar categorical data to geometric objects with symmetry.

**Picture to work on:** a bundle as a pullback of a universal bundle, keeping the base action, fiber action, and their compatibility visible. A naive ordinary classifying-space picture can hide the equivariant conditions. Do not assume that fixed points commute with every realization or quotient without checking the relevant construction.

### 11. David White — Monoidal Bousfield localizations and algebras over operads

[Guide page](https://mathusersguides.com/enchiridion-vol-1-2015-david-white/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2015/10/ug1-white.pdf) · [Paper](https://arxiv.org/abs/1404.5197)

Localization changes which maps count as equivalences. The paper asks when operadic algebra structures survive this change and supplies criteria rather than an unconditional preservation theorem.

**Picture to work on:** retain the underlying object and visibly change the arrows being inverted, then ask which multiplication diagrams remain valid. Equivariant examples demonstrate that preservation can fail. This is a good companion to Yeakel's operadic localization work, but the two constructions should not be identified merely because both use the word localization.

### 12. F. Luke Wolcott — Bousfield lattices of non-Noetherian rings: some quotients and products

[Guide page](https://mathusersguides.com/volume-1-wolcott/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2015/10/ug1-wolcott.pdf) · [Paper](https://arxiv.org/abs/1301.4485)

This guide studies tensor-annihilation information in derived categories of particular non-Noetherian rings, including behavior under quotients and products. It is a distinct paper from Wolcott's 2016 guide.

**Starting question:** when does passage between ring/module categories induce a manageable map on their Bousfield lattices? Equality of Bousfield classes does not assert isomorphism of the original objects. A lattice picture displays one kind of information, not a complete classification of the derived category.

### 13. Carolyn Yarnall — The slices of Sⁿ ∧ Hℤ̲ for cyclic p-groups

[Guide page](https://mathusersguides.com/enchiridion-vol-1-2015-carolyn-yarnall/) · [Guide PDF](https://mathusersguides.com/wp-content/uploads/2015/07/ug1-yarnall1.pdf) · [Paper](https://arxiv.org/abs/1510.02077)

The paper computes slices for the stated family of integer suspensions of the equivariant Eilenberg–Mac Lane spectrum, for cyclic p-groups at odd primes. The notation ℤ̲ denotes the constant Mackey functor.

The guide compares the slice filtration with a Postnikov-style decomposition. A display could show layers together with subgroup and representation information. It must not depict the slice tower as merely an ordinary Postnikov tower or silently extend the calculation to p=2 or to all equivariant spectra.

## Attribution and reuse

Each guide remains attributed to its author, with source-paper coauthors named where applicable. The linked guide pages display Creative Commons Attribution–NonCommercial 4.0 licensing; this notebook does not apply that license to the separate research papers. No source PDF is mirrored here. These are independently written summaries, reading questions, and links. See [individual and bibliography-level acknowledgments](ACKNOWLEDGMENTS.md).
