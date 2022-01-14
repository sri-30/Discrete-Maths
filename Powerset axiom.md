> For any [[set]], there is a set consisting of all its subsets.

$\mathcal{P}(U)$

$\forall X. X \in \mathcal{P}(U) \iff X \subseteq U$

$\mathcal{P}(\set{x, y, z})$
$= \set{\emptyset, \set{x}, \set{y}, \set{z}, \set{x, y}, \set{x, z}, \set{y, z}, \set{x, y, z}}$

$|\mathcal{P}(\set{x, y, z})| = 8$

$\forall U.|\mathcal{P}(U)| > 0$ because
$\emptyset \subseteq \mathcal{P}(U)$ as $\emptyset \subseteq U$ and 
$U \subseteq \mathcal{P}(U)$ as $U \subseteq U$

#### Hasse diagram of the Powerset $\mathcal{P}(\set{x, y, z})$
![[Pasted image 20211215135051.png]]

#### Iteration of the Powerset construction

$\mathcal{F} \in \mathcal{P}(\mathcal{P}(U) \iff \mathcal{F} \subseteq \mathcal{P}(U))$

that is, $\mathcal{F}$ is a set of subsets of $U$, sometimes referred to as a family.

Example:

The family $\mathcal{E} \subseteq \mathcal{P}([5])$ consisting of the non-empty subsets of $[5]=\set{0,1,2,3,4}$ all whose elements are even is $\mathcal{E}=\set{\set{0}, \set{2}, \set{4}, \set{0, 2}, \set{0, 4}, \set{2, 4}, \set{0, 2, 4}}$

#### Boolean Algebra

$(\mathcal{P}, \emptyset, U, \cup, \cap, (\cdot)^c)$

$\forall A,B \in \mathcal{P}(U)$

$A \cup B = \set{x \in U | x \in A \lor x \in B} \in \mathcal{P}(U)$

$A \cap B = \set{x \in U | x \in A \land x \in B} \in \mathcal{P}(U)$

$A^c = \set{x \in U | \neg(x \in A)} \in \mathcal{P}(U)$

The union operation $\cup$ and the intersection operation $\cap$ are [[Associative]], [[Commutative]] and idempotent.

$(A \cup B) \cup C = A \cup (B \cup C), A \cup B = B \cup A, A \cup A = A$

$(A \cap B) \cap C = A \cap (B \cap C), A \cap B = B \cap A, A \cap A = A$

The [[set]] with the union and intersection operations each form a [[Commutative]] [[Monoid]].

The empty set $\emptyset$ is a neutral element for $\cup$ and the universal set $U$ is a neutral element for $\cap$.

$\emptyset \cup A = A = U \cap A$

The empty set $\emptyset$ is an annihilator for $\cap$ and the universal set $U$ is an annihilator for $\cup$.

$\emptyset \cap A = \emptyset$
$U \cup A = U$

With respect to each other, the union operation $\cup$ and the intersection operation $\cap$ are [[Distributive]] and [[absorptive]].

$A \cap (B \cup C) = (A \cap B) \cup (A \cap C), A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$

$A \cup (A \cap B) = A = A \cap (A \cup B)$

The [[complement]] operation $(\cdot)^c$ satisfies complementation laws.

$A \cup A^c = U, A \cap A^c = \emptyset$

##### Proposition
$A \cup (A \cap B) = A$

Proof. $\forall x. x \in A \cup (A \cap B) \iff x \in A$

Let $x$ be arbitrary.

1. Assume $x \in A \cup (A \cap B)$

	Equivalently we are assuming $(x \in A \lor x \in A \cap B)$

	RTP $x \in A$

	Case $x \in A$, we are done

	Case $x \in A \cap B \iff (x \in A \land x \in B) \implies x \in A$
2. Assume $x \in A$
	
	RTP $x \in A \cup (A \cap B)$, which is the case because $x \in A$ by assumption.

QED

