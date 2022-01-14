For all integers $n$, either $n^2 \cong 0 \mod{4}$ or $n^2 \cong 1 \mod{4}$

Proof:

RTP: $\forall n \in \mathbb{Z}. n^2 \cong 0 \mod{4} \lor n^2 \cong 1 \mod{4}$
or by definition $4|n^2 \lor 4|(n^2 - 1)$

Proof strategy: [[Disjunction]]

1. Case 1: $n$ is odd
Let $n = 2 \cdot k + 1$ where $k$ is an arbitrary integer.
$n^2 = (2 \cdot k + 1)^2 = 4\cdot k^2 + 4 \cdot k + 1$
$n^2 - 1 = 4 \cdot k^2 + 4 \cdot k = 4 \cdot (k^2 + k)$ so $4|(n^2-1)$
QED.

2. Case 2: $n$ is even
Let $n = 2 \cdot j$ where $j$ is an arbitrary integer.
$n^2 = 4 \cdot j^2$ so $4| n^2$
QED.

QED as the statement holds for all cases of $n$.