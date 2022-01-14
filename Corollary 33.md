[[Congruence]]

For all natural numbers $m$, $n$ and primes $p$,

$(m+n)^p \cong m^p + n^p\mod {p}$

Proof:

Let $m$ and $n$ be natural numbers and let $p$ be a prime

We have that $(m+n)^p = \sum_0^p {p \choose i}\cdot m^i \cdot n^{p-i} = m^p + n^p + \sum_1^{p-1} {p \choose i}\cdot m^i \cdot n^{p-i}$

$a_i \cong b_i \mod {m} \implies \sum_i a_i \cong \sum_i b_i\mod m$

${p \choose i}\cdot m^i \cdot n^{p-i} \cong 0 \mod {p}$ for all integers $i$ where $0 < i < p$ so $\sum_1^{p-1} {p \choose i}\cdot m^i \cdot n^{p-i} \cong 0 \mod {p}$

Therefore $p | ((m+n)^p - m^p - n^p)$

QED.