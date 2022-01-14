## Definition

> For every $a$ and $b$, there is a set with $a$ and $b$ as its only elements.

$\set{a, b}$

is defined by

$\forall x. x \in \set{a, b} \iff (x = a \lor x = b)$

The set $\set{a, a}$ is abbreviated as $\set{a}$, and referred to as a [[singleton]].

## Proposition
$\forall a, b, c, x, y:$
1. $\set{x,y} \subseteq \set{a} \implies (x = a \land y = a)$
2. $\set{c,x} = \set{c,y} \implies x=y$

Proof: 

1. Assume $\set{x,y} \subseteq \set{a}$
	Then since $x \in \set{x, y} \implies x \in \set{a} \implies x=a$
	Analagously for $y=a$
2. Assume $\set{c,x} = \set{c,y} \implies x=y$
Then $(x=c \lor x=y) \land (y=c \lor y=x)$
[[Unfinished]]