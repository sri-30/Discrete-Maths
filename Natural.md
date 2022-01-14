### Definition

Natural [[Numbers]] are defined by the following sequence:

$\mathbb{N} : 0, 1,...,n,n+1,...$

They are generated from zero by successive increment

### Additive structure
The additive structure $( \mathbb{N}, 0, +)$ of natural numbers with zero and addition satisfies the following:
- [[Monoid]] Laws
	- A neutral element (0) is present
	- The operation is [[Associative]]
	- $0 + n = n = n + 0$, $(l+m)+n=l+(m+n)$
- [[Commutative]]
	- $m+n=n+m$

This additive structure is hence referred to as a [[Commutative]] monoid.

### Multiplicative Structure
The multiplicative structure $(\mathbb{N},1,\cdot)$ of natural numbers with one and multiplication is also a [[Commutative]] monoid:
- Monoid laws
	- $1\cdot n = n = n \cdot 1$, $(l \cdot m)\cdot n = l \cdot (m \cdot n)$
- Commutativity laws
	- $m \cdot n = n \cdot m$

### Distributivity
These additive and multiplicative structures interact nicely in that they are [[distributive]]: $l \cdot (m+n) = l\cdot m + l \cdot n$

This makes the overall structure $(\mathbb{N},0,+,1,\cdot)$ into something known as a [[Commutative]] [[Semiring]].

### [[Cancellation]]
The additive and multiplicative structures of natural numbers further satisfy the following laws.

- Additive cancellation
	- For all natural numbers $k, m, n,$
		- $k+m=k+n \implies m = n$
- Multiplicative cancellation
	- For all natural numbers $k, m, n,$
		- if $k \ne 0$ then $k \cdot m = k \cdot n \implies m = n$
### [[Inverses]]
1. A number $x$ is said to admit an additive inverse whenever there exists a number $y$ such that $x+y=0$
	- The only natural number with an additive inverse is 0
1. A number $x$ is said to admit a multiplicative inverse whenever there exists a number $y$ such that $x \cdot y = 1$
	- The only natural number with a multiplicative inverse is 1

Extending the system of natural numbers to:

1. admit all additive [[Inverses]] and then
2. also admit all multiplicative [[Inverses]] for non-zero numbers yields two very interesting results

From 1. we obtain the [[Integers]]
And applying 2. gives the [[Rational]] numbers.