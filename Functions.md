$$(A \rightarrow B) \subseteq (A \rightharpoonup B) \subseteq Rel(A, B)$$
A partial function is said to be total, and referred to as a (total) function or map, whenever its domain of definition coincides with its source.

![[Pasted image 20220126203606.png]]

For all $f \in Rel(A, B)$

$$f \in (A \rightarrow B) \iff \forall a \in A. \exists! b \in B. a f b$$
![[Pasted image 20220126204104.png]]

![[Pasted image 20220126204225.png]]
![[Pasted image 20220127000059.png]]
![[Pasted image 20220127000611.png]]
![[Pasted image 20220127000731.png]]
![[Pasted image 20220127002214.png]]
![[Pasted image 20220127003350.png]]
![[Pasted image 20220127003408.png]]

Lemma: r is (a, f)-closed
Corllary: R is total

$$\forall n \in \mathbb{N}. \exists x \in A. n r x$$
Proof: By Induction

Base case: $n=0$. RTP: $\exists x \in A. 0 r x$
This is true by the definition of (a, f)-closed

Inductive Step: For $n \in \mathbb{N}$

(IH): $\exists x \in A. n r x$
(RTP): $\exists y \in A. (n+1) r y$

Indeed if $n r x$ then $(n+1) r f(n,x)$, since $r$ is (a,f)-closed.

Proposition: $r$ is functional
There is only one pair $(n,x)$ in $r$ for all $n$.

Proof: By Induction

Base case: $n=0$ We know $(n,R) \in r$
Consider $r' \subseteq \mathbb{N} \times A$
$(0, a) \in r'$
$(n,x) \in r' \forall n \geq 1, \forall x$
$r \subseteq r'$ which is (a,f)-closed
hence $r'$ is functional at $0$ and so is $r$.

Inductive step:

IH- Suppose that $r$ is functional at $n$

Consider $r' \subseteq \mathbb{N}