# 02 — Homotopy cofibers and homotopy fibers

**Source:** [Caleb Ji, *Stable homotopy theory*, §2, pp. 5–9](https://www.math.columbia.edu/~calebji/stable-notes.pdf), recording lectures in Paul VanKoughnett's 2021 seminar.

**Video status:** Course-associated mathematical notes; the matching individual recording and timestamps have **not** been verified. This file is numbered by notebook topic, not claimed YouTube episode number.

## 1. The basic asymmetry in spaces

Start with a map of pointed spaces

\[
f:A\longrightarrow X.
\]

A **homotopy cofiber** models the space obtained by attaching a cone on \(A\) along \(f\). A **homotopy fiber** models the collection of points of \(X\) equipped with a path certifying that their image under \(f\) goes to the base point.

These are dual constructions, but they behave differently in the ordinary homotopy category of spaces:

- Iterated cofibers extend a sequence **forward**, using suspension.
- Iterated fibers extend a sequence **backward**, using loop spaces.
- Only after passing to spectra does the symmetry become especially strong.

This is one of the reasons to learn the constructions before introducing stable model categories.

## 2. Mapping cone and homotopy cofiber

Write \(CA=A\times[0,1]/(A\times\{1\}\cup\{*\}\times[0,1])\) for the **reduced cone**. Its boundary copy of \(A\) sits at \(t=0\).

The mapping cone of \(f\) is

\[
C(f):=X\cup_f CA.
\]

A pointed map \(X\to C(f)\) is canonical. Up to the appropriate weak equivalence, \(C(f)\) is the homotopy cofiber of \(f\).

If \(A\hookrightarrow X\) is a CW-subcomplex inclusion, then

\[
C(f)\simeq X/A.
\]

**Why not define it as \(X/A\) for every map?** Because \(X/A\) is only a literal quotient when \(A\subseteq X\), and even then it can behave poorly under homotopy equivalence if the inclusion lacks appropriate cofibration properties.

### Example: boundary of a disk

For the inclusion \(S^1\hookrightarrow D^2\),

\[
\operatorname{hocofib}(S^1\hookrightarrow D^2)
\simeq D^2/S^1\cong S^2.
\]

The result is not a disk with a slightly different boundary; collapsing the boundary produces a sphere.

## 3. The Puppe sequence

Take the cofiber of a map, then the cofiber of the next map. In the pointed homotopy category this yields the **Puppe sequence**

\[
A\xrightarrow f X
\longrightarrow C(f)
\longrightarrow\Sigma A
\xrightarrow{\Sigma f}\Sigma X
\longrightarrow\Sigma C(f)
\longrightarrow\cdots.
\]

The key structural assertion is that the cofiber of \(X\to C(f)\) is equivalent to \(\Sigma A\).

Apply pointed homotopy classes of maps **into** a test space \(Z\):

\[
\cdots\longrightarrow[\Sigma X,Z]_*
\longrightarrow[\Sigma A,Z]_*
\longrightarrow[C(f),Z]_*
\longrightarrow[X,Z]_*
\longrightarrow[A,Z]_*.
\]

This is an exact sequence of pointed sets near the right end; farther left, where suspension gives group structures, it is exact as a sequence of groups.

**Exactness at \([X,Z]_*\)** has a particularly concrete interpretation:

A map \(g:X\to Z\) lies in the image of \([C(f),Z]_*\) precisely when \(g\circ f:A\to Z\) is null-homotopic. The null-homotopy supplies the required extension over the attached cone.

That observation is almost the whole proof of this part of the sequence.

## 4. The homotopy fiber

For a pointed map \(f:X\to Y\), let \(y_0\in Y\) be the base point. A model for its homotopy fiber is

\[
F(f):=
\bigl\{(x,\gamma)\,:\,
x\in X,\quad
\gamma:[0,1]\to Y,\quad
\gamma(0)=f(x),\;\gamma(1)=y_0
\bigr\}.
\]

The fiber remembers both the point \(x\) **and the chosen path**. If we took the set-theoretic inverse image \(f^{-1}(y_0)\) without replacing \(f\) by a fibration, we could obtain the wrong homotopy type.

This leads to a homotopy fiber sequence

\[
\cdots\longrightarrow
\Omega X\longrightarrow\Omega Y
\longrightarrow F(f)
\longrightarrow X\xrightarrow f Y.
\]

Applying \([B,-]_*\), for a pointed space \(B\), gives exactness. Setting \(B=S^n\) leads to the usual long exact sequence of homotopy groups of a fibration, with the low-degree pointed-set caveats.

### Example: a loop space as a homotopy fiber

Take \(*\to Y\), the inclusion of the base point. Its homotopy fiber is

\[
F(*\to Y)\simeq\Omega Y.
\]

For \(Y=S^1\), the components of \(\Omega S^1\) are indexed by winding number:

\[
\pi_0(\Omega S^1)\cong\pi_1(S^1)\cong\mathbb Z.
\]

The ordinary fiber of \(*\to S^1\) is a point. It misses the entire winding-number phenomenon—an immediate demonstration of why the *homotopy* fiber is needed.

## 5. Group structure from looping and suspension

There is a multiplication on \(\Omega X\) by concatenating loops. Consequently \([B,\Omega X]_*\) has a group structure. Iterated loop spaces have more commutativity:

\[
[B,\Omega^2 X]_*\quad\text{is abelian}.
\]

Dually, pinching the equator of the reduced suspension gives a comultiplication

\[
\Sigma A\longrightarrow\Sigma A\vee\Sigma A.
\]

Thus \([\Sigma A,Z]_*\) is a group, and \([\Sigma^2 A,Z]_*\) is abelian.

The **Eckmann–Hilton argument** explains the commutativity: once two compatible unital multiplication laws coexist, interchange forces them to agree and be commutative.

## 6. Why spectra simplify everything

In a **stable** homotopy theory, a fiber sequence and a cofiber sequence determine each other.

For a map \(f:A\to B\) of spectra, write \(F=\operatorname{fib}(f)\) and \(C=\operatorname{cofib}(f)\). Then

\[
F\simeq\Omega C,\qquad C\simeq\Sigma F,
\]

and we can continue in either direction:

\[
\cdots\to\Omega B\to F\to A\xrightarrow f B\to C\to\Sigma A\to\Sigma B\to\cdots.
\]

The associated cofiber triangle

\[
A\longrightarrow B\longrightarrow C\longrightarrow\Sigma A
\]

is one of the structures behind a **triangulated category**. In modern treatments the stable \(\infty\)-category retains higher coherences that the triangulated homotopy category alone forgets.

Applying \(\pi_k\) gives a long exact sequence of **abelian groups in every degree**:

\[
\cdots\to\pi_k(A)\to\pi_k(B)\to\pi_k(C)
\to\pi_{k-1}(A)\to\pi_{k-1}(B)\to\cdots.
\]

### Concrete stable example: the Moore spectrum

Take the multiplication-by-\(m\) map on the sphere spectrum,

\[
m:\mathbb S\longrightarrow\mathbb S.
\]

Define the mod-\(m\) Moore spectrum \(M(m)\) as its cofiber:

\[
\mathbb S\xrightarrow{m}\mathbb S\longrightarrow M(m)
\longrightarrow\Sigma\mathbb S.
\]

Since \(\pi_0(\mathbb S)=\mathbb Z\) and \(\pi_{-1}(\mathbb S)=0\),

\[
\pi_0(M(m))\cong\mathbb Z/m.
\]

**Do not conclude** that \(M(m)\simeq H(\mathbb Z/m)\). The Moore spectrum can have higher homotopy groups; the Eilenberg–Mac Lane spectrum \(H(\mathbb Z/m)\) has none except in degree zero.

For example, using \(\pi_1(\mathbb S)=\mathbb Z/2\), the long exact sequence shows

\[
\pi_1(M(2))\cong\mathbb Z/2.
\]

The comparison \(M(2)\not\simeq H\mathbb F_2\) is already visible one degree above zero.

## Exercises

1. Write out the definition of \(C(f)\) and check that a null-homotopy of \(g\circ f\) extends \(g\) from \(X\) to \(C(f)\).
2. Compute the homotopy fiber of \(X\to *\) and explain why it is equivalent to \(X\).
3. Construct the pinch map \(\Sigma A\to\Sigma A\vee\Sigma A\) and identify the induced addition on \([\Sigma A,Z]_*\).
4. Derive \(\pi_0(M(m))=\mathbb Z/m\) from the long exact sequence rather than by analogy with homology.
5. Explain why the formula \(F\simeq\Omega C\) is **not** a general statement about arbitrary maps of spaces.

## References and credits

Thanks to **Paul VanKoughnett** and **Caleb Ji** for the seminar and notes. The standard Puppe sequence is named for **Dieter Puppe**; relevant foundational books include **J. Peter May**, *A Concise Course in Algebraic Topology*, and **Tammo tom Dieck**, *Algebraic Topology*. In the course notes, Ji also cites **Philip S. Hirschhorn** and **Marcelo Aguilar, Samuel Gitler, and Carlos Prieto** for homotopical treatments.
