For all $n \in \mathbb{N}$,

$(x+y)^n = \sum^n_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^k$

Proof:

$P(n) = [(x+y)^n = \sum^n_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^k]$

RTP: $\forall n \in \mathbb{N}. P(n)$

We proceed by [[Mathematical Induction]].

**Base Case: $n = 0$**

$(x+y)^0 = 1$

$\sum^n_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^k = \sum^1_{k=0} {0 \choose k} \cdot x^{0-k} \cdot y^k = {0 \choose 0} \cdot x^0 \cdot y^0 = 1$

**Inductive Step**

Let $n$ be an arbitrary natural number. Assume $P(n)$

RTP: $P(n+1)$

RTP: $(x+y)^{n+1} = \sum^{n+1}_{k=0} {n+1 \choose k} \cdot x^{n+1-k} \cdot y^k$

$(x+y)^{n+1} = (x+y)^{n} \cdot (x+y) = (\sum^n_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^k) \cdot (x+y)$

$= \sum^n_{k=0} {n \choose k} \cdot x^{n-k+1} \cdot y^{k} + \sum^n_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^{k+1}$

$= x^{n+1} + (\sum^n_{k=1} {n \choose k} \cdot x^{n-k+1} \cdot y^{k}) + y^{n+1} + (\sum^{n-1}_{k=0} {n \choose k} \cdot x^{n-k} \cdot y^{k+1})$

$= x^{n+1} + (\sum^n_{k=1} {n \choose k} \cdot x^{n-k+1} \cdot y^{k}) + y^{n+1} + (\sum^{n}_{k=1} {n \choose {k-1}} \cdot x^{n-k+1} \cdot y^{k})$

*Lemma: ${n \choose k} + {n \choose k+1} = {n+1 \choose k}$*

$x^{n+1} + (\sum^n_{k=1} {n \choose k} \cdot x^{n-k+1} \cdot y^{k}) + y^{n+1} + (\sum^{n}_{k=1} {n \choose {k-1}} \cdot x^{n-k+1} \cdot y^{k})$

$= \sum^n_{k=1} {n+1 \choose k} \cdot x^{n+1-k} \cdot y^k + x^{n+1} + y^{n+1} =  \sum^{n+1}_{k=0} {n+1 \choose k} \cdot x^{n+1-k} \cdot y^k$

QED.



