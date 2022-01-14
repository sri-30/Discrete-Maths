### Definition

Sets are a well-defined, unordered collection of mathematical objects, called the elements or members of the set.

For set membership we use the symbol $\in$. This can be used like so $x \in A$ to show that $x$ is a member of the set $A$.

For the negation of set membership $\neg (x \in A)$ we write $x \notin A$

A set with only one element is known as a [[Singleton]].

### Enumerating elements

A set can be defined by enumerating the elements:

Examples:

The set of even primes: ${2}$
The set of booleans: ${true, false}$

### Set Comprehension
A set comprehension defines a set by means of a property that precisely characterises all the elements of the set.

Notations:

$\set{x \in A | P(x)}$, $\set{x \in A: P(x)}$
$a \in \set{x \in A | P(x)} \iff a \in A \land P(a)$

[[Russell's Paradox]]

##### With subsets
${x \in A | P(x)} \subseteq {y \in B | Q(y)}$
is equivalent to
$\forall z. [(z \in A) \land P(z)] \implies [(z \in B) \land Q(z)]$

### Equality

Two sets are equal precisely when they have the same elements:

$\forall \text{ sets } A, B. A = B \iff (\forall x. x \in A \iff x \in B)$

Examples:

{$x \in \mathbb{Z_m} | \text { x has a reciprocal in }\mathbb{Z_m}$} = {$x \in \mathbb{Z_m} | \text{ 1 is an integer linear combination of m and x}$}

**Proposition:**
$\forall b, c \in R$ let

$A = \set{x \in \mathbb{C} | x^2 - 2bx + c = 0}$
$B = \set{b + \sqrt{b^2-c}, b-\sqrt{b^2-c}}$
$C = \set{b}$

Then,

1. $A=B$
2. $b^2 = c \iff B=C$

For 1. $\set{x \in \mathbb{C} | x^2 - 2bx + c = 0} \equiv\set{b + \sqrt{b^2 -c}, b - \sqrt{b^2 -c}}$
Equivalently,
RTP: $\forall x \in \mathbb{C}. x^2 - 2bx + c = 0 \iff (x = b + \sqrt{b^2 - c} \lor x = b-\sqrt{b^2-c})$

RTP: $b^2 = c \iff \set{b + \sqrt{b^2-c}, b-\sqrt{b^2-c}} = \set{b}$

### Subsets and Supersets
$A \subseteq B$ - A is a subset of B or B is a superset of A

$A \subseteq B \iff \forall x. x \in A \implies x \in B$

$A = B \iff (A \subseteq B \land B \subseteq A)$

##### Proper subsets
$A \subset B$ stands for $A \subseteq B \land A \neq B$
Hence $A \subset B \iff (\forall x. x \in A \implies x \in B) \land (\exists y. y \notin A \land y \in B)$

### Properties of Sets
[[Lemma 83]]

[[Empty Set]]

[[Cardinality]]