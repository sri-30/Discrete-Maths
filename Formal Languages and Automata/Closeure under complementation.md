![[Pasted image 20220221025102.png]]
E.g. Complement

>**Lemma**: If $L$ is a regular language over alphabet $\Sigma$, then its complement $\set{U \in \Sigma* | u \notin L}$ is also regular

**Proof**: Since $L$ is regular, by definition there is a DFA $M$ such that $L = L(M)$. Let $Not(M)$ be the DFA constructed from $M$ such that every accepting state becomes a non-accepting state and every non-accepting state becomes an accepting state. Then $\set{u \in \Sigma* \vert u \notin L}$ is the set of [[string]]s accepted by $Not(M)$ and hence is regular.

It is a consequence of [[Kleene's Theorem]] along with the above lemma that for each regular expression $r$ over an alphabet $\Sigma$, there is a regular expression $\neg r$ that determines via matching the complement of the language determined by $r$:
$$L(\neg r) = \set{u \in \Sigma*|u\notin L(r)}$$
To see this, given a regular expression $r$, by the first part of Kleene's Theorem there is a DFA $M$ such that $L(r) = L(M)$. Then by the second part of the theorem applied to the DFA $Not(M)$, we can find a regular expression $\neg r$ so that $L(\neg r) = L(Not(M))$. Since $L(Not(M)) = \set{u \in \Sigma* | u \notin L(M)} = \set{u \in Sigma*| u \notin L(r)}$, this $\neg r$ is the regular expression we need for the complement of $r$.

# Not(M)
Given DFA $M=(Q,\Sigma, \delta, s, F)$, then $Not(M)$ is the DFA with
- set of states $Q$
- input alphabet $\Sigma$
- next-state function $\delta$
- start state $s$
- accepting states $\set{q \in Q| q\notin F}$
Because $M$ is a deterministic finite automaton, then $u$ is accepted by $Not(M)$ iff it is not accepted by $M$:
$$L(Not(M)) = \set{u \in \Sigma* | u \notin L(M)}$$
