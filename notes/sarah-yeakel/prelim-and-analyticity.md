# Sarah Yeakel: prelim and analyticity notes (2013–2014)

[Reading hub](README.md) · [Research notebook](research-notes.md) · [K-theory and trace-methods branch](k-theory-and-trace-methods.md)

Checked 2026-10-09. These notes summarize two author-hosted PDFs whose text was recoverable directly from the public Google Drive files linked by [Sarah Yeakel's research page](https://sites.google.com/view/syeakel/research). They are formative notes, not later peer-reviewed theorem statements.

## Sources and reading status

1. **Sarah Yeakel, _Why we can take hocolim over I with Tn's_**, Spring 2013.  
   [Public PDF](https://drive.google.com/open?id=1W8oGXsacV-Bxz4Mw8fzUMz9J2XQ8AEkH)

   The extracted text was read throughout. The PDF is about 24 pages and includes its own bibliography.

2. **Sarah Yeakel, analyticity notes**, circa 2014.  
   [Public PDF](https://drive.google.com/open?id=1tASjLVcOxGNMLldAKChSmwcYl3P7vSan)

   The extracted text was read throughout. It is a short handout built around stable excision, analyticity, and examples.

The later thesis and 2017 user's guide contain cross-effect errors explicitly acknowledged by the author. Nothing below upgrades a 2013 or 2014 exploratory claim merely because it appears in these notes.

## 1. The problem: composition versus an ordinary sequential homotopy colimit

Goodwillie's (n)-excisive approximation is built from an infinite iteration of intermediate functors (T_n):

[
F longrightarrow T_nF longrightarrow T_n^2F longrightarrow cdots ,
qquad
P_nF simeq operatorname*{hocolim}_{kinmathbb N} T_n^kF.
]

Yeakel starts from work of **Brenda Johnson** and **Randy McCarthy** on algebraic functor calculus. In the algebraic setting, degree-(n) functors can be organized through a category whose morphisms are polynomial approximations to mapping objects. The topological analogue runs into a strict-composition problem: composing two sequential homotopy colimits naturally produces an indexing problem over (mathbb N	imesmathbb N). There is no canonical choice of a single stage that gives the desired strictly associative composition.

This is the early form of a problem that reappears in the later derivative work: the homotopy type is not the only issue; the **model must retain enough symmetry and coherence for composition**.

## 2. Replace (mathbb N) by (mathbb I)

The proposed repair, credited in the notes to McCarthy and inspired by **Marcel Bökstedt's construction of topological Hochschild homology**, is to use

[
mathbb I = {	ext{finite sets and injections}}.
]

The ordinary sequential category (mathbb N) sits inside (mathbb I) through the standard inclusions. But (mathbb I) also contains permutations. Informally, the extra maps remember that there are many ways to insert new coordinates, rather than forcing every construction through one preferred left-to-right staircase.

The prelim decomposes the construction into three pieces:

- an action of symmetric groups on iterates of an endofunctor;
- order-preserving injections produced from a natural transformation (eta:1	o F);
- compatibility between these two structures, so a general injection can be factored into a permutation followed by an ordered inclusion.

For the symmetric-group action, a natural transformation

[
sigma:Fcirc F	o Fcirc F
]

must behave like a swap. Besides (sigma^2=1), the adjacent swaps must satisfy the braid relation. This is exactly the point at which “we can swap two coordinates” is weaker than “we have a coherent symmetric action on all iterates.”

### A small combinatorial example

There are six injections from a two-element set into a three-element set. A sequential model chooses one standard inclusion; (mathbb I) retains all six, related by permutations. This is the elementary content behind the slogan **add the missing symmetry to the indexing category**.

## 3. Homotopy limits and colimits are part of the proof, not notation

The prelim reviews the **Bousfield–Kan** constructions:

- homotopy colimits from geometric realization of a simplicial replacement;
- homotopy limits from totalization of a cosimplicial replacement.

It also discusses fat realization and why a homotopy-invariant construction cannot simply be replaced by an ordinary colimit.

A later comparison asks when the (mathbb N)-indexed and (mathbb I)-indexed constructions agree up to weak equivalence. The argument uses increasing connectivity, a Bökstedt-style lemma, and a form of **Quillen's theorem B**. The notes quote a proposition from the appendix of the Dundas–Goodwillie–McCarthy book to control the map from an object of a diagram into a homotopy fiber of its homotopy colimit over the classifying space of the indexing category.

This is a useful warning for any implementation or visualization: the arrows of the indexing category and their coherences are mathematical data. Replacing the diagram by a pile of stage objects loses the reason the comparison works.

## 4. Stable excision

For a homotopy functor (F:C	o D), the notes write (E_n(c,kappa)) for a quantitative stable (n)-excision condition. Roughly, if the initial edges of a strongly cocartesian ((n+1))-cube have connectivities (k_sge kappa), then the image cube under (F) is

[
left(-c+sum_s k_sight)	ext{-cartesian}.
]

Smaller (c) and smaller (kappa) are stronger conditions.

The point of keeping the quantitative version is that each application of the (T_n) construction improves connectivity. Under suitable hypotheses, the maps between later iterates become arbitrarily highly connected. That is what allows the (mathbb I)-indexed model to agree with the usual (P_nF) in the cases under discussion.

## 5. Analyticity as a convergence slope

The separate analyticity handout defines (F) to be (ho)-analytic when one fixed constant (q) works so that

[
E_n(nho-q,ho+1)
]

holds for every (nge1).

The longer prelim explains the geometric meaning: analyticity controls a **vanishing-line slope** in the spectral sequence associated to the Goodwillie tower. If

[
D_qF(X)=operatorname{hofib}(P_qF(X)	o P_{q-1}F(X)),
]

then the tower produces a spectral sequence whose first page is built from the homotopy groups of the layers (D_qF(X)). A positive-slope vanishing line gives strong convergence under the appropriate hypotheses.

The useful analogy with ordinary calculus is therefore not merely “Taylor polynomials approximate functions.” A closer match is:

- degree/excision controls the polynomial stage;
- connectivity estimates control the error;
- analyticity controls where the tower converges.

The author explicitly warns that the analogy with an ordinary radius of convergence is imperfect: being outside a guaranteed convergence range does not itself prove divergence.

## 6. Examples in the analyticity handout

The handout records:

- the identity functor on spaces is **1-analytic**, using higher Blakers–Massey;
- being (k)-excisive by itself does not supply all the lower-(n) stable-excision estimates needed to infer a single analyticity line;
- examples built from (Q(-)) and mapping-space functors illustrate slopes (0) and (dim K), respectively.

These examples are especially visualizable as a plot in the ((n,c))-plane: available excision estimates are points or regions, while an analyticity statement asks for one linear bound working simultaneously for all (n).

## 7. Why this belongs in the K-theory branch

The prelim opens by naming **algebraic K-theory** and **chromatic homotopy theory** as applications of Goodwillie calculus. More concretely, its main indexing trick is traced to Bökstedt's THH construction, and the bibliography includes **Dundas, Goodwillie, and McCarthy, _The Local Structure of Algebraic K-Theory_**.

So Yeakel's early path is not “a K-theory project that later wandered into Goodwillie calculus.” It is better described as a Goodwillie-calculus project whose technical machinery was already intertwined with the machinery of THH and trace methods.

That distinction matters for the original “K-bar spectrum” recollection: this material gives several real K-theory/spectra associations, but does **not** identify that remembered phrase.

## 8. Bibliography and thanks from the prelim

The prelim's own bibliography names:

- **J. F. Adams**, _Stable Homotopy and Generalized Homology_;
- **Marcel Bökstedt**, _Topological Hochschild Homology_;
- **A. K. Bousfield** and **D. M. Kan**, _Homotopy Limits, Completions, and Localizations_;
- **Bjørn Ian Dundas**, **Thomas G. Goodwillie**, and **Randy McCarthy**, _The Local Structure of Algebraic K-Theory_;
- **Paul Goerss** and **John Jardine**, _Simplicial Homotopy Theory_;
- **Thomas G. Goodwillie**, _Calculus I_, _Calculus II_, and _Calculus III_;
- **G. W. Whitehead**, _Generalized Homology Theories_.

The prelim also explicitly credits **Eric Peterson** for the spectral-sequence explanation used in the analyticity discussion.

Thank you to all of them, and especially to Sarah Yeakel for leaving these formative notes public. The fact that later corrections exist makes the notes more useful historically, not less: they show which coherence problems were visible early and which ones survived into later work.
