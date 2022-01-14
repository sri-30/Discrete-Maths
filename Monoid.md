### Definition
A monoid is an algebraic structure with
- A neutral element, say $e$,
- A binary operation, say $*$,

satisfying
- neutral element laws: $e*x = x = x*e$
- associativity laws: $(x*y)*z=x*(y*z)$

A monoid is [[Commutative]] if
- commutativity: $x*y=y*x$ is satisfied

### Examples
- $(\alpha \text{ list}, \text{nil}, \text{@})$
	- $\text{nil@l=l=l@nil}$
	- $(l_1@l_2)@l_3=l_1@(l_2@l_3)$
	- This example is typically not [[Commutative]]
	- It is only [[Commutative]] when alpha is of the unit type
