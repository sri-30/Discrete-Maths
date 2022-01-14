## Definition

[[Ordered Pairing]]

The product of $A \times B$ of two [[set]]s $A$ and $B$ is the set

> $A \times B = \set{x| \exists a \in A, b \exists B. x=(a,b)}$
> $= \set{(a,b)| a \in A \land b \in B}$

where
$\forall a_1,a_2 \in A, b_1, b_2 \in B. (a_1,b_1) = (a_2,b_2) \iff (a_1 = a_2 \land b_1 = b_2)$

Thus,

$\forall x \in A \times B. \exists! a \in A. \exists! b \in B. x = (a,b)$

## Pattern-Matching Notation
For a property $P(a,b)$ with $a$ ranging over a set $A$ and $b$ ranging over a set $B$,

$\set{(a,b) \in A \times B | P(a,b)}$

abbreviates

$\set{x \in A \times B | \exists a \in A. \exists b \in B. x = (a,b) \land P(a,b)}$

Example:

The subset of ordered pairs from a set $A$ with equal componenets (the diagonal) is formally

$\set{x \in A \times A | \exists a_1 \in A. \exists a_2 \in A. x=(a_1,a_2) \land a_1=a_2}$

but often abbreviated using pattern-matching notation as

$\set{(a_1,a_2) \in A \times A | a_1=a_2}$