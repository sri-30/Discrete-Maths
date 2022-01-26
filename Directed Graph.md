# Definition
A directed graph $(A, R)$ consists of a set $A$, and a relation $R$ on $A$ (i.e. a relation from $A$ to $A$).

![[Pasted image 20220126164616.png]]

$R \subseteq A \times A$
There is a connection from $s$ to $t$ iff $(s, t) \in R$

$(Rel(A), id_A, \circ)$ is a [[Monoid]].

Given $R \in Rel(A)$
$R, R \circ R, R \circ R \circ R, ... \text{n times}$
$R^{\circ(1)}, R^{\circ(2)}, R^{\circ(3)} ... R^{\circ(n)}$

By definition: $R^{\circ (\emptyset)} = id_A$
$R^{\circ(n+1)} = R^{\circ(n)} \circ R = R \circ R^{\circ(n)}$


$$x R^{\circ(2)} y \iff \exists z. x R z \land z R y$$

# Definition
For $R \in Rel(A)$ let

$$R^{\circ *} = \bigcup \set{R^{\circ n} \in Rel(A) | n \in \mathbb{N}} = \bigcup_{n \in \mathbb{N}} R^{\circ n}$$
[[Corollary 115]]
