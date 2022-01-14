Let $m$ and $m'$ be natural numbers and let $n$ be a positive integer such that $m \cong m' \mod {n}$.

Then $CD(m,n)=CD(m',n)$

Let $m,m'$ be natural numbers. Let $n$ be a positive integer.

Assume $m \cong m' \mod {n}$

RTP: {$d \in \mathbb{N} : d|m \land d|n$} = {$d \in \mathbb{N} : d|m' \land d|n$}

Equivalently [$\forall d \in \mathbb{N} . (d|n \land d|m) \iff (d|m' \land d|n)$]

Let $d$ be a natural number. 
1. Assume $d|m$ and $d|n$.
	RTP: $d|m'$ and $d|n$
	$d|n$ is trivially true, so $n = i \cdot d$ for some integer $i$
	$d|m \implies m = k \cdot d$ for some integer $k$
	$m \cong m' \mod {n} \implies m - m' = j \cdot n$ for some integer $j$
	$m' = m - j \cdot n = k\cdot d - j \cdot i \cdot d = d \cdot (k - j\cdot i)$ hence $d|m$
	QED.
2. Assume $d|m'$ and $d|n$
	RTP: $d|m$ and $d|n$
	[[Unfinished]]