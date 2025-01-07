# Spectral Sequences and Homology

The homology definition \( H_n(A_ullet) \) of a chain complex is defined for arbitrary homology theories as the quotient \( \ker d_n / 	ext{im} \, d_{n+1} \). With respect to spectral sequences, there exists in a chain complex a differential that goes out of the group, in this case \( d_n \), and one that goes into the group, in this case \( d_{n+1} \). With this viewpoint, we can examine different homology groups depending on which differentials we use. Such an approach can be numbered and organized in what are known as *pages*. A spectral sequence behaves like a book consisting of an infinite number of pages. Each page is a two-dimensional grid of groups assigned to specific differentials. We can apply a natural transformation to move from one page to the next, and ideally, the pages stabilize to a *page limit* in the infinite. The notation for homologies is \( E^r_{p,q} \), where \( r \) represents the page number from a totally ordered index set \( (I,\leq) \), and \( p \in \mathbb{Z} \) and \( q \in \mathbb{Z} \) are the horizontal and vertical indices.

In some sense, each page of a spectral sequence behaves like a two-dimensional chain complex. The groups are indexed by two parameters rather than one, and each group has exactly one differential leading out of the group and one differential entering the group. Furthermore, it always holds that \( d^2 = 0 \).

### The Operation from \( E^r_{p,q} \) to \( E^{r+1}_{p,q} \)

What does the operation look like that leads us from \( E^r_{p,q} \) to \( E^{r+1}_{p,q} \)? The differentials on each page \( r \) depend heavily on the definition of the spectral sequence. Let us denote \( d_{\operatorname{IN}}, d_{\operatorname{OUT}} \) as the incoming and outgoing differentials of \( E^r_{p,q} \), then we define:

\[
E^{r+1}_{p,q} \coloneq \ker d_{\operatorname{OUT}} / 	ext{im} \, d_{\operatorname{IN}}
\]

The functioning of the spectral sequence consists of defining the groups on the first page \( E^1_{p,q} \). We then let the spectral sequence machinery work. In the case of the Serre spectral sequence, it stabilizes, meaning that there exists an \( R \) such that for all \( r > R \), we have \( E^r_{p,q} = E^R_{p,q} \). These are the entries of the stabilized page \( E^\infty_{p,q} \).

### Spectral Sequence Example: The Serre Spectral Sequence

We now describe what we need to put into our spectral sequence and what we can expect as an outcome, particularly with the example of Serre's spectral sequence.
