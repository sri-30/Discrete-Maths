For every positive integer $n$ there exists a unique finite sequence of primes $(p_1, ..., p_l)$ with $l \in \mathbb{N}$ such that $n = \pi (p_1, ..., p_l)$.

### Proof of finite sequence:

We prove $\forall n \geq 1 \in \mathbb{N}. P(n)$ where there exists a finite sequence of primes $P(n) = (p_1, ..., p_l)$ with $l \in \mathbb{N}$ such that $n = \pi (p_1, ..., p_l)$. By strong [[mathematical induction]].

$\pi () = 1$
$\pi (P) = P$

**Base Case**

$P(1)$

1 = $\pi()$

**Inductive Step**

Let $n$ be a positive integer

Assume the inductive hypotheses that for all $l \leq l \leq n, l =$ the product of a finite sequence of primes.

RTP: $n+1 =$ the product of a finite sequence of primes

- Case 1: If $n+1$ is a prime, say $p$, then $n+1$ = $\pi (p)$

- Case 2: If $n+1$ is composite, that is $n+1 = i \cdot j$ for some $1 \leq i, j \leq n$ and $i$ and $j$ can be expressed as the products of finite sequences of primes according to the induction hypotheses, therefore $n+1$ also can.
$i = \pi(p_1 ... p_k)$ for primes $p_1 ... p_k$
$j = \pi(q_1 ... q_l)$ for primes $q_1 ... q_l$
so $n+1 = \pi (p_1 ... p_k, q_1 ... q_l)$

QED.

### Proof of Uniqueness:

$\forall m \in \mathbb{N}. P(m)$

where

$P(m)$ = for all primes $(p_1 \leq ... \leq p_m)$ and for all $n \in \mathbb{N}$ and primes $(q_1 \leq ... \leq q_n)$ if $\pi^m_{i=1}p_i = \pi^n_{j=1}q_j$ then $m=n$ and $\forall 1 \leq k \leq m. p_k = q_k$ by induction.

**Base Case**

$P(0)$

$1 = \pi^m_{j=1}q_j \implies m=0$

Assume $1 = \pi^m_{j=1}q_j \geq 2^m$ as $2$ is the smallest prime
Then $1 \geq 2^m$
Hence $m=0$

**Inductive Step**

Assume the inductive hypothesis for $m \in N$

$P(m)$ = for all primes $(p_1 \leq ... \leq p_m)$ and for all $n \in \mathbb{N}$ and primes $(q_1 \leq ... \leq q_n)$ if $\pi^m_{i=1}p_i = \pi^n_{j=1}q_j \implies m=n \land \forall 1 \leq k \leq m. p_k = q_k$

RTP: $P(m+1)$

Consider $s_1 \leq s_2 \leq ... \leq s_m \leq s_{m+1}$ primes. $t_1 \leq t_2 \leq ... \leq t_{l}$ such that $\pi(s_1 \leq s_2 \leq ... \leq s_m \leq s_{m+1}) = \pi(t_1 \leq t_2 \leq ... \leq t_{l})$

RTP: $l=m+1$ and $s_k=t_k$ for $1 \leq k \leq m+1$

$s_1 | \pi(t_1 \leq t_2 \leq ... \leq t_{l})$

So $s_1 = t_{j0}$ for some $j_0$ and $t_1 \leq s_1$

Analogously $s_1 \leq t_1$ and hence $s_1 = t_1$

Since $\pi(s_1 \leq s_2 \leq ... \leq s_m \leq s_{m+1}) = \pi(t_1 \leq t_2 \leq ... \leq t_{l})$ and $s_1 = t_1$ we have that $\pi(s_2 \leq s_3 \leq ... \leq s_m \leq s_{m+1}) = \pi(t_2 \leq t_3 \leq ... \leq t_{l})$

$\pi(s_2 \leq s_3 \leq ... \leq s_m \leq s_{m+1})$ is a sequence of length $m$, so by the induction hypothesis $m = l-1 \implies l = m+1$ and $s_k = t_k$ for all $k = 2...m+1$

QED.