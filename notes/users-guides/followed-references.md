# Following the guides beyond their landing pages

[Guide catalogue](README.md) · [Yeakel notebook](../sarah-yeakel/README.md) · [Coverage and unfinished branches](crawl-log.md)

Checked 2026-10-09. A direct recommendation, a bibliography citation, and an editorially added reading suggestion are distinguished below. This is a finite reading map, not a claim to have exhausted the citation network.

## Direct recommendation: homotopy colimits

**Sarah Yeakel, imagery section → Daniel Dugger, *A primer on homotopy colimits*.**

[Recommending passage, section 2.1](https://mathusersguides.com/wp-content/uploads/2015/06/yeakel-t2.pdf) · [Dugger's text](https://pages.uoregon.edu/ddugger/hocolim.pdf)

Read: contents, introduction, initial examples, and bibliography. Start with section 2, then sections 4–6; return to sections 11 and 16 for bar constructions and coherence. The retrieved draft contains unfinished placeholders near its end. Its first pushout example and cylinder diagram were checked visually; the whole 109-page document was not read.

## Bibliography hop: calculus meets chromatic homotopy

**Yeakel's revised paper [Kuh07] → Nicholas J. Kuhn, *Goodwillie towers and chromatic homotopy: an overview*.**

[Primary record](https://arxiv.org/abs/math/0410342) · [Publisher](https://msp.org/gtm/2007/10/b015.html)

Read: metadata and abstract. This survey, published in 2007, connects towers of functors with applications to periodic homotopy. It offers a bridge between the Goodwillie and chromatic portions of this notebook; it is not an introduction starting from elementary single-variable calculus. A useful reading question is which information becomes simpler after periodic localization, and what has been discarded in doing so.

## Bibliography hop: operads, partitions, and bar constructions

**Yeakel's revised paper [Chi05] → Michael Ching, *Bar constructions for topological operads and the Goodwillie derivatives of the identity*.**

[Primary record](https://arxiv.org/abs/math/0501429)

Read: metadata and abstract. Bar and cobar constructions supply cooperadic and operadic structures; partition-poset models connect these constructions to derivatives of the identity. The paper also addresses modules and the relation to Lie structures on homology.

This is a technical reference, not a substitute for the friendly guide. A sensible worked example would begin with a small partition poset and its refinement relations before adding the spectrum-level interpretation. The exact identifications, dualities, and hypotheses still need paper-level study.

## Editorial addition: a later survey of the whole calculus

**Gregory Arone and Michael Ching, *Goodwillie Calculus* (2019).**

[Record](https://arxiv.org/abs/1902.00803) · [Text](https://arxiv.org/html/1902.00803)

Read: introduction and section 1; later sections mapped by their headings. The survey proceeds from polynomial approximation through homogeneous layers, the identity functor, extension/Tate data, and algebraic K-theory applications. Our [Goodwillie note](../sarah-yeakel/goodwillie-and-imagery.md) uses its definitions to keep the older guide's pictures separate from theorem statements.

This was added through the authors and subject of the bibliography, not discovered as a link in a 2017 guide. Reading section 4 is a natural next step for understanding why knowing every layer is not the same as knowing the tower.

## Historical update: the telescope conjecture

**Wolcott's 2016 guide → current-status check → Robert Burklund, Jeremy Hahn, Ishan Levy, Tomer M. Schlank, *K-theoretic counterexamples to Ravenel's telescope conjecture*.**

[Primary paper, 2023](https://arxiv.org/abs/2310.17459)

Read: metadata and abstract. The authors prove that telescopic and chromatic localizations differ at every prime and every height at least two. Consequently, the original telescope conjecture's open status in the old exposition is historical. This result does not, by itself, settle every distinct version formulated inside other localized categories.

A related expository lead is the same four authors' [*Arbeitsgemeinschaft: Algebraic K-Theory and Telescope Conjecture*](https://ems.press/journals/owr/articles/14298802), an Oberwolfach report on the 2024 workshop. Its description was inspected; the full report has not been studied here.

## Repairing a provisional source: cellular fluctuations

**Catanzaro guide → Michael J. Catanzaro's publication list → Catanzaro, Vladimir Y. Chernyak, and John R. Klein, *On fluctuations of cycles in a finite CW complex*.**

[Guide](https://mathusersguides.com/enchiridion-vol-2-2016-mike-catanzaro/) · [Author-maintained list](https://catanzaromj.github.io/publications/) · [Article record](https://arxiv.org/abs/1710.07995)

Read: guide selections, publication-list entry, and article abstract. The later article studies stochastic motion of cellular cycles and fractional quantization of average current in a low-temperature adiabatic limit. This is a verified related paper, not a silently assumed exact replacement for the guide's provisional manuscript. The author's [2016 thesis](https://digitalcommons.wayne.edu/oa_dissertations/1433) was identified but its full text was not retrieved.

## Friendly bridge: spectra, K-theory, transfer, and norm

**Yeakel's development story / Enchiridion collection → Cary Malkiewich's user's guide.**

[Detailed reading note](malkiewich-k-theory-bridge.md) · [Guide landing page](https://mathusersguides.com/enchiridion-vol-1-2015-cary-malkiewich/) · [Source paper](https://arxiv.org/abs/1503.06504)

All four guide sections were read. Malkiewich builds from a concrete “elements of spectra” picture to perfect modules, algebraic K-theory, group rings, assembly/coassembly, transfer, and the equivariant norm. His development story also shows why an attractive THH/TC route did not automatically prove the K-theory statement and why the eventual finite-set/norm model was cleaner.

For this notebook the most useful connection to Yeakel is structural: both stories discover that permutation data and coherent sums must be retained rather than replaced by an arbitrary ordering. Malkiewich also gives a clean place to keep (K(R)) (algebraic K-theory) separate from (K(n)) (Morava K-theory).

## Trace-methods branch: from K-theory to THH and TC

**Yeakel's prelim and public talks → Bökstedt's THH construction → Dundas–Goodwillie–McCarthy.**

[Yeakel K-theory/trace-methods notebook](../sarah-yeakel/k-theory-and-trace-methods.md) · [Sam Raskin, modern DGM account](https://arxiv.org/abs/1807.06709)

The 2013 prelim explicitly says that the use of finite sets and injections was inspired by Bökstedt's THH construction. Public programs then show a progression through Yeakel's 2015 algebraic K-theory introduction and the three-part 2017 Dundas–McCarthy lectures with Aaron Royer. Raskin gives a modern formulation and a proof organized around Goodwillie calculus.

The conceptual chain is useful but must not be shortened to “K and TC have the same derivative, therefore K=TC.” The theorem concerns relative fibers under connectivity/nilpotence hypotheses and uses substantially more structure.

## Workshop hop: several friendly entries into functor calculus

**2019 Functor Calculus Workshop at Ohio State.**

[Workshop page](https://people.math.osu.edu/osborne.422/functor-calculus-workshop/)

The program places several routes next to one another: Thomas Goodwillie on the origins of the subject, Brenda Johnson on abelian calculus, Michael Ching on Taylor towers and operadic structure, Ayelet Lindenstrauss on the Taylor tower of algebraic K-theory, Duncan Clark on higher excision, Jens Kjaer on periodic homotopy through a K-theory-based Goodwillie spectral sequence, and Sarah Yeakel on chain rules and operads in abelian functor calculus.

For this notebook, that workshop is more useful than treating every bibliography as a flat list: it exposes how algebraic K-theory, chromatic questions, Taylor towers, and operads were being taught as neighboring but distinct uses of calculus.

## Two bibliography leads that remain unresolved

Yeakel's revised bibliography lists **Kristine Bauer, Brenda Johnson, and Sarah Yeakel**, *Chain rules and operads for abelian functor calculus*, as in preparation, and **Sarah Yeakel**, *A classification of n-excisive functors to spectra*, as a preprint in preparation. Those are statuses in that historical bibliography, not assertions about their status today. No verified later publication record was established in this pass.

Source: [bibliography of arXiv:1706.06915v2](https://arxiv.org/html/1706.06915v2).

Thank you to every named author for making these research and expository connections available. The [attribution ledger](ACKNOWLEDGMENTS.md) also records authors from the bibliographies actually inspected.
