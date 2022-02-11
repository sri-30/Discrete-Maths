## Lauwvere's [[fixed-point]] argument
For sets $A$ and $X$, if there exists a [[surjection]] $A \twoheadrightarrow (A \Rightarrow X)$ then every function $X \rightarrow X$ has a fixed-point; and hence $X$ is a [[singleton]].

Proof:
If every function on $X$ has a fixed-point then $X$ is a singleton.

Suppose $x_1 \in X, x_2 \in X$ and $x_1 \neq x_2$
Define $X \rightarrow X :$ $x_1 \mapsto x_2$, $x \neq x_1 \mapsto x_1$

Suppose we have an enumeration $e: A \twoheadrightarrow (A \Rightarrow X)$
Let $f: X \rightarrow X$ and define
$s: A \rightarrow X, s(a) = f(e(a)(a))$
$\exists \alpha. e(\alpha) = s$
$e(\alpha)(\alpha)=s(\alpha)=f(e(\alpha)(\alpha))$

## Corollary
The sets
$$\mathcal{P}(\mathbb{N}) \cong (\mathbb{N} \Rightarrow [2]) \cong [0,1] \cong \mathbb{R}$$
are not enumerable