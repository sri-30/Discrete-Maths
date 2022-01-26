Let $(A, R)$ be a [[directed graph]]. For all $n \in \mathbb{N}$ and $s, t \in A, s R^{\circ n} t$ iff there exists a path of length $n$ in $R$ with source $s$ and target $t$.

Proof:

Paths:

A path of length $n$ from $s$ to $t$ is a sequence $s= a_0 R a_1 R a_2 ... R a_n = t$ 
In particular, there is always a path of length 0 from a node to itself.

Proof by induction on $n \in \mathbb{N}$

Base case $(n=0)$

$s R^{\circ(0)} t \iff \exists \text{path of length 0 from s to t}$
$s id_a t \iff s = t$


Inductive Step:

IH $s R^{(n)} t \iff \exists \text{path of length n from s to t}$
RTP: $s R^{(n+1)} t \iff \exists \text{path of length n+1 from s to t}$


[[Unfinished]]