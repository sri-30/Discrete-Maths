![[Pasted image 20220213151943.png]]
Accepting states are indicated by the symbols with circular borders

# Language accepted by a finite automaton M
- Look at paths in the transition graph from the start state to *some* accepting state
- Each such path gives a [[string]] of input symbols, namely the string of labels on each transition in the path.
- The set of all such strings is by definition the language accepted by $M$, written $L(M)$

Notation: write $q \xrightarrow{u}* q'$ to mean that in the automaton there is a path from state $q$ to state $q'$ whose labels form the string $u$. (N.B. $q \xrightarrow{\epsilon}* q'$ means $q=q'$; path of length 0)
![[Pasted image 20220213152850.png]]
Claim:
$$L(m) = L((a|b)^{*}aaa(a|b){*})$$
	set of all strings matching the regular expression $(a|b)^{*}aaa(a|b){*}$

($q_i$(for $i=0,1,2$) represents the state in the process of reading a string in which the last $i$ symbols read were all $a$s)

# Determinism and non-determinism
The reason for the qualification 'non-deterministic' is because in general, for each state $q \in Q$ and each input symbol $a \in \Sigma$, there may be no, one, or many states that can be reached in a single transition labelled $a$ from $q$.

We single out as particularly important the case when there is always exactly one next state for a given input symbol in any given state and call such automata **deterministic**. The finite automaton shown above is deterministic. But note that if we took the same graph of transitions but insisted that the alphabet of input symbols was $\set{a,b,c}$ say, then we have specified an NFA not a DFA. When specifying an NFA, as well as giving the graph of state transitions it is important to say what is the [[alphabet]] of input symbols (because some input symbols may not appear in the graph at all).

# Non-deterministic finite automaton (NFA)
A 5-tuple $M=(Q,\Sigma,\Delta,s,F)$, where:
- $Q$ is a finite [[set]] (of states)
- $\Sigma$ is a finite set (the alphanet of input symbols)
- $\Delta$ is a subset of $Q \times \Sigma \times Q$ (the transition relation) (e.g. $Q_0 a Q_{17}$)
- $s$ is an element of $Q$ (the start state)
- $F$ is a subset of $Q$ (the accepting states)
Notation: write $q \xrightarrow{a} q'$ in $M$ to mean $(q, a, q') \in \Delta$

## Example of an NFA
![[Pasted image 20220213154611.png]]
The main difference is that inputting $a$ in state $q_0$ can lead to $q_0$ or $q_1$.

# Deterministic finite automaton (DFA)
>A deterministic finite automaton (DFA) is an NFA
>$M = (Q, \Sigma, \Delta, s, F)$ with the property that for each state $q \in Q$ and each input symbol $a \in \Sigma_{M}$, there is a unique state $q' \in Q$ satisfying $q \xrightarrow{a} q'$.

In a DFA $\Delta \subseteq Q \times \Sigma \times Q$ is a graph of a function $Q \times \Sigma \rightarrow Q$, which we write as $\delta$ and call the next-state function.

Thus for each (state, input symbol)-pair $(q,a), \delta(q,a)$ is the unique state that can be reached from $q$ by a transition labelled $a$:
$$\forall q' (q \xrightarrow{q} q' \iff q' = \delta(q,a))$$
## Example of a DFA
![[Pasted image 20220213155514.png]]
![[Pasted image 20220213155646.png]]
