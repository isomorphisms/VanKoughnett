# Sarah Yeakel: K-theory and trace-methods reading path

[Reading hub](README.md) · [Prelim and analyticity](prelim-and-analyticity.md) · [Research notebook](research-notes.md)

Checked 2026-10-09. This note follows the public trail around Yeakel's K-theory talks and the Goodwillie/THH/TC background they point into. It is a reading map, not a claim that all of these topics are results of Yeakel's own research.

## 1. 2014: Manifolds, K-theory, and related topics

At the 2014 Dubrovnik conference celebrating **Thomas Goodwillie's** 60th birthday, Yeakel's abstract was titled:

> **Classifying n-excisive functors by generic representations**

The abstract says that **Nicholas Kuhn** classified degree-(n) functors of vector spaces using modules over matrix rings, that **Randy McCarthy** generalized this to endofunctors of module spectra, and that Yeakel would discuss a further generalization to (n)-excisive functors from suitable simplicial model categories to spaces or spectra.

The technical bridge already visible in that abstract is **Bökstedt's THH construction**: a slight modification of Goodwillie's (n)th Taylor-polynomial construction is used to retain extra structure.

Conference archive: [ALGTOP announcement](https://lists.illinois.edu/lists/arc/algtop-l/2014-05/msg00003.html).

The conference also included **Inna Zakharevich** immediately afterward with a talk on a spectral sequence for the Grothendieck spectrum of varieties. That adjacency is worth recording because these are two different mathematical trails and should not be merged in hindsight.

## 2. 2015: a compact K-theory course at European Talbot

Yeakel's research page lists an **“Intro to K-theory”** talk at European Talbot in July 2015. The workshop schedule makes the sequence unusually useful as a reading syllabus:

1. **Sarah Yeakel** — _Algebraic K-theory of rings and ring spectra: introduction_;
2. **Gabe Angelini-Knoll** — big theorems in algebraic K-theory;
3. **Cary Malkiewich** — the Dennis trace map;
4. **Valentin Krasontovitsch** — topological cyclic homology and the cyclotomic trace map.

Workshop page: [European Talbot 2015 schedule](https://www.math.ku.dk/english/calendar/events/talbot2015/).

This gives a clean conceptual progression:

[
K longrightarrow HH/THH longrightarrow TC,
]

with trace maps providing a computational comparison between difficult algebraic K-theory and more tractable Hochschild/cyclic constructions.

## 3. 2017: Dundas–McCarthy in three parts

At the **Midwest Topology Summer School on Trace Methods in Algebraic K-Theory** at Indiana University, Yeakel and **Aaron Royer** gave three successive lectures:

- _The Dundas–McCarthy Theorem I_;
- _The Dundas–McCarthy Theorem II_;
- _The Dundas–McCarthy Theorem III_.

The surrounding school makes the intended context explicit. Other lectures covered computations via trace methods, equivariant stable homotopy, THH and Frobenius, cyclotomic spectra and TC, Bökstedt periodicity, Tate diagonals, symmetric powers in K-theory, and the cyclotomic trace.

Archive: [Indiana University summer-school page](https://math.indiana.edu/events/2017-summer-school.html).

### Modern formulation of the theorem

One convenient modern statement is: for a map of connective (E_1)-ring spectra (B	o A) that is surjective on (pi_0) with nilpotent kernel, the cyclotomic trace

[
K(-)longrightarrow TC(-)
]

induces an equivalence on the corresponding **relative fibers**.

See **Sam Raskin**, [“On the Dundas–Goodwillie–McCarthy theorem”](https://arxiv.org/abs/1807.06709).

The Goodwillie-calculus mechanism behind this is important. Very roughly:

- differentiate algebraic (K)-theory;
- its linear/stable approximation is controlled by **THH**;
- differentiate (TC);
- the same first-order object appears;
- then exploit additional structure to promote this infinitesimal agreement to the stated relative comparison under nilpotence hypotheses.

“Same derivative” by itself is not the theorem. The nilpotence, connectivity, and structural arguments are essential.

## 4. Why THH keeps reappearing in Yeakel's functor-calculus work

Yeakel's 2013 prelim says the move from a sequential indexing category to finite sets and injections was inspired by **Bökstedt's definition of THH**. Her 2017 user's guide repeats the same historical source for the idea.

The mathematical pattern is broader than K-theory:

- naive iterated constructions often have the right homotopy type but insufficient strict symmetry;
- adding finite-set/injection indexing exposes permutation data;
- that extra symmetry helps build coherent multiplicative or compositional structures.

This is why THH is not merely an application sitting at the end of the story. Its construction influenced the *model-building technique* used in the Goodwillie work.

## 5. 2019: Functor Calculus Workshop — where the branches meet

The 2019 Ohio State Functor Calculus Workshop provides an unusually good continuation because many talks were explicitly expository.

Important entries include:

- **Thomas Goodwillie**, _Origins of functor calculus_: the subject grew partly from stable pseudoisotopy and algebraic K-theory;
- **Brenda Johnson**, on abelian functor calculus;
- **Michael Ching**, on pro-operads and classification of Taylor towers;
- **Ayelet Lindenstrauss**, _The Goodwillie Taylor tower of algebraic K-theory_;
- **Duncan Clark**, an expository route to higher excision and the Taylor tower;
- **Jens Kjaer**, on unstable (v_1)-periodic homotopy via a **K-theory-based (v_1)-periodic Goodwillie spectral sequence**;
- **Sarah Yeakel**, _Chain rules and operads in abelian functor calculus_.

Workshop page: [Ohio State Functor Calculus Workshop](https://people.math.osu.edu/osborne.422/functor-calculus-workshop/).

Yeakel's 2019 contribution returns to Johnson–McCarthy's abelian calculus. In ongoing work with **Kristine Bauer** and **Brenda Johnson**, the goal was a higher-order chain rule, operadic structure on derivatives of monads of (R)-modules, and a monoidal structure for derivatives of functors of abelian categories.

That is a useful second branch from her thesis: one branch went toward isovariant homotopy theory; another continued the chain-rule/operad questions in abelian functor calculus.

## 6. Midwest 2013 scan: Agnès Beaudry is a stronger K-spectrum clue

The actual handwritten Midwest scan is now readable and the section headed **Agnès Beaudry** is substantially closer to the original fuzzy recollection than the generic Goodwillie material.

Her pages discuss:

- Bousfield localization (L_E X);
- Morava (K)-theory (K(n));
- chromatic convergence;
- localized spheres;
- Morava (E)-theory (E_n);
- height (2), stabilizer groups, and spectral sequences aimed at (K(2))-local homotopy.

This does **not** establish that Beaudry is the person originally remembered: the scan is from Midwest 2013, and Beaudry was not an Illinois PhD student. But if “K-bar spectrum” was actually a distorted memory of (K(n))-local spectra, this is one of the best concrete leads found so far.

See the page-image summary in [Public handwritten scans](public-scan-notes.md#5-midwest-notes--fall-2013).

## 7. A compact reading route

For someone entering from the VanKoughnett stable-homotopy notes:

1. [Yeakel's 2013 prelim](prelim-and-analyticity.md): why the indexing category matters.
2. **Bökstedt / THH**: understand why finite-set symmetry fixes multiplicative problems.
3. **Goodwillie calculus**: (P_nF), layers (D_nF), derivatives and convergence.
4. **Algebraic K-theory**: understand the functor (K) as a hard nonlinear invariant.
5. **Dennis/cyclotomic traces**: compare (K) with (THH) and (TC).
6. **Dundas–Goodwillie–McCarthy**: understand when the relative (K)-theory and (TC) fibers agree.
7. Return to **Arone–Ching / Yeakel**: derivatives, operads, chain rules, and the coherence required to compose approximations.

This route explains why K-theory, spectra, THH, operads, and Goodwillie calculus repeatedly occur together without collapsing them into one subject.

## 8. On the original “K-bar spectrum” recollection

This search has now produced several phrases that could plausibly blur together in memory:

- algebraic (K)-theory of ring spectra;
- stable (K)-theory;
- (K)-theory-based (v_1)-periodic Goodwillie spectral sequences;
- THH and TC as spectra associated to ring spectra;
- Goodwillie derivatives, themselves spectra;
- chromatic (K(n))-local language in neighboring work.

None establishes an object actually called a **“K-bar spectrum.”** The identification should remain open rather than forcing one of these into the recollection.

## Thanks

Thank you to **Sarah Yeakel, Aaron Royer, Thomas Goodwillie, Randy McCarthy, Brenda Johnson, Marcel Bökstedt, Bjørn Ian Dundas, Gabe Angelini-Knoll, Cary Malkiewich, Valentin Krasontovitsch, Teena Gerhardt, Michael Mandell, Thomas Nikolaus, Lars Hesselholt, Gijs Heuts, Saul Glasman, Nick Rozenblyum, Michael Ching, Ayelet Lindenstrauss, Duncan Clark, Jens Kjaer, Kristine Bauer, Nicholas Kuhn**, and the other lecturers and authors whose work forms this trail.

The broader repository-wide attribution ledger remains in [acknowledgments](../users-guides/ACKNOWLEDGMENTS.md).
