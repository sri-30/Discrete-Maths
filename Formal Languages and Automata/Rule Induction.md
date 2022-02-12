>The subset $I \subseteq U$ with an [[inductive definition]] by a collection of axioms and rules is [[closed]] under them and is the least such subset: if $S \subseteq U$ is also closed under the axioms and rules, then $I \subseteq S$

Given axioms and rules for inductively defining a subset of a set $U$, we say that a subset $S \subseteq U$ is closed under the axioms and rules if
- for every axiom $\frac{}{a}$, it is the case the $a \in S$
- for every rule $\frac{h_1, h_2, ..., h_n}{c}$ if $h_1, h_2,...,h_n \in S$, then $c \in S$

We use a similar approach as method of proof: given a property $P(u)$ of elements of $U$, to prove $\forall u \in I. P(u)$ it suffices to show

- base cases: $P(a)$ holds for each axiom $\frac{}{a}$
- induction steps: $P(h_1) \land P(h_2) \land ... \land P(h_n) \implies P(c)$ holds for each rule $\frac{h_1,h_2,...,h_n}{c}$
![[Pasted image 20220212203514.png]]

## Example
![[Pasted image 20220212204609.png]]
