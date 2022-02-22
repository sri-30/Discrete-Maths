![[Pasted image 20220222023640.png]]

In the context of programming languages, a typical example of a regular language is the set of all [[string]]s of characters which are well-formed tokens (basic keywords, identifiers etc) in a particular programming language. The set of all strings which represent well-formed programs is a typical example of a language that is not regular.

## Examples of languages that are not regular
- The set of strings over $\set{a,b,...,z}$ which are palindromes
- $\set{a^nb^n | n \geq 0}$ e.g. $aaabbb$

The finite number of states in a DFA limits how much it can "remember", hence why these are not regular languages.

# The Pumping Lemma
For every language $L$, there is a number $\mathcal{l} \geq 1$ satisfying the pumping lemma property:
> All $\mathcal{w} \in L$ with $\mathcal{w} \geq \mathcal{l}$ can be expressed as a concatenation of three strings, $\mathcal{w} = u_1\mathcal{v}u_2$, where $u_1, \mathcal{v}$ and $u_2$ satisfy:
> - $|v| \geq 1$ i.e. $\mathcal{v} \neq \varepsilon$
> - $|u_1v| \leq l$
> - for all $n \geq 0, u_1v^nu_2 \in L$

Every DFA has a number of states such that all the strings that exceed the number of states are pumpable as at some point they are doing a loop around the states. The loop can be repeated an arbitrary number of times.

If a language is regular, the pumping lemma is satisfied. If the language is not regular, it must violate the pumping lemma at some point.

# Proving a language is not regular
For each $l \geq 1$, find some $w \in L$ of length $\geq l$ so that no matter how $w$ is split into three, $w=u_1vu_2$, with $|u_1v| \leq l$ and $|v| \geq 1$, there is some $n \geq 0$ for which $u_1v^nu_2$ is not in $L$.

The following languages are not regular:
- $L_1 \triangleq \set{a^nb^n | n \geq 0}$ 
	- For each $l \geq 1, a^lb^l \in L_1$ is of length $\geq l$ and has the above property
	- E.g. $a^nb^n = aaaabbbb$ $w=a^ra^sa^{l-r-s}b^l$; pumping this string will always imbalance the number of $a$s and $b$s
- $L_2 \triangleq \set{w \in \set{a,b}* | w \text{ is a palindrome}}$
	- For each $l \geq 1, a^lba^l \in L_2$ is of length $\geq l$ and has the above property
- $L_3 \triangleq \set{a^p | p \text{ prime}}$
	- For each $l \geq 1$ we can find a prime $p$ with $p > 2l$ and then $a^p \in L_3$ has length $\geq l$ and has the above property