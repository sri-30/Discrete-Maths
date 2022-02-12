# Axioms and rules
For inductively defining a subset of a given [[formal language]] $U$
- axioms $\frac{}{a}$ are specified by giving an element $a$ of $U$ ($a$ is always in the language)
- rules $\frac{h_1,h_2,...,h_n}{c}$ are specified by giving a finite subset $\set{h_1,h_2,...,h_n}$ of $U$ (the hypotheses of the rule) and an element $c$ of $U$ (the conclusion of the rule)

# Derivations
Given a [[set]] of axioms and rules for inductively defining a subset of a given set $U$, a derivation (or proof) that a particular element $u \in U$ is in the subset is by definition a finite tree with vertices labelled by elements of $U$ and such that:
- the root of the tree is $u$ (the conclusion of the whole derivation)
- each vertex of the tree is the conclusion of a rule whose hypotheses are the children of the node
- each leaf of the tree is an axiom

![[Pasted image 20220212195705.png]]

# Inductively defined subsets
> Given a set of axioms and rules over a set $U$, the subset of $U$ inductively defined by the axioms and rules consists of all and only the elements of $u \in U$ for which there is a derivation with conclusion $u$

For example (using the above axioms and rules):
- $abaabb$ is in the subset defined inductively
- $abaab$ is not in that subset (there is no derivation with that conclusion as there are different numbers of the letters $a$ and $b$ in the [[string]])