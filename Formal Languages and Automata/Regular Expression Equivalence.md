![[Pasted image 20220222022122.png]]

> **Definition**: Two regular expressions $r$ and $s$ are said to be **equivalent** if $L(r) = L(s)$, that is, they determine exactly the same sets of [[string]]s via [[regular expression matching]].

For example $b*a(b*a)*$ and $(a|b)*a$ are equivalent.

$L(r) = L(s)$

iff

- $L(r) \subseteq L(s)$ and $L(s) \subseteq L(r)$
- $(\Sigma* \backslash L(r)) \cap L(s) = \emptyset = (\Sigma* \backslash L(s)) \cap L(r)$
- $L((\neg r) \land s) = \emptyset = L((\neg s) \land r)$
- $L(M) = \emptyset = L(N)$

where $M$ and $N$ are DFAs accepting the sets of strings matched by the regular expressions $(\neg r) \land s$ and $(\neg s) \land r$ respectively.

So to decide equivalence for regular expressions it suffices to check, given any given DFA $M$, whether or not it accepts some string.

The number of transitions needed to reach an accepting state in a finite automaton is bounded by the number of states (we can remove loops from longer paths). So we only have to check finitely many strings to see whether or not $L(M)$ is empty.