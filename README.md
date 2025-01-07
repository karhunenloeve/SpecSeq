# 📘 Spectral Sequences and Homology

This document explains spectral sequences and homology in a concise and clear way. It delves into the basics of chain complexes, differentials, and the important notation of spectral sequences. The focus is placed on the Serre spectral sequence and its stabilization.

## Definition of Homology Groups

The homology definition $H_n(A_\bullet)$ of a chain complex is defined for arbitrary homology theories as the quotient:
$$
\ker d_n / \text{im} \, d_{n+1}
$$
With respect to spectral sequences, there exists in a chain complex a differential that goes out of the group, in this case $d_n$, and one that goes into the group, in this case $d_{n+1}$. This leads to a powerful framework for examining various homology groups depending on which differentials we use. These considerations are organized into what are called *pages*. 

### 📖 How Spectral Sequences Work

A spectral sequence behaves like a book with an infinite number of pages. Each page represents a two-dimensional grid of groups assigned to specific differentials. We move from one page to the next using a natural transformation, and ideally, the pages stabilize to a *page limit* in the infinite. 

The notation for homology groups is $E^r_{p,q}$, where $r$ denotes the page number from a totally ordered index set $(I,\leq)$, and $p, q \in \mathbb{Z}$ are the horizontal and vertical indices.

### 🔄 The Operation from $E^r_{p,q}$ to $E^{r+1}_{p,q}$

The differentials on each page $r$ are heavily dependent on the definition of the spectral sequence. We define the differentials $d_{\operatorname{IN}}$ and $d_{\operatorname{OUT}}$ as the incoming and outgoing differentials of $E^r_{p,q}$, and the operation from one page to the next is:
$$
E^{r+1}_{p,q} \coloneq \ker d_{\operatorname{OUT}} / \text{im} \, d_{\operatorname{IN}}
$$

### ✨ Serre Spectral Sequence Example

The Serre spectral sequence is a concrete example where the sequence stabilizes. There exists an $R$ such that for all $r > R$, we have:
$$
E^r_{p,q} = E^R_{p,q}
$$
These entries form the stabilized page $E^\infty_{p,q}$, and we will go over the essential concepts needed to populate the spectral sequence.

## 📥 Download the PDF

For a printable version of this material in PDF format, [click here to download](https://karhunenloeve.github.io/SpecSeq/main.pdf).

---

### ⚡ Highlights

- **Spectral Sequences:** A versatile tool for homological computations.
- **Stabilization:** Key insight of the Serre spectral sequence.
- **Visual Representation:** Pages behave like two-dimensional chain complexes.

## 📚 Further Reading

For deeper exploration into homology theories and spectral sequences, here are some resources:
- [Homology and Spectral Sequences – MathWorld](https://mathworld.wolfram.com/Homology.html)
- [Introduction to Spectral Sequences – SAGE](https://doc.sagemath.org/html/en/thematic_tutorials/spectral-sequences.html)

Enjoy your journey into the fascinating world of algebraic topology and homology theory!
