A positive real number $x$ is rational iff $\exists$ positive integers $m,n: x = m/n \land \neg(\exists \textrm{prime } p: p|m \land p|n)$

Proof:
Assume $x$ is rational: $x = a/b$ for integers $a$ and $b$
RTP: $m,n: x = m/n \land \neg(\exists \textrm{prime } p: p|m \land p|n)$

We proceed by [[Proof by Contradiction]]

To that end assume $m,n: x = m/n \land \neg(\exists \textrm{prime } p: p|m \land p|n)$ is not the case.

So for all positive integers m and n, 

$\neg (x = m/n) \lor (\exists \text{prime }p. p|m \land p|n)$

$\iff$

$\forall m, n. x=m/n \implies \exists \text{prime }p. p|m \land p|n$

Recall $x = a/b$

By instantiation

$x = a/b \implies \exists \text{prime } p. p|a \land p|b$

Hence

$\exists \text{prime }p. p|a \land p|b$

So $a = p_0 \cdot a_1$ and $b = p_0 \cdot b_1$ for a prime $p_0$ and integers $a_1$, $b_1$

Then $x = a_1/b_1$

By instantiation
$x = a_1/b_1 \implies (\exists \text{prime }p. p|a_1 \land p|b_1$)