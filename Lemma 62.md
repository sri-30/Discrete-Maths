Fundamental Properties of the [[Greatest Common Divisor]]

1. (Commutativity) $gcd(m,n) = gcd(n,m)$
2. (Associativity) $gcd(l,gcd(m,n)) = gcd(gcd(l,m),n)$
3. (Linearity) $gcd(l \cdot m, l\cdot n) = l \cdot gcd(m,n)$

Proof of (3):

$gcd(l \cdot m, l\cdot n)$ and $l \cdot gcd(m,n)$ satisfy the same properties

$l \cdot gcd(m,n)$ satisfies the following

1. $(l \cdot gcd(m,n))|l\cdot m$ and$(l \cdot gcd(m,n))|l\cdot n$
2. $\forall d \in \mathbb{N}. d|l\cdot m \land d|l \cdot n \implies d| l\cdot gcd(m,n)$

##### Proof of 1

RTP: $l \cdot gcd(m,n) | l\cdot m$

Since $gcd(m,n) | m$ then $l \cdot gcd(m,n) | l\cdot m$

RTP: $l \cdot gcd(m,n) | l\cdot n$

Since $gcd(m,n) | n$ then $l \cdot gcd(m,n) | l\cdot n$

QED

##### Proof of 2

RTP: $\forall d \in \mathbb{N}. d|l\cdot m \land d|l \cdot n \implies d| l\cdot gcd(m,n)$

Let $d$ be an arbitrary positive integers such that $d|l \cdot m$ and $d | l \cdot n$

RTP: $d | l\cdot gcd(m,n)$

From $d|l \cdot m$ and $d | l \cdot n$ we have that $d|gcd(l\cdot m, l \cdot n)$

RTP: $gcd(l \cdot m, l \cdot n) | l \cdot gcd(m,n)$ as therefore $d|l\cdot gcd(m,n)$

By the properties of $gcd(l\cdot m, l\cdot n)$,

$l|l \cdot m \land l| l\cdot n \implies l| gcd(l \cdot m, l \cdot n)$

Hence $gcd(l \cdot m, l \cdot n) = l \cdot k$ for an integer $k$

Also $gcd(l\cdot m, l \cdot n) | l \cdot m$ and $gcd(l\cdot m, l \cdot n) | l \cdot m$

Thus $l \cdot m = gcd(l \cdot m, l \cdot n) \cdot a = l \cdot k \cdot a$ for some integer $a$
and $l \cdot n = gcd(l \cdot m, l \cdot n) \cdot b = l \cdot k \cdot b$ for some integer $b$

It follows that $m=k \cdot a$ and $n = k \cdot b$ by [[Cancellation]].

So $k|m$ and $k|n$, therefore $k|gcd(m,n)$ so $l\cdot k| l \cdot gcd(m,n)$

Since $l \cdot k = gcd(l\cdot m, l \cdot n)$, we have that $gcd(l\cdot m, l \cdot n)| l \cdot gcd(m,n)$
QED.