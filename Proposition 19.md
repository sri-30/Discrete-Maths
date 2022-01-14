[[Universal Quantification]]

Fix a positive integer $m$. 

For integers $a$ and $b$, we have that $a \cong b \mod {m} \iff \forall n \in \mathbb{Z^+}.n\cdot a \cong n \cdot b \mod{n \cdot m}$

Proof:
Let $m$ be a fixed positive integer.
Let $a$ and $b$ be arbitrary integers.
RTP: $a \cong b \mod {m} \iff \forall n \in \mathbb{Z^+}.n\cdot a \cong n \cdot b \mod{n \cdot m}$
Proof Pattern: [[Bi-implication]]
1. Assume $\forall n \in \mathbb{Z^+}.n\cdot a \cong n \cdot b \mod{n \cdot m}$
	1. RTP: $a \cong b \mod {m}$
	2. By Universal Instantiation, let $n=1$, $1 \cdot a \cong 1 \cdot b \mod{1 \cdot m}$
	3. QED
2. Assume $a \cong b \mod {m}$
	1. RTP: $\forall n \in \mathbb{Z^+}.n\cdot a \cong n \cdot b \mod{n \cdot m}$
	2. By definition of [[Congruence]] we have to show that $\forall n \in \mathbb{Z^+}.(n \cdot m)|(n \cdot a - n \cdot b)$
	3. Moreover we must show that for some integer $k$, $n \cdot a - n \cdot b = n \cdot m \cdot k$
	5. By our assumption we have that $m|(a-b)$
	6. So for some integer $k'$, $a-b = k' \cdot m$
	7. Multiplying both sides by $n$ gives $n \cdot (a-b) = n \cdot k' \cdot m$
	8. Hence we have that $n \cdot a - n \cdot b = n \cdot m \cdot k'$ which is of the form $n \cdot a - n \cdot b = n \cdot m \cdot k$
	9. QED
3. QED by (1) and (2)