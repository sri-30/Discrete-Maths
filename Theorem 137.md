For all $m, n \in \mathbb{N}$,
![[Pasted image 20220205172143.png]]
![[Pasted image 20220205172257.png]]
![[Pasted image 20220205172531.png]]
$$\forall m, n \in \mathbb{N}. ([m] \Rightarrow [n]) \cong [n^m]$$
By induction:

$m = 0$: $([0] \Rightarrow [n]) \cong [n^0] = [1]$

There is a unique function from $\emptyset$ to any other set, namely the empty relation.

$m = k+1$ $[k] \Rightarrow [n] \cong [n^k]$

RTP: $[k+1] \Rightarrow [n] \cong [n^{k+1}]$
$([k+1] \Rightarrow [n])\cong ([k] \uplus [1]) \Rightarrow [n]$
$\cong ([k] \Rightarrow [n]) \times ([1] \Rightarrow [n])$
$\cong [n^k] \times [n]$
$\cong [n^k \cdot n]$
$\cong [n^{k+1}]$

QED