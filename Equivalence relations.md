$R \subseteq A \times A$ is an equivalence relation whenever:

1. [[reflexive]]: $\forall x \in A. x R x$
2. [[symmetry]]: $\forall x, y \in A. x R y \implies y R x$
3. [[Transitive]]: $\forall x, y, z \in A. xRy \land yRz \implies xRz$

Notion of equality between sets

Examples:

- For a positive integer, let $R_m \subseteq \mathbb{Z} \times \mathbb{Z}$
$$x R_m y \iff x \cong y (mod m)$$
- Let $A$ be a set
	- $I \subseteq \mathcal{P}(A) \times \mathcal{P}(A)$
	- $= \set{(u,v) \in \mathcal{P}(A) \times \mathcal{P}(A)|u \cong v}$
![[Pasted image 20220131191610.png]]
A [[partition]] $P$ of a set $A$ is a [[set]] of subsets of $A$

$$P \subseteq \mathcal{P}(A)$$
such that

1. $\emptyset \notin P$
2. $\bigcup P = A$
3. $\forall u, v \in P. u \neq v \implies u \cap v = \emptyset$

Examples: Partitions of $\mathbb{Z}$

$P_1 = \set{\mathbb{Z}}$
$P_2 = \set{\text{Odd}, \text{Even}}$
$P_3 = \set{\set{3k, k \in \mathbb{Z}}, \set{3k+1, k \in \mathbb{Z}}, \set{3k+2, k \in \mathbb{Z}}}$




