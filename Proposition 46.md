Let $m$ be a positive integer. For all natural numbers $k$ and $l$,

$k \cong l \mod {m} \iff rem(k,m) = rem(l,m)$

[[Bi-implication]]
[[Congruence]]

Proof:

Let $m$ be a positive integer
Let $k$ and $l$ be natural numbers

1. Assume $k \cong l \mod {m}$
RTP: $rem(k,m) = rem(l,m)$
$k-l = q \cdot m$ for an arbitrary integer $q$
$k = q \cdot m + l = q \cdot m + q_1 \cdot m + r$ where $q_1 \cdot m + r = l$ and $q_1, r$ are integers, where $r < m$
Hence $k = m \cdot (q+q_1) + r$ and $l = m \cdot q_1 + r$, and since $r < m$, it is the remainder for both $k$ and $l$ when divided by $m$.
QED

2. Assume $rem(k,m) = rem(l,m)$
RTP: $k \cong l \mod {m}$
By the assumption: $k = a\cdot m + r$ and $l = b\cdot m + r$ where $a, b, r$ are integers.
So $r = k - a \cdot m = l - b \cdot m$
$k - l = a \cdot m - b \cdot m$
$k - l = m \cdot (a - b)$
Since $a-b$ is an integer, this means $m|k-l$
QED by definition of [[Congruence]]

QED by 1. and 2.