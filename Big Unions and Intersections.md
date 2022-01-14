[[Powerset axiom]]

$\bigcup$ is logically $\exists$
$\bigcap$ is logically $\forall$

$\mathcal{D} = \set{T \subseteq[5] | \text{ The sum of the elements of T is less than or equal to 2}}$

$=\set{\emptyset, \set{0}, \set{1}, \set{0,1}, \set{0,2}}$

$\bigcup \mathcal{D}$ is the union of the sets in $\mathcal{D}$

$n \in \bigcup \mathcal{D} \iff \exists T \in \mathcal{D}. n \in T$

$\bigcup \mathcal{D} = \set{0, 1, 2}$

## Big Union Definition

Let $U$ be a set. For a collection of sets $\mathcal{F} \in \mathcal{P}(\mathcal{P}(U))$, we let the [[big union]] (relative to $U$) be defined as $\bigcup\mathcal{F} = \set{x \in U | \exists A \in \mathcal{F}.x \in A} \in \mathcal{P}(U)$

Examples:

$\bigcup (\mathcal{P}(U)) = \set{x \in U | \exists S \in \mathcal{P}(U). x \in S} = \set{x \in U | true} = U$

$\bigcup \emptyset = \set{x \in U| \exists S \in \emptyset, x \in S} = {x \in U | false} = \emptyset$

## Big Intersection Definition
Let $U$ be a set. For a collection of sets $\mathcal{F} \subseteq \mathcal{P}(U)$, we let the big intersection (relative to $U$) be defined as

$\bigcap \mathcal{F} = \set{x \in U| \forall A \in \mathcal{F}. x \in A}$

Instead of finding elements that exist for *some* sets in a family, the big intersection finds elements that exist for *all* sets in a family.

$\mathcal{S} = \set{S \subseteq [5]|\text{The sum of the lements of S equals 6}}$

$=\set{\set{2, 4}, \set{0, 2, 4}, \set{1, 2, 3}}$

$\bigcap(\mathcal{S})$ is the intersection of the sets in $\mathcal{S}$

$n \in \bigcap(\mathcal{S}) \iff \forall S \in \mathcal{S}. n \in S$

$\bigcap \mathcal{S} = \set{2}$

Examples:

$\bigcap(\mathcal{P}(U)) = \set{x \in U | \forall S \in \mathcal{P}(U). x \in S}$
$= \set{x \in U | false} = \emptyset$

$\bigcap(\emptyset) = \set{x \in U | \forall S \in \emptyset. x \in S}$
$= \set{x \in U | true} = U$

![[Pasted image 20211217123419.png]]