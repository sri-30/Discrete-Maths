## Principle of Induction

Let $P(m)$ be a statement for $m$ ranging over the set of [[natural]] numbers $\mathbb{N}$

**Base Case**
- If the statement $P(0)$ holds, and

**Induction Step**
- the statement $\forall n \in \mathbb{N}. (P(n) \implies P(n+1))$ also holds
- then the statement $\forall m \in \mathbb{N}. P(m)$ holds


## From basis $l$

**Base Case**
- If the statement $P(l)$ holds, and

**Induction Step**
- the statement $\forall n \geq l \in \mathbb{N}. (P(n) \implies P(n+1))$ also holds
- then the statement $\forall m \geq l \in \mathbb{N}. P(m)$ holds

## Principle of Strong Induction
###### From basis $l$ and Induction Hypothesis $P(m)$
Let $P(m)$ be a statement for $m$ ranging over the set of [[natural]] numbers greater than or equal to a fixed natural number $l$.

If both

- $P(l)$ and
- $\forall n \geq l \in \mathbb{N}. ((\forall k \in [l..n].P(k) \implies P(n+1)))$
then
- $\forall m \geq l in \mathbb{N}. P(m)$ holds

**Base Case**
- If the statement $P(0)$ holds, and

**Induction Step**
- the statement $\forall n \in \mathbb{N}. (P(n) \implies P(n+1))$ also holds
- then the statement $\forall m \in \mathbb{N}. P(m)$ holds