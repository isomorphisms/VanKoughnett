# 03 — What a spectrum actually is

**Primary sources:** [Caleb Ji's course notes, §3, pp. 10–12](https://www.math.columbia.edu/~calebji/stable-notes.pdf) (lecture of 2021-03-01 attributed to Paul VanKoughnett); [VanKoughnett, course outline, items 3, 6, and 7](https://www.math.purdue.edu/~pvankoug/spectra/outline.pdf).

**Video status:** Based on documented seminar content; no independently verified URL or timestamps for the corresponding recording. Original mathematical exposition, not a transcript.

## 1. Sequential spectra: a concrete first definition

A **sequential spectrum** \(E\) consists of pointed spaces

\[
E_0,\ E_1,\ E_2,\ \ldots
\]

and pointed *structure maps*

\[
\sigma_n:S^1\wedge E_n\longrightarrow E_{n+1}\qquad (n\geq0).
\]

The same data can be written using the suspension–loop adjunction:

\[
\widetilde\sigma_n:E_n\longrightarrow\Omega E_{n+1}.
\]

A map \(f:E\to F\) of these concrete objects is a sequence \(f_n:E_n\to F_n\) making the squares

\[
\begin{array}{ccc}
\Sigma E_n & \xrightarrow{\sigma_n^E} & E_{n+1}\\
\downarrow{\Sigma f_n} && \downarrow{f_{n+1}}\\
\Sigma F_n & \xrightarrow{\sigma_n^F} & F_{n+1}
\end{array}
\]

commute.

**Point to retain:** A prespectrum is a *sequence with structure maps*. It is not a sequence of arbitrary unrelated spaces, a spectral sequence, or a spectrum of eigenvalues.

A **strict/levelwise equivalence** is an equivalence at every \(E_n\to F_n\). A **stable equivalence** will instead be detected by stable homotopy groups. These notions differ.

## 2. Omega-spectra

An **\(\Omega\)-spectrum** is a sequential spectrum whose adjoint structure maps are weak equivalences:

\[
E_n\xrightarrow{\ \simeq\ }\Omega E_{n+1}.
\]

This condition says that consecutive levels are compatible deloopings:

\[
E_n\simeq\Omega E_{n+1}\simeq\Omega^2E_{n+2}\simeq\cdots.
\]

The terminology is justified by the original motivation from generalized cohomology. If

\[
\widetilde E^n(X)\cong[X,E_n]_*
\]

and \(\widetilde E^n(X)\cong\widetilde E^{n+1}(\Sigma X)\), then

\[
[X,E_n]_*
\cong[\Sigma X,E_{n+1}]_*
\cong[X,\Omega E_{n+1}]_*.
\]

The representing spaces therefore satisfy the \(\Omega\)-spectrum condition up to weak equivalence.

### A distinction worth testing

**Every \(\Omega\)-spectrum is a spectrum, but not every sequential spectrum is an \(\Omega\)-spectrum.**

The ordinary sphere spectrum below is the simplest test case. It is a perfectly good sequential spectrum even though its levelwise adjoint structure maps do not all satisfy the \(\Omega\)-condition.

## 3. Examples with different purposes

### Suspension spectrum of a pointed space

For a pointed space \(X\), define

\[
(\Sigma^\infty X)_n=\Sigma^n X=S^n\wedge X.
\]

Its structure maps are the evident identifications

\[
\Sigma(\Sigma^nX)\cong\Sigma^{n+1}X.
\]

This is the basic way to move from spaces to spectra. At the homotopy-category level, \(\Sigma^\infty\) is left adjoint to the zeroth infinite-loop-space functor \(\Omega^\infty\).

### Sphere spectrum

Take \(X=S^0\), the two-pointed set with one designated base point:

\[
\mathbb S:=\Sigma^\infty S^0,\qquad
\mathbb S_n=S^n.
\]

The sphere spectrum plays the role of a **monoidal unit** for smash product of spectra, analogously to the integers for tensor products of abelian groups. Its homotopy groups are the stable stems:

\[
\pi_k(\mathbb S)=\pi_k^s.
\]

The spectrum whose \(n\)-th level is \(S^n\) is not already an \(\Omega\)-spectrum: the maps \(S^n\to\Omega S^{n+1}\) are generally not weak equivalences. It can be replaced by a stably equivalent \(\Omega\)-spectrum.

### Eilenberg–Mac Lane spectrum

For an abelian group \(A\), the Eilenberg–Mac Lane space \(K(A,n)\) has one prescribed nonzero homotopy group:

\[
\pi_n(K(A,n))\cong A,\qquad
\pi_i(K(A,n))=0\quad(i\neq n)
\]

for \(n\geq1\). The \(n=0\) case is a discrete space with components indexed by \(A\).

A model of the Eilenberg–Mac Lane spectrum \(HA\) has levels \(K(A,n)\) and weak equivalences

\[
K(A,n)\simeq\Omega K(A,n+1).
\]

Consequently,

\[
\pi_q(HA)=
\begin{cases}
A,&q=0,\\
0,&q\neq0.
\end{cases}
\]

This represents ordinary cohomology with coefficients in \(A\). Its apparent simplicity contrasts sharply with the sphere spectrum: \(\mathbb S\) has nonzero positive-degree homotopy groups, whereas \(HA\) does not.

### Periodic complex K-theory

The complex K-theory spectrum \(KU\) is an \(\Omega\)-spectrum with levels exhibiting Bott periodicity. Models can be arranged so that

\[
KU_{2n}\simeq\mathbb Z\times BU,\qquad
KU_{2n+1}\simeq U,
\]

where \(U\) is the stable unitary group and \(BU\) its classifying space.

In homotopy grading, with \(u\) the Bott class of degree \(2\),

\[
\pi_*(KU)\cong\mathbb Z[u,u^{-1}],\qquad |u|=2.
\]

Thus the nonzero homotopy groups occur in **every even degree, positive or negative**. Unlike \(HA\), \(KU\) is *not connective*.

Real K-theory \(KO\) has eightfold Bott periodicity.

### Thom spectrum and cobordism

Let \(\gamma_n\) be the universal real \(n\)-plane bundle over \(BO(n)\). Its Thom space is

\[
\operatorname{Th}(\gamma_n)=D(\gamma_n)/S(\gamma_n).
\]

Adding a trivial real line to a bundle corresponds to suspension of its Thom space. The inclusions of universal bundles therefore yield

\[
\Sigma\operatorname{Th}(\gamma_n)
\longrightarrow
\operatorname{Th}(\gamma_{n+1}).
\]

These spaces assemble into the unoriented cobordism spectrum \(MO\). The Pontryagin–Thom construction identifies \(\pi_k(MO)\) with unoriented bordism of closed smooth \(k\)-manifolds.

This is a geometric reason spectra matter: the graded groups organize manifolds up to a geometric equivalence relation.

## 4. Homotopy groups of spectra

Let \(E\) be a sequential spectrum and \(q\in\mathbb Z\). Define

\[
\pi_q(E)
:=
\operatorname*{colim}_{n\to\infty}
\pi_{q+n}(E_n),
\]

starting at sufficiently large \(n\) that \(q+n\geq2\), so the displayed terms are abelian groups. The transition maps are induced by

\[
E_n\longrightarrow\Omega E_{n+1}.
\]

For an \(\Omega\)-spectrum, the transition maps become isomorphisms once the indices make sense, so each stable homotopy group can be computed at a sufficiently high level.

For the suspension spectrum of \(X\),

\[
\pi_q(\Sigma^\infty X)
=
\operatorname*{colim}_n\pi_{q+n}(\Sigma^nX),
\]

which recovers the stable homotopy groups of \(X\).

This definition works for **negative** \(q\). Negative degrees are not an afterthought: they are essential to desuspension and periodicity, especially in \(KU\).

## 5. Why naive maps between prespectra are not enough

A strict collection of level maps \(f_n:E_n\to F_n\) seems like the natural answer to the question “what is a map of spectra?” But the homotopy theory must formally invert *stable equivalences*.

Consider the Hopf map

\[
\eta:S^3\to S^2.
\]

Its stable class is an element

\[
\eta\in\pi_1(\mathbb S)
\cong[\Sigma\mathbb S,\mathbb S]_{\mathrm{Ho(Sp)}}.
\]

It is nonzero. Yet a strict level-zero map for a purported map \(\Sigma\mathbb S\to\mathbb S\) would include a pointed map \(S^1\to S^0\), which is constant. This illustrates why maps in the **localized stable homotopy category** cannot simply be identified with raw pointwise maps of the most naive prespectra.

Models using CW spectra, model categories, or stable \(\infty\)-categories account for this correctly.

One practical distinction:

\[
\text{levelwise equivalence} \implies \text{stable equivalence},
\]

but the converse does *not* hold.

## 6. What follows later in the seminar

The [course outline](https://www.math.purdue.edu/~pvankoug/spectra/outline.pdf) proposes, among other subjects:

- Model structures and stable equivalences, so that the correct maps of spectra are available.
- Smash products and structured models (symmetric or orthogonal spectra).
- Ring spectra and \(E_\infty\)-rings.
- The Atiyah–Hirzebruch and Adams spectral sequences.
- The Steenrod algebra, operations, cobordism, and chromatic applications.

These are subjects from the **proposed syllabus**, not a claim that each corresponding video has been individually identified.

## Exercises and checks

1. Write down \((\Sigma^\infty S^1)_n\) and compare it with \(\mathbb S_n\). In what sense is \(\Sigma^\infty S^1\simeq\Sigma\mathbb S\)?
2. Verify \(\pi_0(H\mathbb Z)\cong\mathbb Z\) directly from the colimit definition, and compute \(\pi_1(H\mathbb Z)\).
3. Why does \(KU\)'s periodicity imply a nonzero \(\pi_{-2}(KU)\)? Why could \(H\mathbb Z\) not represent complex K-theory?
4. Identify which property fails for \(S^n\to\Omega S^{n+1}\) to be a weak equivalence.
5. Describe the difference between a spectrum \(E\), a **spectrum** in functional analysis, and a **spectral sequence** \(E_r^{p,q}\). The names overlap; the objects do not.

## References and credits

Thanks to **Paul VanKoughnett** for the course and **Caleb Ji** for the preserved notes. The constructions discussed here are associated with **Samuel Eilenberg**, **Saunders Mac Lane**, **Raoul Bott**, **René Thom**, and **Lev Pontryagin**. For comprehensive sources, see **J. Frank Adams**, *Stable Homotopy and Generalised Homology*, Part III, and **David Barnes** and **Constanze Roitzheim**, *Foundations of Stable Homotopy Theory*. This file is independently phrased and does not reproduce the course notes.
