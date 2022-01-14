For every positive integer $m$, the integers modulo $m$ are:

$\mathbb{Z}_m : 0,1,...,m-1$
with arithmetic operations of addition $+_m$ and multiplication $\cdot_m$ defined as follows
$k+_ml = [k+l]_m = rem(k+l, m),$
$k \cdot_m l=[k \cdot l]_m = rem(k \cdot l, m)$
for all $0 \leq k,l < m$

![[Pasted image 20211210151920.png]]
![[Pasted image 20211210152053.png]]
Interestingly, 3 is its own multiplicative inverse in $\mathbb{Z_4}$

![[Pasted image 20211210183821.png]]
According to fermat's little theorem, 
For a prime $p$, $i \ncong 0 \mod {p}$ 
$i^{p-2} \cdot i \cong 1 \mod {p}$
So every number which is not zero in modular arithmetic has a multiplicative inverse.