A preorder $(P, \sqsubseteq)$ consists of a [[Set]] $P$ and a relation $\sqsubseteq$ on $P$ (i.e. $\sqsubseteq \in \mathcal{P} (P \times P)$) satisfying the following two axioms:

[[Reflexivity]]: $$\forall x \in P, x \sqsubseteq x$$
[[Transitivity]]:

$$ \forall x, y, z \in P, (x \sqsubseteq y \land y \subseteq z) \implies x \sqsubseteq z$$

Examples:

- $(R, \leq)$ and $(R, \geq)$
- $(\mathcal{P}(A), \subseteq) and (\mathcal{P}(A), \supseteq)$
- $(\mathbb{Z}, |)$ - note $n| -n$ and $-n | n$ but $n \neq -n$ for $n \neq 0$



[[Partial order]]: A preorder such that ([[antisymmetry]]):

$$x \sqsubseteq y \land y \sqsubseteq x \implies x = y$$
