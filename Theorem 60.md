[[Euclid's Algorithm]] gcd terminates on all pairs of positive integers and, for such $m$ and $n$, $gcd(m,n)$ is the greatest common divisor of $m$ and $n$ in the sense that the following two properties hold:

1. both $gcd(m,n)|m$ and $gcd(m,n)|n$
2. for all positive integers $d$ such that $d|m$ and$d|n$ it necessarily follows that $d|gcd(m,n)$

$CD(m,n)=D(k) \iff [\forall d \in \mathbb{N} (d|m \land d|n) \iff d|k]$

$\iff [(k|m \land k|n) \land (\forall d \in \mathbb{N}. d|m \land d|n \implies d|k)]$

### Proving that these properties uniquely characterise $k$

Suppose for an integer $k_1$

1. $(k_1|m \land k_1|n)$
2. $\forall d \in \mathbb{N}. d|m \land d|n \implies d|k_1$

and

3. $(k_2|m \land k_2|n)$
4. $\forall d \in \mathbb{N}. d|m \land d|n \implies d|k_2$
Then we claim $k_1 = k_2$

By (1) we can see that $k_1|m \land k_1|n$, so by property (4), $k_1|k_2$. However by properties (3) and (2) we can also see that $k_2|k_1$. Therefore $k_1 = k_2$ necessarily.
QED.