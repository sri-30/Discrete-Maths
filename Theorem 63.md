[[Greatest Common Divisor]]

For positive integers $k$, $m$ and $n$, if $k|(m\cdot n)$ and $gcd(k,m)=1$ then $k|n$.

Proof:
Assume $k|(m\cdot n)$ and $gcd(k,m) = 1$

$n\cdot gcd(k,m) = n = gcd(n\cdot k, n\cdot m)$

Since $k| (m \cdot n)$, $m \cdot n = l \cdot k$ for some integer $l$, so $gcd(n\cdot k, n \cdot m) = gcd(n \cdot k, l \cdot k) = k \cdot gcd(n,l)$

$k \cdot gcd(n,l) = n$

Hence by definition $k | n$

QED.