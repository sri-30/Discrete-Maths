### Definition
For a [[Monoid]] with a neutral element $e$ and a binary operation $*$, an element $x$ is said to admit an:
- inverse on the left if there exists an element $l$ such that $l*x=e$
- inverse on the right if there exists and element $r$ such that $x*r=e$
- inverse if it admits both left and right inverses

### Reciprocals in [[Modular Arithmetic]]
Let $m$ be a positive integer. A modular integer $x$ in $\mathbb{Z_m}$ has a reciprocal iff there exist integers $i$ and $j$ such that $x \cdot i + m \cdot j = 1$ 

Proof: Let $m$ be an arbitrary positive integer and $x$ in $\mathbb{Z_m}$

1. Assume $x$ has a reciprocal, that is by definition, there is some $z$ in $\mathbb{Z_m}$ such that $x \cdot z \cong 1 \mod {m}$
	
	RTP: There exist integers $i$ and $j$ such that $x \cdot i + m \cdot j = 1$ 
 
	$x \cdot z - 1 = m \cdot k$ for some integer $k$

	Hence $x \cdot z - m \cdot k = 1$

	QED as $j$ has been instantiated as $-k$.

2. Assume there exist integers $i$ and $j$ such that $x \cdot i + m \cdot j = 1$ 
	RTP: $x$ has a reciprocal in $\mathbb{Z_m}$, moreover that there exists an integer $k$ in $\mathbb{Z_m}$ such that $x \cdot k \cong 1 \mod {m}$
	
	Let $z = [i]_m$
	
	$x \cdot i - 1 = - m \cdot j$
	
	$x \cdot i \cong 1 \mod {m}$
	
	QED
	
QED by 1. and 2.
