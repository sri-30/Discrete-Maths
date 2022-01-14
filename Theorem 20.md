[[Divisibility]]

For every integer $n$, we have that $6|n \iff 2|n \land 3|n$

Proof:
Let $n$ be an arbitrary integer.
RTP: $6|n \iff 2|n \land 3|n$
Proof patterns: [[Bi-implication]] and [[Conjunction]]
1. Assume $6|n$
	1. RTP $2|n \land 3|n$
		1. RTP $2|n$
			1. Since $2|6$ and $6|n$ by the lemma $a|b \land b|c \implies a|c$, $2|n$
			2. QED
	2. RTP $3|n$
		1. Since $3|6$ and $6|n$ by the lemma $a|b \land b|c \implies a|c$, $3|n$
		2. QED
2. Assume $2|n \land 3|n$
	1. RTP: $6|n \iff n = 6\cdot k$ for some integer k
	2. By the assumption we have that $n=2 \cdot i = 3 \cdot j$ for integers $i, j$
	3. $3 \cdot n = 6\cdot i$ and $2 \cdot n = 6 \cdot j$
	4. So $n = 3 \cdot n - 2\cdot n = 6 \cdot i - 6 \cdot j = 6 \cdot (i - j)$
	5. QED
3. QED by 1. and 2.