### Definition

Theorems can usually be written in the form
>if a collection of assumptions hold, then so does some conclusion

or, in other words

> a collection of assumptions implies some conclusion

or, in symbols,
> a collection of hypotheses $\implies$ some conclusion

Identifying precisely what the assumptions and conclusions are is the first goal in dealing with a theorem.

### Proof strategy
To prove a goal of the form
$P \implies Q$
assume that $P$ is true and prove $Q$.

### Proof pattern:
In order to prove that $P \implies Q$
Write: Assume $P$.
Show that $Q$ logically follows.

### Example

If $m$ and $n$ are odd integers, then so is $m \cdot n$.

$m = 2 \cdot i + 1$ for some integer $i$ and $n = 2 \cdot j + 1$ for some integer $j$ $\implies m \cdot n = 2 \cdot k + 1$ for some integer $k$

Proof:
Assume $m$ and $n$ are odd integers
RTP: $m \cdot n$ is an odd integer
Let $m$ and $n$ be odd integers: $m = 2i +1$ for some integer $i$ and $n = 2j + 1$ for some integer $j$.

$m \cdot n = 4ij + 2i + 2j + 1 = 2 \cdot(2ij + i + j) + 1$ which is of the form $2 \cdot i + 1$ and so $m \cdot n$ is [[odd]] by definition.

QED.

### Alternative Proof Strategy
An alternative proof strategy for implication is to prove the equivalent statement given by its [[Contrapositive]].

### Use of implications
To use an assumption of the form $P \implies Q$, aim at establishing $P$. Once this is done, by [[Modus Ponens]], one can conclude $Q$ and so further assume it.

### Chaining Implications
**Theorem 11** Let $P_1$, $P_2$ and $P_3$ be statements. If $P_1 \implies P_2$ and $P_2 \implies P_3$ then $P_1 \implies P_3$.

Proof:
Assume (1) $P_1 \implies P_2$ and (2) $P_2 \implies P_3$
RTP: $P_1 \implies P_3$
Assume: (3) $P_1$
RTP: $P_3$
From (1) and (3), by [[Modus Ponens]], we have (4) $P_2$
From (2) and (4), by [[Modus Ponens]], we have $P_3$ as required.