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
