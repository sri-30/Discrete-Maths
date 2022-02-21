Regular Expressions and Finite Automata are equal

# From [[Regular Expression]]s to [[Finite Automata]]

## Definition
A language is regular iff it is equal to $L(M)$, the set of [[string]]s accepted by some deterministic finite automaton $M$.

> Theorem
> - For any regular expression $r$, the set $L(r)$ of strings matching $r$ is a regular language.
> - Conversely, every regular language is of the form $L(r)$ for some regular expression $r$.

### Base cases
Show that $\set{a}, \set{\epsilon}$ and $\emptyset$ are regular languages.

![[Pasted image 20220221003621.png]]

For $\set{a}$ state with starting state with transition through input $a$ to accepting state.

For $\em

### Induction step

$r_1|r_2$

Given NFA$^{\epsilon}$s $M_1$ and $M_2$, construct an NFA$^{\epsilon}$ $Union(M_1, M_2)$ satisyfing
> $L(Union(M_1, M_2)) = \set{u | u \in L(M_1) \lor u \in L(M_2)}$

Thus if $L(r_1) = L(M_1)$ and $L(r_2) = L(M_2)$ then $L(r_1 \vert r_2) = L(Union(M_1, M_2))$

$r_1 r_2$

Given NFA$^{\epsilon}$s $M_1$ and $M_2$, construct an NFA$^{\epsilon}$ $Concat(M_1, M_2)$ satisyfing
> $L(Concat(M_1, M_2)) = \set{u_1u_2 | u_1 \in L(M_1) \land u_2 \in L(M_2)}$

Thus if $L(r_1r_2)=L(Concat(M_1, M_2)$ when $L(r_1)=L(M_1)$ and $L(r_2)=L(M_2)$

![[Pasted image 20220221003804.png]]

$r^{*}$
Given an NFA$^{\epsilon}$ $M$ construct an NFA$^{\epsilon}$ $Star(M)$ satisyfing

> $L(Star(M)) = \set{u_1u_2...u_n|n\geq0 \text{ and each } u_i \in L(M)}$

Thus $L(r^{*}) = L(Star(M))$ when $L(r) = L(M)$
