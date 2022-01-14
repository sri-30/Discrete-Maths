### Divisors

Given a natural number $n$, the [[set]] of its divisors is defined by the set comprehension as follows

$D(n) =$ {$d \in \mathbb{N} : d|n$}

Examples:

$D(0) = \mathbb{N}$
$D(12) =$ {$1, 2, 3, 4, 6, 12$}

### Common Divisors
$CD(m,n) =$ {$d \in \mathbb{N} : d | m \land d | n$} for $m,n \in \mathbb{N}$

Since $CD(n,n)=D(n)$, the computation of common divisors is as hard as that of divisors.

(1) $CD(m,n) = CD(n,m)$
(2) $CD(m,n \cdot m) = D(m)$

For a natural number $l$,
(1) $CD(l,l) = CD(l,0) = D(l)$
(2) $CD(1,l) =$ {1}

[[Lemma 56 (Key Lemma)]]:
Let $m$ and $m'$ be natural numbers and let $n$ be a positive integer such that $m \cong m' \mod{n}$. 

Then, $CD(m,n)=CD(m',n)$

As an application of this lemma, for a natural number $m$ and a positive integer $n$, since $m \cong rem(m,n) \mod {n}$, it follows that $CD(m,n) = CD(n, rem(m,n))$

For all positive integers $m$ and $n$

$CD(m,n) = D(n)$ if $n|m$ otherwise it is $CD(n, rem(m,n))$

Since a positive integer$n$ is the geatest divisor in $D(n)$, the lemma suggests a recursive procedure for computing the greatest common divisor:

$gcd(m,n) = n$ if $n|m$ otherwise it is $gcd(n,rem(m,n))$

This is [[Euclid's Algorithm]].

### GCD Definition
1. both $gcd(m,n)|m$ and $gcd(m,n)|n$
2. for all positive integers $d$ such that $d|m$ and$d|n$ it necessarily follows that $d|gcd(m,n)$