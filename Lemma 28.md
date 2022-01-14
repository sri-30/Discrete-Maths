For all integers $p$ and $m$, if $p$ is prime and $0 < m < p$ then ${p \choose m} \cong 0 \mod{p}$

Proof:
Let $p$, $m$ be arbitrary integers
Assume $p$ is prime and $0 < m < p$
RTP: ${p \choose m} \cong 0 \mod{p}$ or by definition $p |\frac {p!}{m!(p-m)!}$
Proof Strategy: [[Existential Quantification]]
$\frac {p!}{m!(p-m)!} = p \cdot \frac {(p-1)!}{m!(p-m)!}$

$p \cdot \frac {(p-1)!}{m!(p-m)!}$ is an integer

Hence $m!(p-m)!$ divides $p \cdot (p-1)!$

As $m < p$, $p-m < p$

By the [[Prime Factorisation Theorem]] 
$(m!(p-m)!)| (p-1)!$ and $\frac{(p-1)!}{m!(p-m)!}$ is an integer