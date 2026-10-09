# Goodwillie calculus: guide, examples, and picture cautions

[Yeakel research notebook](research-notes.md) · [All 13 user's guides](../users-guides/README.md)

These are independent study notes, checked 2026-10-09. Yeakel's 2017 guide is useful for motivation but **predates the correction to its cross-effects claims**. Use the narrower, corrected result recorded in the research notebook, not the old guide's abstract as a theorem statement.

## Read the four parts separately

**Sarah Yeakel**, Enchiridion volume 3 (2017): [landing page](https://mathusersguides.com/enchiridion-vol-3-2017-sarah-yeakel/), [key ideas](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t1.pdf), [mental imagery](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t2.pdf), [development story](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t3.pdf), [colloquial explanation](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t4.pdf).

The four-part organization separates mathematical structure, intuition, discovery, and explanation. Those are different kinds of evidence: a motivating image need not certify a theorem.

## 1. What is being differentiated?

A homotopy functor transforms spaces or spectra while respecting weak equivalence. Its Taylor approximations fit into a tower

$$F\longrightarrow\cdots\longrightarrow P_2F\longrightarrow P_1F\longrightarrow P_0F.$$

An n-excisive functor takes strongly homotopy cocartesian (n+1)-cubes to homotopy cartesian cubes. At n=1, homotopy pushout squares become homotopy pullback squares. For the identity on pointed spaces,

$$P_1\mathrm{Id}(X)\simeq\Omega^\infty\Sigma^\infty X.$$

Thus stabilization is the first approximation, not a claim that a space is already stable. The layers are homotopy fibers, not literal set differences. Under the usual finitary hypotheses their classification uses spectra with symmetric-group actions. Layers alone omit extension data, and convergence of the whole tower requires an additional theorem.

Source: **Gregory Arone and Michael Ching**, [*Goodwillie Calculus*, introduction and sections 1–2](https://arxiv.org/html/1902.00803). This later survey is a supplementary reference, not a link that existed in the 2017 guide.

## 2. An elementary model of an interaction term

For a quadratic function, the mixed finite difference is

$$q(x+y)-q(x)-q(y)+q(0)=2xy,\qquad q(t)=t^2.$$

At x=2 and y=3, it is 25−4−9=12. The expression vanishes for an additive linear function. This calculation motivates asking what information appears only when two inputs occur together.

In homotopy calculus, the corresponding cross-effect uses a **total homotopy fiber**, rather than subtraction of numerical values, of the square

```text
F(X ∨ Y)  ───→  F(X)
   │               │
   ↓               ↓
 F(Y)     ───→   F(*)
```

The arrows collapse wedge summands. The finite-difference calculation above is an independently worked analogy, not a proof that this square has any particular operadic composition law. For the latter, the cross-effects correction is decisive.

Source for the cross-effect viewpoint: Yeakel's [key-ideas section](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t1.pdf); see the [version warning](research-notes.md#3-a-lax-monoidal-model-for-multilinearization).

## 3. Why replace a single sequence of inclusions by injections?

A diagram indexed by 0→1→2→⋯ remembers a particular route through increasing sizes. The category of finite sets and injections also remembers relabellings and different inclusions.

For example, six injections send a two-element set into a three-element set: three choices for the first image and two for the second. Keeping only the usual inclusion discards five choices. Disjoint union then provides a way to combine indexing sets without arbitrarily selecting a staircase through a grid.

This is an intuition for retaining symmetry, not a proof that changing an indexing category preserves every homotopy colimit. The comparison in Yeakel's corrected construction has connectivity hypotheses. See her [imagery section](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t2.pdf) and the research notebook.

## 4. Homotopy colimits retain the manner of gluing

Yeakel's imagery section explicitly recommends **Daniel Dugger's [*A primer on homotopy colimits*](https://pages.uoregon.edu/ddugger/hocolim.pdf)**.

For a span X←A→Y, a homotopy pushout inserts A×[0,1] between X and Y before identifying its ends. For a more general indexing category, composable arrows require higher-dimensional coherence data, not just isolated connecting tubes.

Dugger's section 2 offers a concrete warning: objectwise weakly equivalent diagrams can have ordinary colimits of different homotopy types. His introductory example and cylinder construction are a useful bridge from [the seminar's fiber/cofiber notes](../02-fibers-and-cofibers.md).

## 5. An ordinary fiber can give the wrong picture

The guide's [colloquial section](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t4.pdf) uses collapsing one circle of a wedge as an accessible fiber example. Do not silently replace “fiber” there by “homotopy fiber.”

**Independent check:** let p:S¹∨S¹→S¹ preserve the circle a and collapse b. The ordinary fiber above the wedge point is the b-circle. The homotopy fiber has the homotopy type of the infinite cyclic covering graph: an infinite line with a b-loop at each integer. Its fundamental group is the free group generated by

$$\{a^kba^{-k}:k\in\mathbb Z\}.$$

This follows by pulling back the contractible universal cover of S¹ and reading the resulting graph. The homotopy fiber is therefore equivalent to a countable wedge of circles, not one circle. This is a useful concrete test for any proposed fiber animation.

## 6. Keep the development story and the correction history distinct

The [development essay](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t3.pdf) describes an earlier connectivity problem involving spheres. For k≥1, S^k is (k−1)-connected, not k-connected. That episode is separate from the later cross-effects error flagged by the author and the [2018 arXiv revision](https://arxiv.org/abs/1706.06915).

A useful picture notebook could therefore start with injection choices, gluing cylinders, and the covering-graph fiber example. Those illustrate actual constructions without suggesting that rotating a diagram proves a coherence identity.

Thank you to Sarah Yeakel, Daniel Dugger, Gregory Arone, and Michael Ching for the explanations and mathematics behind this reading path. Broader credits and reading limits are in the [attribution ledger](../users-guides/ACKNOWLEDGMENTS.md) and [coverage log](../users-guides/crawl-log.md).
