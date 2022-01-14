For every [[Natural]] number $m$ and positive natural number $n$, there exists a unique pair of [[Integers]] $q$ and $r$ such that $q \geq 0, 0 \leq r < n$, and $m = q \cdot n + r$.

#### Computing $Q$ and $R$


#### Uniqueness:
For natural number $m$ and positive natural number $n$,
If $m = q_1 \cdot n + r_1$ with $q_1 \geq 0$ and $0 \leq r_1 < n$
and $m = q_2 \cdot n + r_2$ with $q_2 \geq 0$ and $0 \leq r_2 < n$
then $q_1 = q_2$ and $r_1 = r_2$

Suppose
(1) $m = q_1 \cdot n + r_1, q_1 \geq 0, 0 \leq r_1 < n$
and
(2) $m = q_2 \cdot n + r_2, q_2 \geq 0, 0 \leq r_2 < n$
RTP: $q_1 = q_2$ and $r_1 = r_2$

From (1) and (2), $q_1 \cdot n + r_1 = q_2 \cdot n + r_2$

$r_1 \geq r_2$

Then $(q_1 - q_2) \cdot n = r_1 - r_2 < n \implies q_1 = q_2$
So $q_1 \cdot n = q_2 \cdot n$ so by [[Cancellation]] $r_1 = r_2$
QED
