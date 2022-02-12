>The subset $I \subseteq U$ with an [[inductive definition]] by a collection of axioms and rules is [[closed]] under them and is the least such subset: if $S \subseteq U$ is also closed under the axioms and rules, then $I \subseteq S$

Given axioms and rules for inductively defining a subset of a set $U$, we say that a subset $S \subseteq U$ is closed under the axioms and rules if
- for every axiom $\frac{}{a}$, it is the case the $a \in S$
- for every rule $\frac{h_1, h_2, ..., h_n}{c}$ if $h_1, h_2,...,h_n \in S$, then $c \in S$

We use a similar approach as method of proof: given a property $P(u)$ of elements of $U$