Regular Expressions and Finite Automata are equal

# From [[Regular Expression]]s to [[Finite Automata]]

## Definition
A language is regular iff it is equal to $L(M)$, the set of [[string]]s accepted by some deterministic finite automaton $M$.

> Theorem
> - For any regular expression $r$, the set $L(r)$ of strings matching $r$ is a regular language.
> - Conversely, every regular language is of the form $L(r)$ for some regular expression $r$.

### Base cases
Show that $\set{a}, \set{\epsilon}$ and $\emptyset$ are regular languages.

![[Pasted image 20220221004625.png]]

For $\set{a}$ state with starting state with transition through input $a$ to accepting state.

For $\epsilon$ make the starting state the accepting state.

For $\emptyset$ no arrows or accepting states.

### Induction step

$r_1|r_2$

Given NFA$^{\epsilon}$s $M_1$ and $M_2$, construct an NFA$^{\epsilon}$ $Union(M_1, M_2)$ satisyfing
> $L(Union(M_1, M_2)) = \set{u | u \in L(M_1) \lor u \in L(M_2)}$

Thus if $L(r_1) = L(M_1)$ and $L(r_2) = L(M_2)$ then $L(r_1 \vert r_2) = L(Union(M_1, M_2))$

![[Pasted image 20220221004650.png]]
![[Pasted image 20220221004728.png]]

$\epsilon$-transitions from start state to both machines

$\epsilon$-transitions from the accepting states of both machines to a single accepting state

$r_1 r_2$

Given NFA$^{\epsilon}$s $M_1$ and $M_2$, construct an NFA$^{\epsilon}$ $Concat(M_1, M_2)$ satisyfing
> $L(Concat(M_1, M_2)) = \set{u_1u_2 | u_1 \in L(M_1) \land u_2 \in L(M_2)}$

Thus if $L(r_1r_2)=L(Concat(M_1, M_2)$ when $L(r_1)=L(M_1)$ and $L(r_2)=L(M_2)$
![[Pasted image 20220221004750.png]]
![[Pasted image 20220221004906.png]]
$\epsilon$-transitions between accepting state of each machine and starting of the next.

$r^{*}$
Given an NFA$^{\epsilon}$ $M$ construct an NFA$^{\epsilon}$ $Star(M)$ satisyfing

> $L(Star(M)) = \set{u_1u_2...u_n|n\geq0 \text{ and each } u_i \in L(M)}$

Thus $L(r^{*}) = L(Star(M))$ when $L(r) = L(M)$
![[Pasted image 20220221004935.png]]
![[Pasted image 20220221004952.png]]
[[Unfinished]]

![[Pasted image 20220221005900.png]]

![[Pasted image 20220221010130.png]]
![[Pasted image 20220221010215.png]]

# From automaton to Regex
> Every regular language is of the form $L(r)$ for some regular expression $r$

> **Lemma**: Given an NFA $M=(Q, \Sigma, \Delta, s, F)$, for each subset $S \subseteq Q$ and each pair of states $q,q' \in Q$, there is a regular expression $r^{S}_{q,q'}$ satisfying
> $$L(r^{S}_{q,q'}=\set{u \in \Sigma^{*} | q \xrightarrow{u}* q' \text{ in M with all intermediate states of the sequence of transitions in S}}$$

Hence if the subset $F$ of accepting states has $k$ distinct elements, $q_1,...,q_k$ say, then $L(M)=L(r)$ with $r \triangleq r_1 | ... r_k$ where
$$r_i=r^{Q}_{s,q_i}. (i=1,...,k)$$
(in case $k=0$, we take $r$ to be the regular expression $\emptyset$)

## Proof of above Lemma
The regular expression $r^{S}_{q,q'}$ can be constructed by induction on the number of elements in the subset $S$.

### Base Case

$S$ is empty**. In this case, for each pair of states $q,q'$, we are looking for a regular expression to describe the set of strings

$$\set{u|q\xrightarrow{u}*q' \text{ with not intermediate states in the sequence of transitions}}$$
So each element of this set is either a single input symbol $a$ (if $q \xrightarrow{a} q'$ holds in $M$) or possibly $\varepsilon$ in case $q=q'$. If there are no input symbols that take us from $q$ to $q'$ in $M$, we can simply take
    $$r^{\emptyset}_{q,q'} \triangleq   \left\{
\begin{array}{ll}
      \emptyset & \text{if } q \neq q' \\
      \varepsilon & \text{if } q = q' \\
\end{array} 
\right.  $$
If there are some such input symbols, $a_1,...,a_k$ say, we can take
    $$r^{\emptyset}_{q,q'} \triangleq   \left\{
\begin{array}{ll}
      \ a_1 \vert ... \vert emptyset & \text{if } q \neq q' \\
      \ a_1 \vert ... \vert \varepsilon & \text{if } q = q' \\
\end{array} 
\right.  $$
### Induction Step
**Notation**: $X \backslash Y = \set{X \in X | x \notin Y}$ set of elements of $X$ that are not in $Y$. *Relative complement* of $X$ by $Y$.

Suppose we have defined the required regular expressions for all subsetss of states with $n$ elements. If $S$ is a subset with $n+1$ elements, choose some element $q_0 \in S$ and consider the $n$-element set $S \backslash \set{q_0} = \set{q \in S| q \neq q_0}$. Then for any pair of states $q,q' \in States_{M}$, by inductive hypothesis we have already constructed the regular expressions

$$r_1 \triangleq r_{q,q'}^{S \backslash \set{q_0}} \, r_2 \triangleq r_{q,q_0}^{S \backslash \set{q_0}} \, r_3 \triangleq r_{q_0,q_0}^{S \backslash \set{q_0}} \, r_4 \triangleq r_{q_0,q'}^{S \backslash \set{q_0}}$$
Consider the regular expression
$$r \triangleq r_1 | r_2(r_3)*r_4$$
Clearly every string matching $r$ is in the set

$$\set{u|q\xrightarrow{u}*q' \text{ with all intermediate states in the sequence of transitions in }S}$$
Conversely, if $u$ is in this set, consider the number of times the sequence of transitions $q \xrightarrow{u}* q'$ passes through state $q_0$. If this number is zero then $u