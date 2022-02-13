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

We single out as particularly important the case when there is always exactly one next state for a given input symbol in any given state and call such automata **deterministic**. The finite automaton shown above is deterministic. But note that if we took the same graph of transitions but insisted that the alph